# Security Policy 🔐

## Supported Versions

| Version | Supported          |
| -------:| ------------------:|
|  main   | ✅ Security updates |
|  < 1.0  | ⚠️ Best-effort       |

## Reporting a Vulnerability

- **Private issue:** Use GitHub Security Advisory to report vulnerabilities
  privately.
- **Email:** <security@example.com>
- **Response target:** We aim to acknowledge reports within **48 hours**.

**Please do not** publicly disclose vulnerabilities until a fix is released.

## Handling Sensitive Data

- **Client-Side Only:** This application runs entirely in your browser. No
  data is sent to a server unless you specifically export it.
- **IndexedDB:** Data stored via the advanced mockup is saved locally in your
  browser's IndexedDB.
- **No Secrets in Code:** We do not store secrets in the repository.

## Hardening Checklist

- [x] **No Server-Side Code:** Eliminates a broad class of server-side
  vulnerabilities (e.g., RCE, SQLi).
- [ ] **Content Security Policy (CSP):** Future enhancement to restrict which
  scripts can run.
- [ ] **Sanitization:** Ensure that user-provided input is properly sanitized
  before being rendered or exported to prevent XSS.
- [x] **Zero Dependencies:** Minimizes the attack surface by avoiding
  third-party library vulnerabilities.

## Best Practices for Users

1. **Keep Browsers Updated:** Always use the latest version of your browser for
   the best security protections.
2. **Review Exports:** Before sharing an exported file, review the content to
   ensure it contains only the data you intend to share.
3. **Local Hosting:** If hosting this project, ensure you use HTTPS and set
   appropriate security headers.

## Contact & Keys

- **Security contact:** @maintainer
