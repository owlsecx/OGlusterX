# 🦉 OGlusterX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OScan-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OGlusterX** — GlusterFS Configuration Hardening Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

GlusterFS configuration hardening auditor (volumes, volfiles, glusterd, TLS, gNFS, Ganesha-Gluster)

---

## ✨ Features

- Stdlib parsers for `gluster volume info`, `gluster volume get <vol> all`, /var/lib/glusterd/vols/*/info, *.vol volfiles, glusterd.vol, gsyncd.conf, glusterd.info, /etc/fstab and NFS-Ganesha EXPORT blocks (FSAL GLUSTER)
- Volume access — auth.allow / auth.reject / auth.ssl-allow, I/O + management TLS (secure-access), cipher lists
- Legacy gNFS exposure, insecure ports, root squash
- Integrity — client / server quorum, replica & arbiter, bitrot scrubbing, self-heal, split-brain policies
- Data exposure — trash, DEBUG/TRACE logs, brick perms, storage.owner-uid 0, plaintext brick credentials
- Geo-replication root SSH / host-key verification
- TLS key / CA / cert presence & permission checks
- Secrets masked everywhere; --root discovery; CWE + MITRE
- Export TXT / Markdown / JSON / CSV / SARIF 2.1.0
- Self-test --demo, CI gates --fail-on / --min-severity

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OGlusterX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
