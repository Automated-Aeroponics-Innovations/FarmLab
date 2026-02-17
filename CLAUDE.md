# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## ⚡️ Initialization (The Standard Protocol)

**Before starting work:**

1. **Activate Venv:** `source /home/griermarkov/Drives/.virtual-environments/FarmLab_env/bin/activate`
2. **Initialize:** Run `/init` to sync and update dependencies.

### /init Command

```bash
# Pull latest changes and install dependencies
git pull origin $(git branch --show-current) && \
  pip install -r requirements.txt 2>/dev/null || \
  pip install -e . 2>/dev/null || \
  echo "No installable dependencies found"
```

### /save-point Command

Smart commit workflow that respects .gitignore and pushes to remote:

```bash
# Phase XV: Federation Save Point
git status
git add .
git commit -m "Phase XV: Federation Infrastructure Update"
git push origin HEAD
```

**Usage:** Run `/save-point` to checkpoint your work.


---

## Project: FarmLab
> **Profile:** aals
> **Identity:** aals / id_ed25519_aals
> **Stack:** Documentation, Markdown, Research PDFs

## Description
Documentation hub and research foundation for ML-operated aeroponics systems targeting scalable vertical farming and food insecurity solutions.

## R&D Team Assignments
* **Architect:** `system-architect` (Use for design & documentation structure)
* **Builder:** `polyglot-dev` (N/A - documentation repo)
* **Researcher:** `quantum-ag-researcher` (Use for research synthesis and literature review)
* **Ops:** `infrastructure-ops` (N/A - documentation repo)
* **Guardian:** `security-qa` (N/A - documentation repo)

## Commands
* **Build:** N/A (documentation repository)
* **Test:** N/A
* **Lint:** N/A

## Key Content
- Comprehensive research on aeroponics and digital agriculture
- Nanoengineered IoT biosensor integration guidance
- MLOps CI/CD pipeline design for precision agriculture
- References to NASA ISS research and Cornell digital agriculture
- Hardware tool stack documentation (3D printers, CAD tools)

## Federation Context
* **Root:** `~/Drives/data/SynologyDrive/grimmerie/repositoriies-by-profile`
* **Sibling Projects:** You are authorized to traverse `../` to reference other repos in the aals profile.
* **Related Repos:** FarmLab-Product-Development (hardware/CAD implementation)
