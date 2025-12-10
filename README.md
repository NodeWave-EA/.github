# .github - Organization Default Community Health Files

Welcome to the organization-level `.github` repository! This repository provides **default community health files, templates, workflows, and policies** that automatically apply to all repositories in the organization that don't have their own versions of these files.

## 📋 What This Repository Contains

This repository establishes organization-wide standards for:

- 📝 Issue and Pull Request templates
- 🔄 Automated workflows (CI/CD, security, maintenance)
- 📖 Community health files (Code of Conduct, Contributing Guidelines, etc.)
- 🛡️ Security policies and reporting procedures
- 👥 Code ownership and review assignments
- 💰 Funding and sponsorship information

## 🗂️ Repository Structure

```
.github/
├── ISSUE_TEMPLATE/              # GitHub Issue Form templates
│   ├── bug_report.yml          # Bug report template
│   ├── feature_request.yml     # Feature request template
│   ├── improvement.yml         # Improvement suggestion template
│   └── config.yml              # Issue template configuration
│
├── workflows/                   # Reusable GitHub Actions workflows
│   ├── org-ci.yml              # Organization-wide CI (lint, test, build)
│   ├── org-codeql.yml          # CodeQL security analysis
│   ├── auto-assign.yml         # Auto-assign reviewers from CODEOWNERS
│   ├── auto-label.yml          # Auto-label PRs and issues
│   ├── stale.yml               # Close stale issues/PRs
│   └── security-scan.yml       # Security vulnerability scanning
│
├── dependabot.yml               # Automated dependency updates
├── PULL_REQUEST_TEMPLATE.md    # Default PR template
├── CODE_OF_CONDUCT.md          # Contributor Covenant Code of Conduct
├── CONTRIBUTING.md             # Contribution guidelines
├── SECURITY.md                 # Security policy and vulnerability reporting
├── SUPPORT.md                  # Support and help resources
├── CODEOWNERS                  # Default code ownership rules
├── FUNDING.yml                 # Sponsorship and funding information
├── copilot-instructions.md     # AI coding assistant guidelines
└── README.md                   # This file
```

## 🚀 How It Works

GitHub automatically uses these files as defaults for any repository in the organization that doesn't have its own versions. This means:

* ✅ **New repositories** automatically inherit these templates and policies
* ✅ **Existing repositories** can reference these as organization defaults
* ✅ **Individual repositories** can override by creating their own versions
* ✅ **Consistency** across all organization projects

## 📝 Issue Templates

We provide three form-based issue templates:

- **Bug Report** ([bug_report.yml](ISSUE_TEMPLATE/bug_report.yml)): Structured bug reporting with severity levels
- **Feature Request** ([feature_request.yml](ISSUE_TEMPLATE/feature_request.yml)): New feature suggestions with use cases
- **Improvement** ([improvement.yml](ISSUE_TEMPLATE/improvement.yml)): Enhancements to existing functionality

All templates use GitHub Issue Forms (YAML) for structured data collection.

## 🔄 Automated Workflows

### CI/CD Workflows

- **[org-ci.yml](workflows/org-ci.yml)**: Lint, test, and build pipeline
- **[org-codeql.yml](workflows/org-codeql.yml)**: Automated security code scanning

### Automation Workflows

- **[auto-assign.yml](workflows/auto-assign.yml)**: Auto-assign reviewers based on CODEOWNERS
- **[auto-label.yml](workflows/auto-label.yml)**: Auto-label PRs by file paths and keywords
- **[stale.yml](workflows/stale.yml)**: Close inactive issues (60 days) and PRs (30 days)

### Security Workflows

- **[security-scan.yml](workflows/security-scan.yml)**:
  - Dependency review for PRs
  - NPM security audits
  - Trivy vulnerability scanning
  - Secret scanning with TruffleHog

### Dependency Management

- **[dependabot.yml](dependabot.yml)**: Weekly automated updates for npm, GitHub Actions, Docker, and Python dependencies

## 📖 Community Health Files

### [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md)
Based on Contributor Covenant 2.1, establishing expected behavior and enforcement guidelines.

### [CONTRIBUTING.md](CONTRIBUTING.md)
Comprehensive contribution guidelines including:
- Development workflow
- Branch strategy (`feature/*`, `fix/*`, `docs/*`)
- Commit message format (Conventional Commits)
- Pull request process
- Code review guidelines
- Testing requirements

### [SECURITY.md](SECURITY.md)
Security policy covering:
- Vulnerability reporting procedures
- Response timelines by severity
- Coordinated disclosure process
- Security best practices

### [SUPPORT.md](SUPPORT.md)
Support resources including:
- Documentation links
- Issue reporting guidelines
- Community channels
- Contact information
- Response time expectations

## 👥 Code Ownership

**[CODEOWNERS](CODEOWNERS)**: Template for defining team ownership of code areas. Individual repositories should customize this based on their structure.

## 💰 Funding

**[FUNDING.yml](FUNDING.yml)**: Configure organization sponsorship options (GitHub Sponsors, Ko-fi, Patreon, etc.)

## 🤖 AI Assistant Guidelines

**[copilot-instructions.md](copilot-instructions.md)**: Guidelines for AI coding assistants (GitHub Copilot, etc.) working in organization repositories.

## 🛠️ Customization

### For Individual Repositories

Repositories can override these defaults by creating their own versions:

1. Copy any file from this repository to your repository
2. Modify as needed
3. Your version takes precedence over the organization default

### For Organization Maintainers

To update organization defaults:

1. Create a branch with your changes
2. Submit a pull request
3. Get approval from maintainers
4. Merge to main branch

Changes immediately apply to all repositories using the defaults.

## 📚 Additional Resources

- [GitHub Community Health Files Documentation](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [Organization Profile Customization](https://docs.github.com/en/organizations/collaborating-with-groups-in-organizations/customizing-your-organizations-profile)
- [GitHub Actions Workflow Syntax](https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions)
- [Conventional Commits Specification](https://www.conventionalcommits.org/)

## 🤝 Contributing

Want to improve our organization defaults? Please:

1. Read [CONTRIBUTING.md](CONTRIBUTING.md)
2. Open an issue to discuss proposed changes
3. Submit a pull request with your improvements

## 📞 Contact

- **Issues**: [Open an issue](../../issues/new/choose)
- **Discussions**: [Join the conversation](../../discussions)
- **Security**: Follow [SECURITY.md](SECURITY.md) for vulnerability reports

## 📄 License

Please refer to individual repository LICENSE files for licensing information.

---

**Note**: This is a special repository. Files here serve as defaults for all organization repositories. Changes here have wide-reaching impact
