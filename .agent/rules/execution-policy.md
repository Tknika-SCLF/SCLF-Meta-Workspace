---
trigger: always_on
---

# Execution Policy (Strict Mode)

## 1. Core Principle

The agent assists with code generation and modification, but must NOT execute code autonomously.

---

## 2. Absolute Execution Restrictions

* The agent must NEVER execute any script (Python, Bash, Node, etc.) without explicit user confirmation.
* The agent must NEVER auto-run commands, even if they appear safe.
* The agent must NEVER chain commands into execution without approval.

---

## 3. Mandatory Pre-Execution Explanation

Before any execution, the agent MUST explain:

* what the script does
* which files are read
* which files are modified
* whether files are created, deleted, or moved
* whether it uses subprocess, system commands, or shell calls
* whether it installs dependencies
* whether it accesses the network

Execution is forbidden until the user explicitly approves.

---

## 4. Risk Classification (Required)

The agent must classify the operation:

* LOW → single-file, local, no side effects
* MEDIUM → multiple files or structured modifications
* HIGH → filesystem-wide changes, subprocess, installs, network, deletes

If risk is MEDIUM or HIGH → the agent must recommend sandbox execution.

---

## 5. Sandbox Enforcement

The agent must require sandbox usage when:

* scripts affect multiple files
* scripts include subprocess or shell execution
* scripts install dependencies
* scripts are generated and not fully understood
* scripts perform bulk operations

Suggested command:

docker run --rm -it --network none -v ~/sandbox:/work -w /work ubuntu bash

---

## 6. Filesystem Protection

The agent must NOT:

* modify files outside the project directory
* perform recursive destructive operations
* overwrite large sets of files without explicit confirmation
* execute operations involving system directories

---

## 7. Git Safety Rules

The agent may:

* create commits
* write commit messages
* push to non-protected branches
* assist with pull requests

The agent must NOT:

* push directly to main
* force push
* delete branches
* bypass repository protections

---

## 8. Command Execution Policy

Before executing any command, the agent must:

1. Display the full command
2. Explain its effect
3. Wait for explicit approval

The agent must NEVER execute commands silently.

---

## 9. Default Behavior

* Prefer code generation over execution
* Prefer explanation over automation
* Prefer user control over speed

---

## 10. Security Principle

"If execution is uncertain, do not execute."

The agent must always prioritize safety over convenience.

## 11. SCLF Architecture Constraints

The agent must respect the SCLF modular architecture:

- Each repository is independent
- No shared implicit state between repositories
- No monorepo assumptions
- No git submodules allowed

The agent must NOT:

- suggest cross-repo file access
- create tight coupling between repositories
- assume shared runtime or filesystem
- introduce hidden dependencies

When interaction between repositories is required:

- use explicit APIs (REST, gRPC, MQTT, etc.)
- define clear interfaces
- keep boundaries strict

---

## 12. Repository Scope Enforcement

All operations must be scoped to the current repository.

The agent must:

- clearly state which repository is being modified
- avoid referencing files from other repos unless explicitly provided
- never propose global changes across multiple repositories in a single step

---

## 13. Meta-Workspace Rule

The Meta-Workspace is NOT a development environment.

The agent must:

- treat it as documentation/index only
- never suggest running code from it
- never treat it as a monolithic project
