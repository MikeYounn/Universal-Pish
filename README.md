# 🎣 UniversalPhish

This repository contains regularly updated phishing domain feeds aggregated from **multiple public threat intelligence sources**. The feeds are processed and cleaned by a private script, and then pushed to this repository every hour.

## 🔍 About

The purpose of this project is to provide a centralized list of phishing domains that can be used in:

- SIEM tools (e.g., Microsoft Sentinel)
- Detection engineering
- Threat hunting
- SOC monitoring and alerting

## 📁 Feeds

There are **two output files** to accommodate platform limitations:

| Filename | Description |
|----------|-------------|
| `UniversalPish_FULL.txt` | Contains **all known unique phishing domains** from public sources. Best for offline or bulk analysis. |
| `UniversalPish_LIMITED.txt` | Contains **only the most recent 9,500 domains**, optimized to remain below **0.95 MB** for compatibility with Microsoft Sentinel analytic rules. |

### Why Split the Feeds?

Microsoft Sentinel imposes a strict size limit (~0.95 MB) on analytic rule match lists. and a maximum argument capacity of 10000. To ensure compatibility, i limited `UniversalPish_LIMITED.txt` to the latest 9500 domains, while still preserving the full dataset in `UniversalPish_FULL.txt`.

---

## 🧠 Sources Aggregated

- [OpenPhish](https://openphish.com/)
- [PhishTank](https://phishtank.org/)
- [Abuse.ch URLHaus](https://urlhaus.abuse.ch/)
- [Phishing.Database by Mitchell Krogza](https://github.com/mitchellkrogza/Phishing.Database)

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
