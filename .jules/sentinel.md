# Sentinel's Journal

## 2025-05-14 - [Initial Security Assessment]
**Vulnerability:** Lack of Content Security Policy (CSP) and lack of validation for data loaded from IndexedDB.
**Learning:** Even static HTML applications are vulnerable to XSS and data tampering. Relying on client-side storage like IndexedDB without validation can lead to unexpected behavior if the data is manually modified by a user or a malicious script.
**Prevention:** Implement a strict CSP and validate all data retrieved from client-side storage before usage.
