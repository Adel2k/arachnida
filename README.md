# 🕷️ ArachNida

A cross-platform, modular web vulnerability scanner and reconnaissance toolkit built for ethical hacking, research, and red team operations. Designed for use in controlled, legal environments such as CTFs, penetration testing labs, or educational projects.

---

## 📖 Table of Contents

- [About](#about)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Modules](#modules)
- [Testing Environment](#testing-environment)
- [Limitations](#limitations)
- [Author](#author)
- [Disclaimer](#disclaimer)

---

## 📌 About

**ArachNida** is a lightweight, extendable toolkit built for identifying common web vulnerabilities and performing active recon tasks. It leverages modular scripts and scanners to allow for customized workflows.

**Educational Use Only. Not for unauthorized deployment.**

---

## ✨ Features

- ✅ Port Scanning (TCP/UDP)
- ✅ Directory brute-forcing
- ✅ Web vulnerability detection:
  - XSS
  - SQL Injection
  - Open Redirect
- ✅ CVE lookups for services
- ✅ Customizable payload injection
- ✅ JSON reporting system
- ✅ Modular code structure for plugin-based scanners

---

## 🛠️ Installation

Clone the repository:
```bash
git clone https://github.com/Adel2k/arachnida.git
cd arachnida
````

Install dependencies (if required):

```bash
pip install -r requirements.txt
```

---

## ⚙️ Usage

Basic usage:

```bash
python3 arachnida.py --target https://example.com
```

Available options:

```
--target        URL of target site
--scan-ports    Run port scan
--dirbuster     Run directory brute-forcing
--vuln-scan     Run vulnerability scanner
--output        Save results to a JSON file
```

Example:

```bash
python3 arachnida.py --target https://victim.local --scan-ports --vuln-scan --output result.json
```

---

## 📦 Modules

| Module        | Description                                |
| :------------ | :----------------------------------------- |
| **portscan**  | TCP/UDP port scanner                       |
| **dirbuster** | Brute-force directories and files          |
| **vulnscan**  | Detects common web vulns (XSS, SQLi, etc.) |
| **cvecheck**  | Looks up known CVEs by service banner      |
| **reporter**  | Generates and saves scan reports           |

---

## 🧪 Testing Environment

* ✅ Ubuntu VM
* ✅ Kali Linux
* ✅ Parrot OS
* ✅ Legal test domains / CTF challenges

Monitored with:

* Wireshark
* Burp Suite
* netstat

---

## ⚠️ Limitations

* No multithreading (planned for future)
* Only supports HTTP/HTTPS
* Intended for local or lab environments
* Some false positives in brute-force modules

---

## 👩‍💻 Author

**Adeline Eminian**
GitHub: [@Adel2k](https://github.com/Adel2k)

---

## ⚠️ Disclaimer

This tool is for **educational and ethical hacking purposes only**.
**Do not use on unauthorized systems.**
The developers assume no responsibility for misuse or damage caused by this tool.

---
