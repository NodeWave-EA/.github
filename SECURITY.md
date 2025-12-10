# Security Policy

## Supported Versions

We release security updates for the following versions:

| Version | Supported          |
| ------- | ------------------ |
| Latest  | :white_check_mark: |
| < Latest| :x:                |

We strongly recommend using the latest version to ensure you have all security updates.

## Reporting a Vulnerability

We take security vulnerabilities seriously. If you discover a security issue, please follow these guidelines:

### 🔒 Private Disclosure

**DO NOT** open a public issue for security vulnerabilities.

Instead, please report security vulnerabilities through one of these channels:

#### GitHub Security Advisories (Preferred)

1. Go to the repository's Security tab
2. Click "Report a vulnerability"
3. Fill out the advisory form with details

#### Email

Send details to: **security@nodewave.net**

#### PGP Encrypted Email

For sensitive disclosures, contact security@nodewave.net to request our PGP public key.

### What to Include

Please provide:

1. **Description**: Clear description of the vulnerability
2. **Impact**: What can be compromised and how severe
3. **Reproduction**: Step-by-step instructions to reproduce
4. **Affected Versions**: Which versions are affected
5. **Proof of Concept**: Code or commands demonstrating the issue
6. **Suggested Fix**: If you have ideas on how to fix it
7. **Credit**: How you'd like to be credited (optional)

### Example Report

```
Title: SQL Injection in User Search API

Description:
The user search endpoint is vulnerable to SQL injection through the
'username' parameter.

Impact:
Attackers can execute arbitrary SQL commands, potentially accessing
or modifying all database data.

Severity: Critical

Affected Versions: v1.0.0 - v1.5.2

Reproduction Steps:
1. Send POST request to /api/users/search
2. Include payload: {"username": "admin' OR '1'='1"}
3. Observe that all users are returned

Proof of Concept:
curl -X POST https://example.com/api/users/search \
  -H "Content-Type: application/json" \
  -d '{"username": "admin'\'' OR '\''1'\''='\''1"}'

Suggested Fix:
Use parameterized queries or an ORM to prevent SQL injection.
```

## Response Timeline

We aim to respond according to the following timeline:

| Stage | Timeline |
|-------|----------|
| **Initial Response** | Within 48 hours |
| **Triage & Validation** | Within 7 days |
| **Fix Development** | Depends on severity |
| **Fix Deployment** | Coordinated disclosure |
| **Public Disclosure** | After fix is deployed |

### Severity Levels

| Severity | Response Time | Example |
|----------|---------------|---------|
| **Critical** | Fix within 7 days | Remote code execution, data breach |
| **High** | Fix within 30 days | Authentication bypass, privilege escalation |
| **Medium** | Fix within 90 days | XSS, CSRF, information disclosure |
| **Low** | Fix as able | Minor information leaks |

## What Happens Next

1. **Acknowledgment**: We'll acknowledge receipt of your report
2. **Investigation**: We'll investigate and validate the issue
3. **Fix Development**: We'll develop and test a fix
4. **Coordination**: We'll coordinate disclosure timing with you
5. **Release**: We'll release the fix and security advisory
6. **Credit**: We'll credit you in the advisory (if desired)

## Disclosure Policy

We follow **coordinated disclosure**:

1. You report the vulnerability privately
2. We work on a fix
3. We release the fix
4. We publish a security advisory
5. Public disclosure happens after users can update

### Timeline for Disclosure

- We aim for disclosure within **90 days** of initial report
- Critical vulnerabilities may be disclosed sooner
- We'll coordinate with you on timing
- Emergency patches may be released without advance notice

## Security Best Practices

### For Contributors

- Never commit secrets (API keys, passwords, tokens)
- Use environment variables for sensitive configuration
- Keep dependencies up to date
- Follow secure coding practices
- Run security scanners before submitting PRs

### For Users

- Always use the latest version
- Keep dependencies updated
- Use strong authentication
- Enable two-factor authentication
- Follow principle of least privilege
- Monitor security advisories

## Security Features

### Built-in Security

Our projects include:

- ✅ Automated dependency scanning (Dependabot)
- ✅ CodeQL security analysis
- ✅ Secret scanning
- ✅ Container vulnerability scanning (Trivy)
- ✅ Regular security audits

### Security Hardening

Recommended security measures:

- Use HTTPS/TLS for all communications
- Implement rate limiting
- Use secure session management
- Validate and sanitize all inputs
- Implement proper access controls
- Log security events
- Regular security updates

## Security Updates

### Notification

Security updates are announced through:

- GitHub Security Advisories
- Repository releases
- Organization discussions
- Email notifications to info@nodewave.net subscribers

### Applying Updates

```bash
# Check for updates
npm audit

# Apply security fixes
npm audit fix

# For breaking changes
npm audit fix --force
```

## Bug Bounty Program

We currently do not have a formal bug bounty program, but we greatly appreciate responsible disclosure of security vulnerabilities. Security researchers who report valid vulnerabilities will be credited in our security advisories and receive our sincere gratitude.

## Hall of Fame

We recognize security researchers who have helped us:

- [List of credited researchers]

## Questions?

For security questions that aren't vulnerabilities:

- Open a [GitHub Discussion](../../discussions)
- Contact us at info@nodewave.net

For vulnerabilities, always use the private reporting channels above.

## Additional Resources

- [OWASP Top 10](https://owasp.org/www-project-top-ten/)
- [CWE Top 25](https://cwe.mitre.org/top25/)
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework)

---

Thank you for helping keep our organization and community safe! 🔒
