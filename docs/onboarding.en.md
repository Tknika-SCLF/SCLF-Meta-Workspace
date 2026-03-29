# 🚀 SCLF Onboarding Guide

Tknika — Smart Collaborative Learning Factory

---

## 🌍 Select language / Hautatu hizkuntza / Selecciona idioma

- 🇬🇧 [English](onboarding.en.md)  
- 🇪🇺 [Euskara](onboarding.eu.md)  
- 🇪🇸 [Español](onboarding.es.md)  

---

## 🎯 Objective

This document explains how to start working in the SCLF ecosystem. The architecture is based on three fundamental principles:

- 👉 No monorepo
- 👉 No submodules
- 👉 Everything is modular

## 🧩 System Structure

SCLF is composed of multiple independent repositories. Each one functions as an autonomous project:

- `sclf-drone`
- `sclf-gripper`
- `sclf-computer-vision`
- `sclf-ikasmes`
- `sclf-xplanar`
- etc.

**Note:** Only clone the modules you are going to use to keep your environment lightweight.

## 🖥️ Initial Setup

### 1. Create Workspace Folder

```bash
mkdir SCLF
cd SCLF
```

### 2. Clone Necessary Repositories

```bash
git clone git@github.com:Tknika-SCLF/sclf-drone.git
git clone git@github.com:Tknika-SCLF/sclf-gripper.git
git clone git@github.com:Tknika-SCLF/sclf-computer-vision.git
```

## 🔐 Authentication (Recommended)

To avoid constantly asking for credentials, using SSH is recommended.

Generate key:

```bash
ssh-keygen -t ed25519 -C "your_email"
```

Then, add the public key to your GitHub configuration.

## 🧠 Workflow Methodology

### Standard Git Flow

For any contribution, follow these steps within the corresponding repository:

1. **Enter the repo**
   ```bash
   cd sclf-drone
   ```
2. **Update the main branch and create a new branch**
   ```bash
   git checkout main
   git pull
   git checkout -b feature/name-of-the-improvement
   ```
3. **Work and commit**
   ```bash
   git add .
   git commit -m "feat: clear description of the changes"
   ```
4. **Push changes**
   ```bash
   git push origin feature/name-of-the-improvement
   ```
5. **Pull Request**
   Create the PR directly in the GitHub interface.

## ⚠️ Important Rules

### ✅ Do's
- Use branches for every change
- Review changes before running scripts
- Keep repositories small and clear

### ❌ Don'ts
- Do not work on `main` directly
- Do not use submodules
- Do not run code without understanding it

## 🧪 Security (Very Important)

If you work with AI assistance:

👉 **Never run auto-generated scripts without supervision.**

**Always:**
- Read the code
- Understand its logic
- Run it manually

## 🧰 Recommended Environment

- **WSL:** Linux within Windows for better compatibility
- **VSCode / Antigravity:** as the main working environment
- **Docker:** optional, but recommended for process isolation

## 📂 Meta-Workspace

Regarding this main repository:

- ❌ It is not a development environment
- ✅ It is an index and entry point to the ecosystem

## 🧭 Summary

- Clone only what is necessary
- Work modularly by repositories
- Always use branches
- Review thoroughly before executing
