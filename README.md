# NYU Login Portal — Threat Model

This project documents a security threat model for a university authentication system similar to the NYU login portal.  
It demonstrates how to identify, analyze, and mitigate security risks using the STRIDE framework.

## Purpose
The goal is to show practical security documentation used by security engineers and technical writers:
- Model system architecture and trust boundaries
- Identify common authentication threats
- Assess risk severity and likelihood
- Propose mitigations and operational procedures

## System
A web login service with:
- User browser → Web server (DMZ)
- Internal authentication + LDAP directory
- MFA service
- Encrypted session database and audit logs

## Major Risks
- Phishing credential theft
- Session hijacking (XSS)
- SQL / LDAP injection
- Credential stuffing & DDoS
- Authentication bypass / privilege escalation

## Security Controls
- TLS encryption and MFA
- Input validation and parameterized queries
- Secure cookies and CSP headers
- Rate limiting and CAPTCHA
- Logging and incident response procedures

## Outcome
The document shows how structured threat modeling can proactively identify critical risks and guide engineering teams toward secure system design.
