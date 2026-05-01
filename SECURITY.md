# Security Policy

## Supported Versions

| Version | Supported |
|---------|-----------|
| 0.1.x (beta) | ✅ Active |

---

## Reporting a Vulnerability

**Please do not report security vulnerabilities through public GitHub Issues.**

If you discover a security issue in AI NutriScan, please report it responsibly by emailing:

**security@nutriscan.ai**

Include as much detail as possible:

- A description of the vulnerability
- Steps to reproduce or proof-of-concept
- The potential impact
- Any suggested mitigations (optional)

### What to expect

- **Acknowledgement** within 48 hours of your report
- **Status update** within 7 days
- **Patch timeline** communicated after initial investigation
- **Credit** in the release notes if you wish (with your permission)

We appreciate responsible disclosure and will work with you to resolve the issue promptly before any public announcement.

---

## Scope

The following are **in scope** for security reports:

- Authentication and authorisation flaws
- Data exposure or privacy leaks (user health data, images, personal information)
- Injection vulnerabilities (SQL, command, etc.)
- Broken access control
- API security issues

The following are **out of scope**:

- Issues in third-party dependencies (please report these upstream)
- Denial of service attacks
- Social engineering or phishing
- Issues already reported or in progress

---

## Security Measures

- All user data is encrypted at rest (AES-256) and in transit (TLS 1.3)
- Images are processed server-side and never stored without explicit user consent
- We are GDPR and UU PDP (Indonesian Personal Data Protection Law) compliant
- Users may export or permanently delete all their data at any time

---

*Thank you for helping keep AI NutriScan and our users safe.*
