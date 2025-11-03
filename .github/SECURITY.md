# Security Policy

## 🔒 Supported Versions

We release patches for security vulnerabilities in the following versions:

| Version | Supported          |
| ------- | ------------------ |
| 0.1.x   | :white_check_mark: |
| < 0.1   | :x:                |

## 🛡️ Reporting a Vulnerability

We take the security of Automate seriously. If you believe you have found a security vulnerability, please report it to us responsibly.

### How to Report

**Please DO NOT report security vulnerabilities through public GitHub issues.**

Instead, please report them via email to: **[YOUR-SECURITY-EMAIL@example.com]**

Include the following information:

- Type of vulnerability
- Full paths of source file(s) related to the vulnerability
- Location of the affected source code (tag/branch/commit or direct URL)
- Step-by-step instructions to reproduce the issue
- Proof-of-concept or exploit code (if possible)
- Impact of the vulnerability
- Possible fixes (if any)

### What to Expect

- **Acknowledgment**: We will acknowledge receipt of your vulnerability report within 48 hours
- **Investigation**: We will investigate and validate the vulnerability
- **Timeline**: We aim to provide a fix within 30 days for critical vulnerabilities
- **Credit**: We will credit you in our security advisory (unless you prefer to remain anonymous)
- **Disclosure**: We follow coordinated disclosure - please allow us time to fix the issue before public disclosure

## 🔐 Security Best Practices

When using Automate:

### For Users

1. **API Keys**: Never share your API keys publicly
2. **Permissions**: Only grant necessary browser permissions
3. **Updates**: Keep Automate updated to the latest version
4. **Source**: Only install Automate from official sources (Chrome Web Store or our GitHub releases)
5. **Profile**: Consider using a separate Chrome profile for sensitive automation tasks

### For Developers

1. **Dependencies**: Regularly update dependencies to patch vulnerabilities
2. **Code Review**: All code changes go through review before merging
3. **Static Analysis**: Use ESLint and TypeScript strict mode
4. **Secrets**: Never commit API keys, tokens, or sensitive data
5. **CSP**: Respect Content Security Policy restrictions

## 🚨 Known Security Considerations

### API Key Storage

- API keys are stored locally in Chrome's storage API
- Keys are encrypted by Chrome's built-in security
- Keys never leave your browser

### LLM Provider Connections

- Direct connections to LLM provider APIs
- No data is sent through our servers
- All prompts and responses stay between you and your chosen provider

### Chrome Debugger Protocol

- Automate uses the Chrome Debugger Protocol for DOM access
- This requires explicit user permission
- Only one debugger can attach at a time (prevents conflicts)

### Content Script Injection

- Content scripts have limited privileges
- Cannot access your API keys or storage
- Follow Chrome's extension security model

## 📋 Security Checklist for Contributors

- [ ] No hardcoded secrets or API keys
- [ ] Input validation for all user inputs
- [ ] Proper error handling (no sensitive data in error messages)
- [ ] Dependencies are up to date
- [ ] Code follows security best practices
- [ ] Tests include security scenarios
- [ ] Documentation updated if security model changes

## 🔗 Related Security Resources

- [Chrome Extension Security](https://developer.chrome.com/docs/extensions/mv3/security/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CWE Top 25](https://cwe.mitre.org/top25/)

## 📞 Contact

For security concerns, contact: **[YOUR-SECURITY-EMAIL@example.com]**

For general issues: [GitHub Issues](https://github.com/yourusername/automate/issues)

---

**Note**: This security policy is subject to change. Please check back regularly for updates.
