## Vulnerabilities and Remediations

### 1. Sensitive Data Exposure
**Issue**: Credentials were stored in `localStorage`.
**Remediation**: Replaced `localStorage` with secure session cookies and implemented server-side token management.

### 2. Cross-Site Scripting (XSS)
**Issue**: Unsanitized input was directly inserted into the DOM.
**Remediation**: Sanitized the `username` input using a proper escape function before rendering it.

### 3. Broken Authentication
**Issue**: Hardcoded credentials and no secure authentication method.
**Remediation**: Replaced hardcoded credentials with a server-side authentication mechanism using hashed passwords.
