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

Offline CI/CD pipeline security linter (GitHub Actions, GitLab, Bitbucket, Azure, Drone)

---

## ✨ Features

- Stdlib YAML-lite parser (anchors, merge keys, flow, block scalars, multi-doc) with line tracking
- GitHub Actions, GitLab CI, Bitbucket, Azure, Drone engines + generic shell analyzer
- Taint tracking: untrusted context → env → step / job outputs → shell (second-order injection)
- CWE / MITRE ATT&CK / OWASP CICD-SEC-1..10 mapping, inline suppression, score & grade
- TXT / MD / JSON / CSV / SARIF export, --demo test
- Read-only: never executes or modifies pipelines

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OCiPipe
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
