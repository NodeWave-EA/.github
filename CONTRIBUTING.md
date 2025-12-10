# Contributing Guidelines

Thank you for considering contributing to our organization! This document outlines the process and guidelines for contributing to any repository in our organization.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [Getting Started](#getting-started)
- [Development Workflow](#development-workflow)
- [Branch Strategy](#branch-strategy)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)
- [Code Review Guidelines](#code-review-guidelines)
- [Testing Requirements](#testing-requirements)
- [Documentation](#documentation)
- [Community](#community)

## Code of Conduct

This project and everyone participating in it is governed by our [Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code. Please report unacceptable behavior to info@nodewave.net.

## Getting Started

1. **Fork the repository** you want to contribute to
2. **Clone your fork** locally
3. **Set up the development environment** following the repository's README
4. **Create a new branch** for your work
5. **Make your changes** and test thoroughly
6. **Submit a pull request** to the main repository

## Development Workflow

### Prerequisites

Before you begin, ensure you have:
- Git installed and configured
- Required development tools (Node.js, Python, Docker, etc. - check repository README)
- An IDE or text editor of your choice
- Access to the repository and its dependencies

### Setting Up Your Local Environment

```bash
# Clone your fork
git clone https://github.com/YOUR_USERNAME/REPOSITORY_NAME.git
cd REPOSITORY_NAME

# Add upstream remote
git remote add upstream https://github.com/NodeWave/REPOSITORY_NAME.git

# Install dependencies
npm install  # or yarn install, pip install -r requirements.txt, etc.

# Run tests to ensure everything works
npm test
```

## Branch Strategy

We use a feature branch workflow:

### Branch Naming Convention

- **Feature branches**: `feature/short-description` or `feat/issue-123`
- **Bug fixes**: `fix/short-description` or `fix/issue-123`
- **Documentation**: `docs/short-description`
- **Refactoring**: `refactor/short-description`
- **Performance**: `perf/short-description`
- **Tests**: `test/short-description`

### Branch Lifecycle

1. Create branch from `main` (or `develop` if available)
2. Make your changes in small, logical commits
3. Keep your branch up to date with the base branch
4. Submit pull request when ready
5. Address review feedback
6. Branch is merged and deleted after approval

### Keeping Your Branch Updated

```bash
# Fetch latest changes
git fetch upstream

# Rebase your branch on latest main
git rebase upstream/main

# Force push to your fork (if needed)
git push --force-with-lease origin your-branch-name
```

## Commit Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification.

### Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- **feat**: A new feature
- **fix**: A bug fix
- **docs**: Documentation only changes
- **style**: Changes that don't affect code meaning (formatting, white-space)
- **refactor**: Code change that neither fixes a bug nor adds a feature
- **perf**: Performance improvement
- **test**: Adding or updating tests
- **build**: Changes to build system or dependencies
- **ci**: Changes to CI configuration files and scripts
- **chore**: Other changes that don't modify src or test files

### Examples

```bash
feat(auth): add OAuth2 authentication

fix(api): resolve race condition in user creation

docs(readme): update installation instructions

refactor(utils): simplify date formatting logic

test(auth): add integration tests for login flow
```

### Rules

- Use present tense ("add feature" not "added feature")
- Use imperative mood ("move cursor to..." not "moves cursor to...")
- Limit first line to 72 characters
- Reference issues and pull requests in the footer
- Provide context in the body for complex changes

## Pull Request Process

### Before Submitting

- [ ] Ensure all tests pass locally
- [ ] Add tests for new functionality
- [ ] Update documentation as needed
- [ ] Follow the code style of the project
- [ ] Rebase on the latest main branch
- [ ] Keep changes focused and atomic

### PR Title

Follow the same format as commit messages:

```
feat(component): add new functionality
fix(api): resolve issue with endpoints
```

### PR Description

Use the pull request template and include:

1. **Summary**: Brief description of changes
2. **Related Issues**: Link to issues this PR addresses
3. **Type of Change**: What kind of change this is
4. **Testing**: How you tested the changes
5. **Screenshots**: For UI changes
6. **Breaking Changes**: Any breaking changes and migration steps

### PR Size Guidelines

Keep pull requests small and focused:

- **Small (< 100 lines)**: Ideal size, easy to review
- **Medium (100-500 lines)**: Acceptable if focused
- **Large (> 500 lines)**: Consider splitting into smaller PRs

### Review Process

1. Automated checks run (CI, linting, tests)
2. Reviewers are automatically assigned
3. Address reviewer feedback
4. Maintainer approves and merges
5. Branch is automatically deleted

## Code Review Guidelines

### For Authors

- Be open to feedback
- Respond to all comments
- Ask questions if feedback is unclear
- Make requested changes promptly
- Keep discussions professional and respectful

### For Reviewers

- Review within 2 business days
- Be constructive and respectful
- Explain reasoning behind suggestions
- Approve when ready, request changes if needed
- Focus on:
  - Correctness
  - Security
  - Performance
  - Maintainability
  - Test coverage
  - Documentation

### Review Checklist

- [ ] Code follows project conventions
- [ ] Logic is sound and efficient
- [ ] Tests are adequate and pass
- [ ] Documentation is updated
- [ ] No security vulnerabilities introduced
- [ ] Backward compatibility maintained
- [ ] Error handling is appropriate

## Testing Requirements

### Required Tests

All code contributions must include appropriate tests:

- **Unit Tests**: Test individual functions/classes
- **Integration Tests**: Test component interactions
- **E2E Tests**: Test complete user flows (for UI changes)

### Test Coverage

- Aim for **80%+ code coverage**
- Critical paths must have **100% coverage**
- All bug fixes must include regression tests

### Running Tests

```bash
# Run all tests
npm test

# Run tests in watch mode
npm test -- --watch

# Run tests with coverage
npm test -- --coverage

# Run specific test file
npm test path/to/test.spec.ts
```

## Documentation

### When to Update Documentation

Update documentation when you:

- Add new features
- Change existing functionality
- Add or modify APIs
- Update configuration options
- Change build or deployment processes

### Documentation Types

1. **Code Comments**: Explain complex logic
2. **JSDoc/Docstrings**: Document functions, classes, and modules
3. **README**: Update setup and usage instructions
4. **API Documentation**: Document endpoints and schemas
5. **Architecture Docs**: For significant architectural changes

### Documentation Standards

- Write clear, concise explanations
- Include code examples
- Keep documentation up to date
- Use proper grammar and spelling
- Format with Markdown

## Community

### Communication Channels

- **GitHub Issues**: Bug reports and feature requests
- **GitHub Discussions**: Questions and general discussion
- **Pull Requests**: Code review and technical discussion

### Getting Help

- Check existing documentation
- Search closed issues
- Ask in GitHub Discussions
- Reference our [Support Guide](SUPPORT.md)

### Recognition

We value all contributions! Contributors are:

- Listed in commit history
- Mentioned in release notes
- Eligible for contributor recognition programs

## Questions?

If you have questions about contributing, please:

1. Check this guide and other documentation
2. Search existing issues and discussions
3. Ask in GitHub Discussions
4. Contact maintainers via info@nodewave.net

Thank you for contributing! 🎉
