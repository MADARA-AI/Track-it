# Contributing to TrackIt

First off, thank you for considering contributing to TrackIt! It's people like you that make TrackIt such a great platform.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Development Setup](#development-setup)
- [Coding Standards](#coding-standards)
- [Commit Guidelines](#commit-guidelines)
- [Pull Request Process](#pull-request-process)

## Code of Conduct

This project and everyone participating in it is governed by a code of conduct. By participating, you are expected to uphold this code. Please be respectful, inclusive, and professional.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the existing issues to avoid duplicates. When creating a bug report, include:

- **Clear title**: Summarize the issue in one line
- **Description**: Detailed explanation of the issue
- **Steps to reproduce**: List the exact steps to reproduce the behavior
- **Expected behavior**: What you expected to happen
- **Actual behavior**: What actually happened
- **Screenshots**: If applicable
- **Environment**: OS, Node version, browser, etc.

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion:

- **Use a clear and descriptive title**
- **Provide a detailed description** of the suggested enhancement
- **Explain why this enhancement would be useful**
- **List any similar features** in other platforms if applicable

### Pull Requests

1. Fork the repository
2. Create a new branch from `main`: `git checkout -b feature/your-feature-name`
3. Make your changes
4. Write or update tests as needed
5. Update documentation as needed
6. Commit your changes following the commit guidelines
7. Push to your fork
8. Open a Pull Request

## Development Setup

### Prerequisites

- Node.js v18 or higher
- MongoDB (Atlas or local)
- Git

### Setup Instructions

```bash
# Clone your fork
git clone https://github.com/your-username/web-backend-bridge.git
cd web-backend-bridge

# Install dependencies
npm install

# Setup backend
cd server
npm install
cp .env.example .env  # Configure your environment variables

# Start backend
npm start

# In a new terminal, start frontend
cd ..
npm run dev
```

## Coding Standards

### JavaScript/TypeScript

- Use ES6+ features
- Follow the existing code style
- Use meaningful variable and function names
- Add comments for complex logic
- Keep functions small and focused

### React Components

- Use functional components with hooks
- Keep components small and reusable
- Use PropTypes or TypeScript for type checking
- Follow the single responsibility principle

### File Naming

- React components: `PascalCase.tsx` (e.g., `UserProfile.tsx`)
- Utilities: `camelCase.ts` (e.g., `formatDate.ts`)
- Styles: `kebab-case.css` (e.g., `user-profile.css`)

### Code Style

This project uses ESLint for code style enforcement. Run before committing:

```bash
npm run lint
```

To automatically fix issues:

```bash
npm run lint -- --fix
```

## Commit Guidelines

We follow [Conventional Commits](https://www.conventionalcommits.org/) specification:

### Commit Message Format

```
<type>(<scope>): <subject>

<body>

<footer>
```

### Types

- `feat`: A new feature
- `fix`: A bug fix
- `docs`: Documentation only changes
- `style`: Changes that don't affect code meaning (formatting, missing semi-colons, etc.)
- `refactor`: Code change that neither fixes a bug nor adds a feature
- `perf`: Code change that improves performance
- `test`: Adding missing tests or correcting existing tests
- `chore`: Changes to the build process or auxiliary tools

### Examples

```bash
feat(auth): add password reset functionality

fix(api): resolve null pointer exception in user routes

docs(readme): update installation instructions

style(components): format code with prettier

refactor(utils): simplify date formatting logic

test(auth): add unit tests for login endpoint

chore(deps): update react to v18.3.1
```

### Scope

The scope should be the name of the affected component or area:
- `auth` - Authentication related
- `api` - API endpoints
- `ui` - UI components
- `db` - Database related
- `docs` - Documentation
- `deps` - Dependencies

## Pull Request Process

1. **Update Documentation**: Ensure README and other docs are updated
2. **Update Tests**: Add or update tests for your changes
3. **Run Tests**: Ensure all tests pass
4. **Run Linter**: Ensure code passes linting
5. **Update Changelog**: Add your changes to CHANGELOG.md if applicable
6. **Review Your Changes**: Double-check your diff before submitting
7. **Fill PR Template**: Complete all sections of the PR template
8. **Link Issues**: Reference related issues using keywords (fixes #123)

### PR Title Format

Follow the same format as commit messages:

```
feat(auth): add OAuth2 integration
fix(ui): resolve responsive layout issues
docs(api): add endpoint documentation
```

### PR Description Template

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Breaking change
- [ ] Documentation update

## Testing
How has this been tested?

## Checklist
- [ ] My code follows the project's style guidelines
- [ ] I have performed a self-review of my code
- [ ] I have commented my code where necessary
- [ ] I have updated the documentation
- [ ] My changes generate no new warnings
- [ ] I have added tests that prove my fix/feature works
- [ ] New and existing unit tests pass locally
```

## Code Review Process

- All PRs require at least one review before merging
- Address all review comments
- Keep PR scope focused and small
- Be respectful and constructive in reviews

## Questions?

Feel free to:
- Open an issue for questions
- Start a discussion in GitHub Discussions
- Reach out to the maintainers

## Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes
- GitHub contributors page

Thank you for contributing to TrackIt! 🎉
