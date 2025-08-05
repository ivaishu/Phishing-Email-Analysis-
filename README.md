# 🛡️ Phishing Email Analysis

This project is part of a cybersecurity internship task. The objective is to analyze a suspicious email and identify characteristics commonly used in phishing attacks.

---

## 📂 Project Files

| File Name              | Description                                      |
|------------------------|--------------------------------------------------|
| `Sample_email.eml`     | Real phishing email sample from [phishing_pot GitHub repository](https://github.com/rf-peixoto/phishing_pot) |
| `header_analysis.md`   | In-depth header analysis and verdict             |
| `Google_Tool_Box_Header_Analyzer.png` |Screenshot of SPF, DKIM, and DMARC results |
---

## 🧠 Task Objective

Analyze a phishing email sample and identify red flags using technical and visual cues.

---

## 🧪 Tools Used

- 📧 **Email Sample Source**: [rf-peixoto/phishing_pot](https://github.com/rf-peixoto/phishing_pot)
- 🛠️ **Header Analysis Tool**: [Google Admin Toolbox - Message Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/analyzeheader)

---

## 🔍 Header Analysis

See detailed analysis in the [`header_analysis.md`](./header_analysis.md) file.  
It includes breakdowns of SPF, DKIM, DMARC, source IP, reply-to mismatches, and server hops.

---

## 🚨 Phishing Traits Found

- **Spoofed sender**: Pretends to be from Microsoft, but the domain is fake (`access-accsecurity.com`).
- **No SPF/DKIM records**: Sender domain has no email authentication mechanisms.
- **Broken DMARC policy**: No policy enforcement for spoofed messages.
- **Suspicious reply-to**: Redirects responses to a Gmail address.
- **Scare tactic**: Claims "unusual login activity" to trigger fear.
- **Mismatch between visual and technical sender**.
- **HTML email** with embedded links to report a false incident, typical social engineering pattern.

---

## 🎯 Learning Outcome

- Developed email header analysis skills
- Identified real-world phishing red flags
- Understood SPF, DKIM, and DMARC mechanisms

---
## 📚 Learning Outcomes
- Developed hands-on skills in analyzing real-world phishing emails
- Understood technical and psychological tactics used by attackers
- Learned to use header analysis tools and critical inspection methods
