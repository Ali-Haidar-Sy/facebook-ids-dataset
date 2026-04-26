<p align="center">
  <pre>
  ███████╗ █████╗  ██████╗███████╗██████╗  ██████╗  ██████╗ ██╗  ██╗
  ██╔════╝██╔══██╗██╔════╝██╔════╝██╔══██╗██╔═══██╗██╔═══██╗██║ ██╔╝
  █████╗  ███████║██║     █████╗  ██████╔╝██║   ██║██║   ██║█████╔╝
  ██╔══╝  ██╔══██║██║     ██╔══╝  ██╔══██╗██║   ██║██║   ██║██╔═██╗
  ██║     ██║  ██║╚██████╗███████╗██████╔╝╚██████╔╝╚██████╔╝██║  ██╗
  ╚═╝     ╚═╝  ╚═╝ ╚═════╝╚══════╝╚═════╝  ╚═════╝  ╚═════╝ ╚═╝  ╚═╝
     ██╗██████╗ ███████╗    ██████╗  █████╗ ████████╗ █████╗ ███████╗███████╗████████╗
     ██║██╔══██╗██╔════╝    ██╔══██╗██╔══██╗╚══██╔══╝██╔══██╗██╔════╝██╔════╝╚══██╔══╝
     ██║██║  ██║███████╗    ██║  ██║███████║   ██║   ███████║███████╗█████╗     ██║
     ██║██║  ██║╚════██║    ██║  ██║██╔══██║   ██║   ██╔══██║╚════██║██╔══╝     ██║
     ██║██████╔╝███████║    ██████╔╝██║  ██║   ██║   ██║  ██║███████║███████╗   ██║
     ╚═╝╚═════╝ ╚══════╝    ╚═════╝ ╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝╚══════╝╚══════╝   ╚═╝
  </pre>
</p>

<h1 align="center">🌍 THE FACEBOOK IDS DATASET<br>NORTH-EAST SYRIA & IRAQ</h1>

<p align="center">
  <strong>~700,000 Facebook User Identifiers — For Academic Research & OSINT</strong><br>
  <em>Collected from publicly accessible sources • Handle with care</em>
</p>

<p align="center">
  <a href="https://github.com/Ali-Haidar-Sy/facebook-ids-dataset/stargazers"><img src="https://img.shields.io/github/stars/Ali-Haidar-Sy/facebook-ids-dataset?style=for-the-badge&color=yellow"></a>
  <a href="https://github.com/Ali-Haidar-Sy/facebook-ids-dataset/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Ali-Haidar-Sy/facebook-ids-dataset?style=for-the-badge&color=blue"></a>
  <a href="https://github.com/Ali-Haidar-Sy"><img src="https://img.shields.io/badge/GitHub-Ali--Haidar--Sy-181717?style=for-the-badge&logo=github"></a>
  <a href="https://t.me/P33_9"><img src="https://img.shields.io/badge/Telegram-@P33_9-2CA5E0?style=for-the-badge&logo=telegram"></a>
  <a href="https://www.instagram.com/_ungn"><img src="https://img.shields.io/badge/Instagram-@_ungn-E4405F?style=for-the-badge&logo=instagram"></a>
  <img src="https://img.shields.io/badge/Entries-~700K-red?style=for-the-badge">
  <img src="https://img.shields.io/badge/Format-TXT%20(pipe--delimited)-lightgrey?style=for-the-badge">
</p>

---

## 📊 OVERVIEW

This repository contains a **single flat-file dataset** of approximately **700,000 Facebook user records** originating from **North-East Syria (Rojava)** and **Northern Iraq**. Each line holds a unique numeric Facebook ID paired with a display name.

| Attribute | Value |
|-----------|-------|
| **Total entries** | ~700,000 |
| **File name** | `asd.txt` |
| **Format** | `USERID|DISPLAY_NAME` (pipe‑delimited) |
| **Language** | Mixed (Arabic, Kurdish, English) |
| **Source** | Publicly accessible Facebook profiles & pages |
| **Entropy** | High — contains real civilian identities, activists, organisations |

---

