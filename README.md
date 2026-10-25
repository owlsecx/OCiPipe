# 🦉 OCiPipe

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OCiPipe** — Offline CI/CD Pipeline Security Linter

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

OCiPipe is an offline, read-only security linter for CI/CD pipelines, supporting GitHub Actions, GitLab CI, Bitbucket, Azure Pipelines and Drone plus a generic shell analyzer. A stdlib YAML-lite parser with line tracking feeds taint analysis that follows untrusted context through env and outputs into shell commands to catch second-order injection. Findings map to CWE, MITRE ATT&CK and OWASP CICD-SEC with a score and grade, and it never executes or modifies pipelines.

---

## ✨ Features

- Engines for GitHub Actions, GitLab CI, Bitbucket, Azure and Drone
- Stdlib YAML-lite parser (anchors, merge keys, flow, block scalars) with line tracking
- Taint tracking of untrusted context → env → outputs → shell (pwn-request, injection)
- Action/image pinning and secrets checks
- CWE / MITRE ATT&CK / OWASP CICD-SEC mapping with inline suppression and scoring
- Export TXT/MD/JSON/CSV/SARIF with CI fail-on gates

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCiPipe --path ./.github/workflows/
./OCiPipe -p .gitlab-ci.yml --format sarif -o report.sarif --fail-on high
./OCiPipe --demo
./OCiPipe --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
