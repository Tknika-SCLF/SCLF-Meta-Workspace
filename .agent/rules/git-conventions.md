---
trigger: always_on
---

# Git Conventions — SCLF

## 1. Branch Strategy

Use one branch per change.

Naming:

- feature/<name>
- fix/<name>
- docs/<name>
- refactor/<name>
- chore/<name>

Examples:
- feature/gripper-control
- fix/drone-connection
- docs/readme-update

---

## 2. Workflow

Always:

1. Create branch from main
2. Make changes
3. Commit
4. Push
5. Open Pull Request

Never work directly on main.

---

## 3. Commit Messages

Format:

<type>: short description

Types:

- feat: new functionality
- fix: bug fix
- docs: documentation
- refactor: code improvement
- chore: maintenance

Examples:

- feat: add gripper control module
- fix: correct camera calibration bug
- docs: update onboarding guide

Rules:

- use lowercase
- be concise
- one logical change per commit

---

## 4. Pull Requests

PR must:

- have clear title
- describe what changed
- explain why
- be small and focused

Avoid:

- large PRs
- unrelated changes in same PR

---

## 5. Protected Branches

- main is protected
- no direct pushes
- PR required

---

## 6. Repository Independence (SCLF Rule)

Each repository is independent.

Do NOT:

- create cross-repo commits
- depend on local changes from another repo
- assume synchronized updates

If coordination is needed:

- document it
- use versioning or APIs

---

## 7. Sync with Remote

Keep branch updated:

git pull --rebase origin main

Avoid merge commits unless necessary.

---

## 8. Clean History

- avoid unnecessary commits
- squash if needed before merge
- keep history readable