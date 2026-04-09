<div align="center">

# HackTheBox Writeups · George Nădejde

**🌐 [georgenadejde.github.io/htb](https://georgenadejde.github.io/htb)**

*Writeups and notes from HackTheBox machines.*

![Status](https://img.shields.io/badge/status-active-00ff88?style=flat-square&labelColor=0a0d0f)
![Platform](https://img.shields.io/badge/platform-HackTheBox-9fef00?style=flat-square&labelColor=0a0d0f)

</div>

---

## About

This repo contains my writeups and notes for HackTheBox machines. Each writeup documents the full methodology: enumeration, exploitation, privilege escalation, and key takeaways.

Machine selection follows the [TJ Null OSCP prep list v3](https://docs.google.com/spreadsheets/d/1dwSMIAPIam0PuRBkCiDI88pU3yzrqqHkDtBngUHNCw8/edit) (PEN-200 2023-2024).

**Mindset:**
- Minimum 2 hours of genuine effort before reading any hints
- If I read a writeup, I reset the box and do it again from scratch without looking
- Document everything during the attempt, not after.

---
## Progress

### Linux

| #  | Machine     | Difficulty | Status |
|----|-------------|------------|--------|
| 1  | Help        | Easy       |        |
| 2  | Networked   | Easy       |        |
| 3  | Busqueda    | Easy       |        |
| 4  | Broker      | Easy       |        |
| 5  | Sau         | Easy       |        |
| 6  | Editorial   | Easy       |        |
| 7  | BoardLight  | Easy       |        |
| 8  | Dog         | Easy       |        |
| 9  | Titanic     | Easy       |        |
| 10 | Magic       | Medium     |        |
| 11 | Pandora     | Easy       |        |
| 12 | Soccer      | Easy       |        |
| 13 | CozyHosting | Easy       |        |
| 14 | Usage       | Easy       |        |
| 15 | LinkVortex  | Easy       |        |
| 16 | Intentions  | Medium     |        |
| 17 | Monitored   | Medium     |        |
| 18 | UpDown      | Medium     |        |
| 19 | StreamIO    | Medium     |        |
| 20 | Mailing     | Medium     |        |

### Windows

| #  | Machine       | Difficulty | Status |
|----|---------------|------------|--------|
| 1  | Access        | Easy       |        |
| 2  | Heist         | Easy       |        |
| 3  | Jeeves        | Medium     |        |
| 4  | ServMon       | Easy       |        |
| 5  | Timelapse     | Easy       |        |
| 6  | Return        | Easy       |        |
| 7  | Builder       | Medium     |        |
| 8  | Keeper        | Easy       |        |
| 9  | Aero          | Medium     |        |
| 10 | Manager       | Medium     |        |
| 11 | Cicada        | Easy       |        |
| 12 | Administrator | Medium     |        |
| 13 | Certified     | Medium     |        |

### Active Directory

| #  | Machine    | Difficulty | Status |
|----|------------|------------|--------|
| 1  | Active     | Easy       |        |
| 2  | Forest     | Easy       |        |
| 3  | Support    | Easy       |        |
| 4  | Sauna      | Easy       |        |
| 5  | Monteverde | Medium     |        |
| 6  | Cascade    | Medium     |        |
| 7  | Intelligence | Medium   |        |
| 8  | Escape     | Medium     |        |
| 9  | Flight     | Hard       |        |
| 10 | Blackfield | Hard       |        |

---

## Writeup Structure

```
MachineName/
├── README.md        <- full writeup
├── nmap/            <- scan outputs
└── screenshots/     <- annotated evidence
```

```yaml
---
title: "Machine Name"
os: Linux
difficulty: Medium
description: "One line summary of the key vulnerability."
tags:
  - web
  - sqli
  - privesc
date: YYYY-MM-DD
status: complete
---
```
---

<div align="center">

[georgenadejde.github.io/htb](https://georgenadejde.github.io/htb) · [Portfolio](https://georgenadejde.github.io) · [GitHub](https://github.com/georgenadejde)

</div>