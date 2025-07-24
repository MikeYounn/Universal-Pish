# 🎣 UniversalPish — Unified Phishing URL Feed

**UniversalPish** is a centralized, deduplicated, and regularly updated list of known phishing URLs.  
It aggregates multiple trusted public phishing intelligence sources into a single `.txt` file for easy consumption by:

- 🔍 SOC teams and analysts
- 🛡️ SIEM platforms (e.g., Sentinel, Splunk, etc.)
- 🤖 Threat Intelligence pipelines
- 🧪 Cybersecurity research

---

## 📦 What's Inside?

The core of this repository is:


- ✅ Plaintext file (1 URL per line)
- ✅ Updated **hourly** via private automation
- ✅ Pulled from open-source threat intel feeds

---

## 📡 Sources Used

This feed currently aggregates phishing URLs from:

- [OpenPhish](https://openphish.com/)
- [PhishTank](https://phishtank.org/)
- [URLHaus (Abuse.ch)](https://urlhaus.abuse.ch/)
- [Phishing.Database (mitchellkrogza)](https://github.com/mitchellkrogza/Phishing.Database)

More sources are being integrated.

---

## 🧠 Use Cases

- Correlate phishing domains/URLs in your SIEM
- Enrich alerts with known indicators
- Block phishing traffic at proxy/firewall
- Feed into SOAR or detection pipelines

---

## ⚠️ Disclaimer

> **This list is for security research, detection, and defense purposes only.**
> Do **not** visit any of the URLs listed unless in a secure sandboxed environment.

---

## 👷 Maintainer

Maintained by [@MikeYounn](https://github.com/MikeYounn)  
If you want to contribute or suggest feed sources, open an [Issue](https://github.com/MikeYounn/Universal-Pish/issues).

---

## 📜 License

This repository is distributed under an open and fair use security research principle.  

---

## 📜 Note

This repository was inspired by [NoMorePhish](https://github.com/NoMorePhish) and his [Tycoon2FADomains](https://github.com/NoMorePhish/Tycoon2FADomains) :")
