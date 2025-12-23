# Mutillidae SQL Injection Lab

## Overview
This repository documents a hands-on security lab demonstrating **SQL Injection vulnerabilities** in the **Mutillidae (OWASP Top 10) deliberately vulnerable web application**.  
The focus is on identifying, analyzing, and documenting the vulnerability in a controlled environment.

---

## Target Application
- **Application:** Mutillidae (Born to be Hacked)
- **Version:** 2.1.19
- **Category:** OWASP Top 10 – Injection
- **Environment:** Local isolated lab

---

## Vulnerability Scope
- Authentication-based SQL Injection
- Error-based SQL Injection
- Input manipulation in login workflow
- Database enumeration through injectable parameters

---

## High-Level Attack Flow
1. Identify vulnerable login input fields
2. Inject crafted SQL payloads
3. Observe SQL error disclosure
4. Manipulate backend SQL queries
5. Enumerate database structure
6. Demonstrate potential data exposure

---

## Evidence
Screenshots are stored in the `assets/` directory and named according to the attack stage.


> Note: Sensitive information such as database names and records has been **masked or blurred** for responsible disclosure.

---

## Impact
If present in a production system, this vulnerability could result in:
- Authentication bypass
- Unauthorized database access
- Exposure of sensitive user data
- Full backend compromise

---

## Mitigation
- Use prepared statements / parameterized queries
- Validate and sanitize all user input
- Disable verbose SQL error messages
- Apply least-privilege database access
- Implement proper logging and monitoring

---

## Legal Disclaimer
This project is intended **strictly for educational purposes**.
All testing was performed on deliberately vulnerable software in a controlled lab environment.
Do not attempt these techniques on systems without explicit authorization.

---

## License
MIT License

