# Contributing to Portfolio Website

Thank you for your interest in contributing to this portfolio website! We welcome contributions from the community.

## 📋 Table of Contents

- [Getting Started](#getting-started)
- [Development Setup](#development-setup)
- [Contributing Guidelines](#contributing-guidelines)
- [Code Style](#code-style)
- [Pull Request Process](#pull-request-process)
- [Issue Reporting](#issue-reporting)

## 🚀 Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally:
   ```bash
   git clone https://github.com/asma019/Next.js-Portfolio-for-System-Admins.git
cd Next.js-Portfolio-for-System-Admins
   ```
3. **Install dependencies**:
   ```bash
   npm install
   ```
4. **Set up environment variables**:
   ```bash
   cp .env.example .env.local
   ```
5. **Start development server**:
   ```bash
   npm run dev
   ```

## 🛠️ Development Setup

### Prerequisites
- Node.js 18+ 
- npm or yarn package manager
- Git

### Environment Variables
The project uses environment variables for configuration. Copy `.env.example` to `.env.local` and fill in the required values:

```env
# SMTP Configuration for AWS SES
SMTP_HOST=email-smtp.ap-southeast-1.amazonaws.com
SMTP_USERNAME=your-aws-ses-username
SMTP_PASSWORD=your-aws-ses-password
SMTP_PORT=587
SMTP_SECURE=false

# Email Configuration
FROM_EMAIL_NAME=Your Name Contact
FROM_EMAIL=no-reply@yourdomain.com
TO_EMAIL=your-email@gmail.com

# Application Configuration
NEXT_PUBLIC_SITE_URL=https://yourdomain.com
```

### Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run start        # Start production server
npm run lint         # Run ESLint
npm run lint:fix     # Fix ESLint issues
```

## 🤝 Contributing Guidelines

### Types of Contributions

We welcome these types of contributions:

- 🐛 **Bug fixes**
- ✨ **New features**
- 📚 **Documentation improvements**
- 🎨 **UI/UX enhancements**
- 🔧 **Performance optimizations**
- 🧪 **Tests**

### Before You Start

1. **Check existing issues** to avoid duplicates
2. **Create an issue** to discuss major changes
3. **Keep pull requests focused** on a single feature/fix
4. **Test your changes** thoroughly

## 📝 Code Style

### TypeScript/JavaScript
- Use TypeScript for new files
- Follow ESLint configuration
- Use meaningful variable names
- Add comments for complex logic

### React Components
- Use functional components with hooks
- Keep components small and focused
- Use proper prop types
- Follow React best practices

### Styling
- Use Tailwind CSS classes
- Keep custom CSS minimal
- Use responsive design principles
- Follow the existing design system

### File Structure
```
src/
├── app/
│   ├── api/              # API routes
│   ├── globals.css       # Global styles
│   ├── layout.tsx        # Root layout
│   └── page.tsx          # Home page
├── components/
│   ├── Header.tsx        # Navigation
│   └── Footer.tsx        # Footer
└── lib/                  # Utility functions
```

## 🔄 Pull Request Process

1. **Create a feature branch**:
   ```bash
   git checkout -b feature/amazing-feature
   ```

2. **Make your changes**:
   - Write clear, focused code
   - Add tests if applicable
   - Update documentation

3. **Test your changes**:
   ```bash
   npm run build
   npm run lint
   ```

4. **Commit your changes**:
   ```bash
   git commit -m "Add amazing feature"
   ```
   
   Use clear commit messages:
   - `feat: add new feature`
   - `fix: resolve bug`
   - `docs: update documentation`
   - `style: improve styling`
   - `refactor: improve code structure`

5. **Push to your fork**:
   ```bash
   git push origin feature/amazing-feature
   ```

6. **Open a Pull Request**:
   - Use a descriptive title
   - Explain what you changed and why
   - Reference related issues
   - Add screenshots for UI changes

### Pull Request Template

```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Performance improvement
- [ ] Other (please describe)

## Testing
- [ ] Tested locally
- [ ] Added tests
- [ ] Updated documentation

## Screenshots
(If applicable)
```

## 🐛 Issue Reporting

### Bug Reports
Include:
- Clear description of the issue
- Steps to reproduce
- Expected vs actual behavior
- Browser/OS information
- Screenshots if applicable

### Feature Requests
Include:
- Clear description of the feature
- Use case/motivation
- Possible implementation ideas
- Examples from other sites

### Issue Templates

**Bug Report:**
```markdown
**Bug Description**
A clear description of the bug

**To Reproduce**
Steps to reproduce the behavior:
1. Go to '...'
2. Click on '....'
3. Scroll down to '....'
4. See error

**Expected Behavior**
What you expected to happen

**Screenshots**
If applicable, add screenshots

**Environment**
- Browser: [e.g. Chrome, Firefox]
- OS: [e.g. Windows, macOS, Linux]
- Version: [e.g. 1.0.0]
```

## 📜 Code of Conduct

### Our Pledge
We pledge to make participation in our project a harassment-free experience for everyone, regardless of age, body size, disability, ethnicity, gender identity and expression, level of experience, nationality, personal appearance, race, religion, or sexual identity and orientation.

### Our Standards
Examples of behavior that contributes to creating a positive environment include:
- Using welcoming and inclusive language
- Being respectful of differing viewpoints and experiences
- Gracefully accepting constructive criticism
- Focusing on what is best for the community

## 🙏 Recognition

Contributors will be recognized in:
- GitHub contributors list
- README acknowledgments
- Release notes (for significant contributions)

## 📞 Questions?

If you have questions about contributing:
- Create an issue with the `question` label
- Join our discussions on GitHub
- Contact the maintainers

---

Thank you for contributing to make this portfolio website better! 🎉 