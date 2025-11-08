# Security Policy

## 🔒 Our Commitment

At Aethyrion, we take security seriously. Our tools handle your code, configurations, and API keys - we understand the responsibility that comes with that trust.

Since all Aethyrion tools run **locally on your machine** with no cloud dependencies, your data never leaves your control. However, we still want to ensure the software itself is secure and free from vulnerabilities.

---

## 🐛 Reporting a Vulnerability

If you discover a security vulnerability in any Aethyrion tool, please report it responsibly.

### How to Report

**Email:** security@aethyrion.org

**Include:**
- Tool name and version
- Description of the vulnerability
- Steps to reproduce
- Potential impact
- Any suggested fixes (optional)

### Response Timeline

- **Initial Response:** Within 48 hours
- **Status Update:** Within 7 days
- **Fix Timeline:** Depends on severity
  - Critical: 1-3 days
  - High: 1-2 weeks
  - Medium: 2-4 weeks
  - Low: Next release cycle

---

## 🎯 Supported Versions

We actively maintain the latest major version of each tool. Security patches are backported to the previous major version when feasible.

| Tool | Version | Supported |
|------|---------|-----------|
| Helix | v1.x | ✅ Yes |
| Prism | v0.x (Beta) | ✅ Yes |
| Observatory | Not released | N/A |
| Conduit | Not released | N/A |
| Spectra | Not released | N/A |

**End of Life:** We'll provide at least 6 months notice before ending support for any major version.

---

## 🔐 Security Best Practices

### API Key Storage
All Aethyrion tools use:
- **AES-GCM encryption** for stored API keys
- **System keychain integration** (macOS, Windows, Linux)
- **Never logged or transmitted** to external services

### Data Privacy
- **Local-first architecture** - Your data stays on your machine
- **No telemetry or analytics** by default
- **No cloud dependencies** for core functionality
- **Open source** - Audit the code yourself

### Safe Updates
- **Digital signatures** on all releases
- **Checksums** for verification
- **GitHub Releases** as sole distribution channel
- **No auto-update without permission**

---

## ⚠️ Known Security Considerations

### AI Provider API Keys
When using external AI providers (OpenAI, Anthropic, etc.):
- Keys are stored encrypted locally
- You control which providers to use
- Consider using local AI (Ollama) for maximum privacy

### Electron Security
Our Electron apps follow security best practices:
- Context isolation enabled
- Node integration disabled in renderers
- Content Security Policy (CSP) enforced
- IPC communication validated

### Third-Party Dependencies
We regularly:
- Audit dependencies with `npm audit`
- Update to patched versions
- Remove unnecessary dependencies
- Pin versions for reproducibility

---

## 🛡️ Security Features by Tool

### Helix
- Encrypted API key storage
- No code execution of generated components
- Sandboxed preview environment
- CSP headers in preview

### Prism
- ServiceNow credential encryption
- No credential transmission to AI providers
- Local validation of generated code
- Secure template rendering

### Observatory (Planned)
- Authentication & authorization
- TLS/HTTPS enforced
- Role-based access control (RBAC)
- Audit logging

### Conduit (Planned)
- Encrypted environment variables
- Secure mock server
- Request signing
- Credential rotation support

### Spectra (Planned)
- 100% local code analysis
- No data transmission
- Secure git integration
- Sandboxed analysis environment

---

## 🔍 Security Audits

We welcome security audits and penetration testing:

**Guidelines:**
- Test against your own installations
- Don't test against shared infrastructure
- Report findings responsibly
- Give us reasonable time to fix issues

**Recognition:**
- Credit in release notes (if desired)
- Listed in SECURITY.md hall of fame
- Our eternal gratitude 🙏

---

## 📜 Disclosure Policy

### Our Commitments
- Acknowledge receipt within 48 hours
- Provide regular updates on fix progress
- Credit reporters in release notes (unless anonymous)
- No legal action against good-faith researchers

### Your Commitments
- Give us reasonable time to fix (90 days recommended)
- Don't publicly disclose before fix is released
- Don't exploit vulnerabilities for harm
- Act in good faith

---

## 🏆 Security Hall of Fame

Thank you to security researchers who've helped make Aethyrion safer:

<!-- 
Format:
- **[Researcher Name](link)** - [Brief description of finding] - [Date]
-->

*No vulnerabilities reported yet - be the first!*

---

## 🔗 Security Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [Electron Security Guidelines](https://www.electronjs.org/docs/latest/tutorial/security)
- [Node.js Security Best Practices](https://nodejs.org/en/docs/guides/security/)
- [NIST Vulnerability Database](https://nvd.nist.gov/)

---

## 📞 Contact

- **Security Issues:** security@aethyrion.org
- **General Questions:** support@aethyrion.org
- **Discord:** [Join our community](https://discord.gg/UZPWT8PxDe)

---

<div align="center">

**Security is a shared responsibility**

*We build secure tools. You use them securely. Together, we keep everyone safe.*

**Report vulnerabilities responsibly** • **Keep your tools updated** • **Follow best practices**

</div>
