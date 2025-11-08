# Contributing to Aethyrion

First off, **thank you** for considering contributing to Aethyrion! It's people like you who make free, quality developer tools possible.

## 🎯 Our Mission

Aethyrion exists to provide professional-grade developer tools that are:
- **100% free forever** - No paywalls, no freemium models
- **Open source** - MIT licensed for maximum freedom
- **Community-driven** - Built by developers, for developers
- **Quality-focused** - Matching or exceeding paid alternatives

Every contribution, no matter how small, helps achieve this mission.

---

## 🤝 Ways to Contribute

### 🐛 Report Bugs
Found a bug? [Open an issue](../../issues/new?template=bug_report.md) with:
- Clear, descriptive title
- Steps to reproduce
- Expected vs actual behavior  
- Screenshots/error messages if applicable
- Your environment (OS, version, etc.)

### 💡 Request Features
Have an idea? [Open an issue](../../issues/new?template=feature_request.md) with:
- Clear description of the feature
- Use case (why it's needed)
- How it aligns with project goals
- Any implementation ideas (optional)

### 📖 Improve Documentation
Documentation is crucial! You can:
- Fix typos or unclear wording
- Add examples or clarifications
- Write tutorials or guides
- Translate docs to other languages

### 🔧 Submit Code
Ready to code? Great! See the sections below.

---

## 🚀 Getting Started

### Prerequisites
```bash
# Check your Node.js version (18+ required)
node --version

# Check npm version
npm --version
```

### Fork & Clone
```bash
# Fork the repo on GitHub, then:
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
cd REPO-NAME

# Add upstream remote
git remote add upstream https://github.com/AethyrionAI/REPO-NAME.git
```

### Install Dependencies
```bash
npm install
```

### Run Development Build
```bash
npm run dev
```

---

## 📝 Development Guidelines

### Code Style
We use **ESLint** and **Prettier** for consistent code style:
```bash
# Run linting
npm run lint

# Auto-fix issues
npm run lint:fix

# Format code
npm run format
```

**Key conventions:**
- Use **TypeScript** for all new code
- Follow **functional components** (React hooks)
- Use **async/await** over promises
- Keep functions **small and focused**
- Write **descriptive variable names**
- Add **comments for complex logic**

### Commit Messages
Follow the [Conventional Commits](https://www.conventionalcommits.org/) standard:

```
<type>(<scope>): <description>

[optional body]

[optional footer]
```

**Types:**
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `style:` Code style changes (formatting, etc.)
- `refactor:` Code refactoring
- `test:` Adding or updating tests
- `chore:` Maintenance tasks

**Examples:**
```
feat(helix): add multi-image upload support
fix(prism): resolve GlideRecord query builder crash
docs: update installation instructions
style: format components with prettier
refactor(api): simplify error handling logic
test: add unit tests for component generator
chore: update dependencies to latest versions
```

### Branch Naming
```
<type>/<description>

Examples:
feat/multi-image-support
fix/query-builder-crash  
docs/installation-guide
refactor/api-error-handling
```

---

## 🔄 Pull Request Process

### 1. Create Your Branch
```bash
# Update your fork
git fetch upstream
git checkout main
git merge upstream/main

# Create feature branch
git checkout -b feat/your-feature-name
```

### 2. Make Your Changes
- Write clean, tested code
- Follow the style guidelines
- Update docs if needed
- Add/update tests

### 3. Test Everything
```bash
# Run all tests
npm test

# Run linting
npm run lint

# Build the project
npm run build
```

### 4. Commit Your Changes
```bash
git add .
git commit -m "feat: your descriptive commit message"
```

### 5. Push to Your Fork
```bash
git push origin feat/your-feature-name
```

### 6. Open a Pull Request
- Go to the original repo on GitHub
- Click "New Pull Request"
- Select your fork and branch
- Fill out the PR template completely
- Link any related issues

### PR Requirements Checklist
- [ ] Code follows style guidelines
- [ ] Self-review of code completed
- [ ] Comments added for complex logic
- [ ] Documentation updated (if needed)
- [ ] No new warnings generated
- [ ] Tests added/updated (if applicable)
- [ ] All tests passing
- [ ] PR title follows conventional commits
- [ ] Related issues linked

---

## 🧪 Testing

### Running Tests
```bash
# Run all tests
npm test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage
```

### Writing Tests
- Place tests next to the code they test
- Use descriptive test names
- Test edge cases and error conditions
- Aim for good coverage, but quality > quantity

**Example:**
```typescript
describe('ComponentGenerator', () => {
  it('should generate valid React component from text prompt', async () => {
    const result = await generateComponent('Create a button');
    expect(result).toContain('export default');
    expect(result).toContain('Button');
  });

  it('should handle errors gracefully', async () => {
    const result = await generateComponent('');
    expect(result).toBeNull();
  });
});
```

---

## 🎨 UI/UX Guidelines

### Design Principles
- **Dark theme first** - Match Aethyrion aesthetic
- **Clean & minimal** - Remove unnecessary elements
- **Responsive** - Work on all screen sizes
- **Accessible** - Follow WCAG 2.1 AA standards
- **Fast** - Optimize for performance

### Color Palette
```css
/* Primary Colors */
--primary-indigo: #6366f1;
--primary-purple: #8b5cf6;
--primary-blue: #3b82f6;
--primary-cyan: #06b6d4;

/* Background Colors */
--bg-dark: #0a0a0a;
--bg-slate: #0f172a;
--bg-slate-light: #1e293b;

/* Text Colors */
--text-primary: #ffffff;
--text-secondary: #94a3b8;
--text-muted: #64748b;

/* Accent Colors */
--success: #10b981;
--warning: #f59e0b;
--error: #ef4444;
```

### Components
- Use **Tailwind CSS** for styling
- Follow existing component patterns
- Ensure components are reusable
- Add proper TypeScript types

---

## 📋 Issue Guidelines

### Before Opening an Issue
1. Search existing issues (open and closed)
2. Check the documentation
3. Try the latest version
4. Gather all relevant information

### Issue Templates
Use the provided templates for:
- 🐛 Bug Reports
- 💡 Feature Requests  
- 📖 Documentation Improvements
- ❓ Questions

### Issue Etiquette
- Be respectful and constructive
- Provide all requested information
- Respond to questions promptly
- Close issues when resolved

---

## 🏆 Recognition

All contributors are recognized! Ways we say thank you:
- Name in CONTRIBUTORS.md
- Mention in release notes
- Special shoutouts for major contributions
- Eternal gratitude from the community ❤️

---

## 📜 Code of Conduct

This project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to uphold this code.

**In short:**
- Be respectful and inclusive
- Accept constructive criticism gracefully
- Focus on what's best for the community
- Show empathy towards others

---

## ❓ Questions?

- 💬 Join our [Discord](#)
- 📧 Email: contribute@aethyrion.org
- 💬 Open a [discussion](../../discussions)

---

## 🎉 Thank You!

Every contribution makes Aethyrion better. Whether you're fixing a typo or building a major feature, **you're making professional developer tools accessible to everyone**.

**We appreciate you!** 🙏

---

<div align="center">

**Built with ❤️ by the Aethyrion community**

[![Star on GitHub](https://img.shields.io/github/stars/AethyrionAI?style=social)](../../stargazers)
[![Follow on Twitter](https://img.shields.io/twitter/follow/aethyrionai?style=social)](https://twitter.com/aethyrionai)

</div>
