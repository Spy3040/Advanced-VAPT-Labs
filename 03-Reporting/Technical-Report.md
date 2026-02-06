## Purpose : 
This is for:
    Developers
    Security engineers
    Blue team

# Technical Findings Report

## Finding 001 – SQL Injection

Severity: Critical  
CVSS Score: 9.1  
OWASP Category: A03 – Injection

### Description
The application fails to properly validate user-supplied input, allowing attackers to manipulate backend SQL queries.
### Impact
An attacker could bypass authentication controls, retrieve sensitive database information, or modify application data.
### Evidence
Manual testing revealed abnormal application behavior when special characters were injected into input fields.
### Remediation
Implement parameterized queries (prepared statements) and enforce strict server-side input validation.


## Finding 002 – Broken Authentication

Severity: High  
CVSS Score: 7.5  
OWASP Category: A07 – Identification and Authentication Failures

### Description
The application allows unlimited login attempts without enforcing rate limiting or account lockout mechanisms.
### Impact
Attackers can perform brute-force attacks to compromise valid user accounts.
### Remediation
Implement rate limiting, account lockout after multiple failed attempts, and strong password policies.

# Findings Table

| Finding ID | Vulnerability    | CVSS Score | Remediation            |
|-----------|------------------|------------|------------------------|
| F001      | SQL Injection    | 9.1        | Input validation       |
| F002      | Weak Password    | 7.5        | Enforce complexity    |

