# 🔐 FUTURE_CS_01 — Vulnerability Assessment Report

> **Future Interns — Cyber Security Track (CS)**  
> Task 1 | Web Application Security Audit

---

## 📌 About This Task

This repository contains a professional **Vulnerability Assessment Report** for a web application, completed as part of the **Future Interns Cyber Security Internship**.

The goal was to analyze a public-facing web application for common security weaknesses, classify risks in a business-friendly way, and suggest practical remediation steps — thinking like a **security consultant, not an attacker**.

---

## 🌐 Website Tested

| Field | Details |
|-------|---------|
| **Application Name** | TaskFlow — Student Task Manager |
| **File Analysed** | `student-task-manager.html` |
| **Type** | Single-Page Application (SPA) — fully client-side |
| **Tech Stack** | HTML5, CSS3, Vanilla JavaScript (ES6+) |

---

## 🎯 Scope of Audit

- ✅ Client-side HTML & JavaScript source code review
- ✅ Authentication flow analysis
- ✅ Sensitive data exposure check
- ✅ Security headers assessment
- ✅ Session management review
- ✅ Input handling & XSS surface analysis
- ❌ No active exploitation
- ❌ No brute-force attacks
- ❌ No denial-of-service testing
- ❌ No login bypass attempts

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| Browser DevTools (View Source) | Identify hardcoded data & client-side logic |
| Static Code Review (Manual) | Analyse authentication, data handling, input validation |
| OWASP Top 10 Reference | Classify vulnerabilities against industry standard |
| securityheaders.com (methodology) | Identify missing HTTP security headers |

---

## 🔍 Findings Summary

| ID | Vulnerability | Risk Level |
|----|--------------|------------|
| VUL-01 | Hardcoded Credentials in Client-Side Source Code | 🔴 Critical |
| VUL-02 | No Server-Side Authentication — Auth Bypass via DevTools | 🟠 High |
| VUL-03 | Student PII Stored in Client-Side JavaScript | 🟠 High |
| VUL-04 | No HTTPS / Secure Transport Enforcement | 🟠 High |
| VUL-05 | Missing Security Headers (CSP, X-Frame-Options, etc.) | 🟡 Medium |
| VUL-06 | Passwords Stored Without Hashing | 🟡 Medium |
| VUL-07 | No Session Management or Timeout | 🟢 Low |

**Total: 7 Vulnerabilities — 1 Critical, 3 High, 2 Medium, 1 Low**

---

## 📂 Repository Contents

```
FUTURE_CS_01/
├── README.md                                        # This file
├── student-task-manager.html                        # Target web application
└── FUTURE_CS_01_Vulnerability_Assessment_Report.docx  # Full audit report
```

---

## 📄 Full Report

The complete **Vulnerability Assessment Report** is available in this repository:  
📥 `FUTURE_CS_01_Vulnerability_Assessment_Report.docx`

It includes:
- Executive Summary
- Scope & Methodology
- Detailed findings (What / Why / Evidence / Fix)
- Remediation Priority Plan
- Positive Security Observations
- Tools & Techniques Used

---

## ⚖️ Disclaimer

This security audit was conducted **for educational purposes only** as part of the Future Interns Cyber Security Internship programme. All analysis was performed using **passive, read-only techniques only**. No active exploitation, brute-force, injection, or denial-of-service testing was performed at any point.

---

## 👤 Author

**Internship Track:** Cyber Security (CS)  
**Programme:** Future Interns  
**Repository:** `FUTURE_CS_01`

[![Future Interns](https://img.shields.io/badge/Future%20Interns-Cyber%20Security-teal?style=for-the-badge)](https://www.linkedin.com/company/future-interns)
