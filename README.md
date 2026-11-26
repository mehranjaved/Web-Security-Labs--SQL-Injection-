# SQL Injection — A-to-Z Practical Learning & Security Assessment Report

**Author:** Mehran  
**Role:** Cybersecurity Student  
**Focus:** Web Application Security  
**Date:** November 2026

## Project overview

This repository section documents foundational SQL Injection concepts and two completed PortSwigger Web Security Academy labs. It combines educational explanations, Burp Suite evidence supplied by the author, analysis of visible HTTP behavior, and defensive recommendations.

The project is an educational portfolio artifact. It does **not** claim real-world client penetration testing, production vulnerabilities, or professional security findings.

## Completed practical labs

1. **SQL injection vulnerability in WHERE clause allowing retrieval of hidden data**
2. **SQL injection authentication bypass**

These are the only two labs claimed as completed in this report.

## Tools used

- Burp Suite Community Edition — HTTP history, request inspection, and Repeater
- Kali Linux — learning and testing environment
- Firefox — browser used with the configured proxy
- PortSwigger Web Security Academy — authorized training labs

## Topics covered

- SQL fundamentals: `SELECT`, `WHERE`, `INSERT`, `UPDATE`, and `DELETE`
- How unsafe query construction can create SQL Injection
- In-band, error-based, UNION-based, boolean-based blind, time-based blind, out-of-band, second-order, and stacked-query concepts
- Evidence-based analysis of the two completed labs
- Burp Suite Proxy, HTTP History, Intercept, and Repeater workflow
- Confidentiality, integrity, availability, and authentication impact
- Parameterized queries, prepared statements, allow-list validation, least privilege, secure ORM usage, and safe error handling
- Authorized testing checklist and professional vulnerability-report structure

## Report contents

See [`SQL_Injection_A_to_Z_Report.pdf`](./SQL_Injection_A_to_Z_Report.pdf) for the full technical report, including:
- Executive summary and SQL fundamentals
- SQL Injection vulnerability classes
- Separate analysis of both completed labs
- Five supplied screenshots, with visible session/credential values redacted
- Burp Suite methodology
- Risk discussion and prevention guidance
- Testing checklist, report template, conclusion, and references

## Evidence

The PDF embeds the five screenshots provided for this report. Sensitive values visible in the original images (such as session data, CSRF values, or credential fields) have been covered in the report copies. The original screenshots should not be published publicly without reviewing them for secrets.

## References

- [PortSwigger Web Security Academy — SQL Injection](https://portswigger.net/web-security/sql-injection)
- [OWASP SQL Injection Prevention Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/SQL_Injection_Prevention_Cheat_Sheet.html)
- [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/)
- [OWASP Juice Shop](https://owasp.org/www-project-juice-shop/)

## Educational and authorized-testing disclaimer

This project is for learning and portfolio demonstration. The practical work described is based on intentionally vulnerable PortSwigger Web Security Academy labs. Test only systems for which you have explicit permission. Do not use these techniques against public services, accounts, or systems outside an authorized scope.

## Suggested repository layout

```text
Web-Security-Labs/
├── README.md
└── SQL-Injection/
    ├── SQL_Injection_A_to_Z_Report.pdf
    ├── README.md
    └── evidence/
        └── screenshots/
            └── (reviewed, redacted evidence images)
```