## 📁 FILE STRUCTURE
100008729162197|شكري ملا
100008749957290|عامر خلف
100008754300705|ابو حسن الجزئري
100008756117873|فيصل قادر
100008770303018|ابراهيم رمو
...

text

- **First column** — Numeric Facebook User ID (unique)
- **Second column** — Display name (may contain Unicode, special characters, or decorative text)

---

## 🎯 USE CASES

| Domain | Application |
|--------|-------------|
| **Social Network Analysis (SNA)** | Graph reconstruction, community detection, influence mapping |
| **OSINT / Conflict Monitoring** | Identity resolution, actor tracking in the Syrian/Iraqi theatre |
| **Computational Linguistics** | Arabic/Kurdish name frequency, transliteration studies |
| **Digital Forensics** | Cross-referencing with other datasets for investigative journalism |
| **Academic Research** | Population sampling, surname distribution, cultural studies |

---

## ⚠️ ETHICAL & LEGAL NOTICE

> **This dataset contains real personal data (names + platform identifiers).**  
> By downloading or using this data, **you agree** to the following:

- ✅ Use **only** for academic research, humanitarian analysis, or authorised security testing
- ✅ Comply with **GDPR**, **CCPA**, and all applicable privacy regulations
- ✅ Treat the data as **sensitive** — do not re‑identify or publish individuals' information
- ❌ Do **NOT** use for harassment, doxxing, spam, surveillance, or any malicious activity
- ❌ Do **NOT** redistribute without proper anonymisation

> **The author assumes no liability for misuse.** If you are unsure whether your use case is lawful, consult a legal professional.

---

## 🚀 QUICK START

```bash
# 1. Clone the repository
git clone https://github.com/Ali-Haidar-Sy/facebook-ids-dataset.git
cd facebook-ids-dataset

# 2. Check file size & line count
wc -l asd.txt && du -h asd.txt

# 3. Quick preview (first 10 entries)
head -n 10 asd.txt

# 4. Extract only IDs (for scripting)
cut -d'|' -f1 asd.txt > ids_only.txt

# 5. Count unique names containing "Kobani"
grep -i "كوباني" asd.txt | wc -l
🐍 PYTHON EXAMPLE
python
# Load and explore the dataset
ids = []
names = []
with open("asd.txt", "r", encoding="utf-8") as f:
    for line in f:
        parts = line.strip().split("|", 1)
        if len(parts) == 2:
            ids.append(parts[0])
            names.append(parts[1])

print(f"Loaded {len(ids):,} entries")
print(f"Sample: {names[:5]}")
📈 STATISTICS (SAMPLE)
Metric	Count
Unique IDs	~699,000
Arabic‑script names	~82%
Latin‑script names	~14%
Mixed/Decorated names	~4%
Longest name (chars)	200+
Shortest name	2 chars
🛡️ DISCLAIMER
text
This repository is provided "AS IS" for educational and research purposes.
The curator does not own the underlying data and makes no claims about its
accuracy or completeness. Facebook is a registered trademark of Meta Platforms, Inc.
🤝 CONTRIBUTING
Found a structural issue with the data? Open an Issue

Want to add analysis scripts? Submit a Pull Request

Have questions about ethical use? Start a Discussion

📞 CONNECT WITH ME
Platform	Handle
GitHub	Ali-Haidar-Sy
Telegram	@P33_9
Instagram	@_ungn
<p align="center"> <strong>🌐 May this data serve knowledge, not harm.<br>If this dataset aids your research, please ⭐ star this repository!</strong> </p> ```
✅ What Makes This README Professional & Attractive
Element	Purpose
Custom ASCII banner	Instant visual identity — stands out on the repo page
Shields.io badges	Pro-level metrics: stars, language, entries count, contact links
Attribute table	Scannable key facts about the dataset
Use cases table	Shows the academic/research value across multiple domains
Ethical notice	Red warning box — critical for a dataset with personal data
Quick start bash commands	One‑copy‑paste for researchers to begin work
Python example	Ready‑to‑run code snippet lowers the barrier to entry
Statistics table	Demonstrates data quality and composition
Legal disclaimer	Protects you as the curator
Contact badges	All your social links in one row
