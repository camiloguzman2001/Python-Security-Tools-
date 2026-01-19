# 🐍 Python Security Tools

A collection of practical security tools built in Python. Designed for penetration testers, SOC analysts, and security professionals to automate common security tasks.

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![License](https://img.shields.io/badge/License-MIT-green)
![Security](https://img.shields.io/badge/Purpose-Security%20Tools-red)

## 🎯 Tools Included

| Tool | Description |
|------|-------------|
| `port_scanner.py` | Fast multi-threaded port scanner with service detection |
| `hash_cracker.py` | Offline password hash cracker (MD5, SHA1, SHA256, NTLM) |
| `log_analyzer.py` | Parse and analyze Windows/Linux security logs for threats |
| `subnet_scanner.py` | Network discovery tool to find live hosts |
| `password_auditor.py` | Check passwords against breach databases and policies |
| `header_analyzer.py` | HTTP security header checker for web applications |

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/camiloguzman2001/python-security-tools.git
cd python-security-tools

# Install dependencies
pip install -r requirements.txt

# Run a tool
python tools/port_scanner.py --target 192.168.1.1 --ports 1-1000
```

## 🔧 Tool Details

### Port Scanner
Fast, multi-threaded port scanner with banner grabbing.
```bash
python tools/port_scanner.py --target 10.0.0.1 --ports 1-1000 --threads 100
python tools/port_scanner.py --target scanme.nmap.org --ports common
```

### Hash Cracker
Crack password hashes using wordlists or brute force.
```bash
python tools/hash_cracker.py --hash 5f4dcc3b5aa765d61d8327deb882cf99 --type md5 --wordlist rockyou.txt
python tools/hash_cracker.py --hash-file hashes.txt --type ntlm --wordlist passwords.txt
```

### Log Analyzer
Parse security logs and identify suspicious activity.
```bash
python tools/log_analyzer.py --file /var/log/auth.log --type linux
python tools/log_analyzer.py --file Security.evtx --type windows
```

### Subnet Scanner
Discover live hosts on a network.
```bash
python tools/subnet_scanner.py --network 192.168.1.0/24
python tools/subnet_scanner.py --network 10.0.0.0/24 --threads 50
```

### Password Auditor
Check password strength and breach status.
```bash
python tools/password_auditor.py --password "MyP@ssw0rd"
python tools/password_auditor.py --file passwords.txt --check-breach
```

### Header Analyzer
Check web application security headers.
```bash
python tools/header_analyzer.py --url https://example.com
python tools/header_analyzer.py --url-file targets.txt --output report.json
```

## 📋 Requirements

- Python 3.8+
- See `requirements.txt` for dependencies

## ⚠️ Legal Disclaimer

These tools are for authorized security testing and educational purposes only. Always obtain proper authorization before scanning or testing systems you don't own.

## 📄 License

MIT License - See [LICENSE](LICENSE) for details.

## 📬 Contact

**Camilo Guzman** - [LinkedIn](https://linkedin.com/in/camiloguzman) | [GitHub](https://github.com/CamiloSteez)
