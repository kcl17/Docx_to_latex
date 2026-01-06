# Contributing to Google Docs to Overleaf Converter

Thank you for your interest in contributing! This document provides guidelines for contributing to this project.

## 🎯 How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check existing issues. When creating a bug report, include:

- **Clear title** describing the issue
- **Steps to reproduce** the bug
- **Expected behavior** vs actual behavior
- **Screenshots** if applicable
- **Browser version** and operating system
- **Sample .docx file** (if possible and not sensitive)

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. Include:

- **Clear title** describing the enhancement
- **Detailed description** of the proposed functionality
- **Use case** explaining why this would be useful
- **Examples** of similar features elsewhere (if applicable)

### Pull Requests

1. **Fork the repository** and create your branch from `main`
2. **Make your changes** with clear, descriptive commits
3. **Test thoroughly** in multiple browsers
4. **Update documentation** if needed
5. **Submit a pull request** with a clear description

## 🔧 Development Setup

Since this is a pure HTML/JavaScript project, setup is minimal:

1. Clone your fork:
   ```bash
   git clone https://github.com/your-username/repo-name.git
   cd repo-name
   ```

2. Open `gdocs-to-overleaf.html` in your browser

3. Make changes and refresh to test

## 📝 Coding Standards

### HTML
- Use semantic HTML5 elements
- Maintain proper indentation (4 spaces)
- Include comments for complex sections

### CSS
- Follow BEM naming convention where possible
- Keep styles organized by section
- Use CSS variables for colors and spacing
- Ensure responsive design (mobile-first)

### JavaScript
- Use ES6+ features
- Write clear, descriptive function names
- Add comments for complex logic
- Handle errors gracefully
- Test in multiple browsers

## 🎨 Adding New Format Templates

To add a new LaTeX format (e.g., ACM, Springer):

1. Create a new generator function (e.g., `generateACM`)
2. Add the format card to HTML:
   ```html
   <div class="format-card" data-format="acm">
       <h4>📚 ACM Format</h4>
       <p>Description of the format</p>
   </div>
   ```
3. Add to the formats object in `generateLatexPackage`:
   ```javascript
   const formats = {
       dissertation: generateDissertation,
       ieee: generateIEEE,
       article: generateArticle,
       report: generateReport,
       acm: generateACM  // Your new format
   };
   ```
4. Test thoroughly with sample documents

## 🧪 Testing Checklist

Before submitting a PR, ensure:

- [ ] Code works in Chrome, Firefox, and Safari
- [ ] Mobile responsive design is maintained
- [ ] File upload/download works correctly
- [ ] All format templates compile in Overleaf
- [ ] Error messages are clear and helpful
- [ ] No console errors or warnings
- [ ] Documentation is updated

## 📋 Commit Message Guidelines

Use clear, descriptive commit messages:

- `feat: Add ACM format template`
- `fix: Correct bibliography generation bug`
- `docs: Update installation instructions`
- `style: Improve mobile responsive design`
- `refactor: Optimize document parsing`
- `test: Add format validation tests`

## 🚀 Release Process

1. Update version number
2. Update CHANGELOG.md
3. Test all features
4. Create release tag
5. Update documentation

## 📞 Questions?

- Open a discussion on GitHub
- Check existing issues and PRs
- Review the README.md

## 🙏 Recognition

Contributors will be recognized in:
- README.md acknowledgments
- Release notes
- Project documentation

Thank you for contributing! 🎉