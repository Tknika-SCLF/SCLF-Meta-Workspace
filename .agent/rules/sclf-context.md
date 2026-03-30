---
trigger: always_on
---

# SCLF — AI Agent Context

## Architecture

- Fully modular system
- No monorepo
- No git submodules
- Each component = independent repository
- Meta-Workspace = index only (NOT a development environment)

## Repositories

Examples:
- sclf-drone
- sclf-gripper
- sclf-computer-vision
- sclf-ikasmes
- sclf-xplanar

Do not assume shared codebase unless explicitly defined.

## Development Model

Always follow:

branch → commit → push → pull request → merge

Never:
- work directly on main
- bypass PR workflow

## Branch Naming

- feature/<name>
- fix/<name>
- docs/<name>
- refactor/<name>

## Commit Convention

- feat: new functionality
- fix: bug fixes
- docs: documentation
- refactor: internal improvements
- chore: maintenance

## Design Principles

- Keep repos independent
- Avoid tight coupling between projects
- Prefer simple and explicit solutions
- No hidden dependencies between repos
- Each repo must be runnable and understandable on its own

## Anti-Patterns (DO NOT DO)

- Do not introduce monolithic structures
- Do not suggest submodules
- Do not centralize logic across repos without clear API boundaries
- Do not assume shared runtime unless defined

## Security Rules

- Never execute scripts blindly
- Always explain what code does before suggesting execution
- Avoid auto-generated unsafe commands

## Agent Role

You must:
- Propose modular solutions
- Respect repository boundaries
- Help structure projects before coding
- Suggest clean architectures over quick hacks

## Response Style

- Be direct and technical
- Avoid unnecessary explanations
- Prefer structure over verbosity
- When proposing solutions:
  1. Explain structure
  2. Then show implementation