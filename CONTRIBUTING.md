# 🤝 Contributing to Black Diamond Store

Thank you for your interest in contributing to Black Diamond Store! We're excited to work with you. This document provides guidelines and instructions for contributing.

## Code of Conduct

We are committed to providing a welcoming and harassment-free experience for everyone. Please:
- Be respectful and inclusive
- Welcome newcomers and help them get started
- Focus on constructive feedback
- Report inappropriate behavior to the project maintainers

## How to Contribute

### 1️⃣ Reporting Bugs

**Before submitting a bug report:**
- Check existing issues to avoid duplicates
- Be specific and descriptive

**Include in your bug report:**
```
Title: [BUG] Brief description of the issue

Description:
- What is the current behavior?
- What is the expected behavior?
- Steps to reproduce the issue
- Screenshots or error logs (if applicable)

Environment:
- Browser: (e.g., Chrome 120, Firefox 121)
- OS: (e.g., Windows 11, macOS 14)
- Device: (Desktop/Tablet/Mobile)
```

### 2️⃣ Suggesting Features

**Before requesting a feature:**
- Check existing issues and discussions
- Is it aligned with the project scope?

**Include in your feature request:**
```
Title: [FEATURE] Brief description of the feature

Use Case:
- What problem does this solve?
- Why is this important?

Proposed Solution:
- How should this feature work?
- Sketches or mockups (if applicable)

Alternatives:
- Are there other ways to achieve this?
```

### 3️⃣ Submitting Pull Requests

#### Prerequisites:
- Fork the repository
- Clone your fork locally
- Create a new branch for your changes

#### Branch Naming Convention:
```
feature/short-description       # New features
bugfix/short-description        # Bug fixes
docs/short-description          # Documentation
style/short-description         # Code style improvements
refactor/short-description      # Code refactoring
```

#### Before You Commit:
1. **Update your code** to follow our coding standards (see below)
2. **Test thoroughly:**
   - Test on different browsers (Chrome, Firefox, Safari, Edge)
   - Test on different screen sizes (desktop, tablet, mobile)
   - Test interactive features
3. **Keep commits atomic:**
   - One logical change per commit
   - Clear, descriptive commit messages

#### Commit Message Format:
```
[TYPE] Short description (50 chars max)

Detailed explanation of what changed and why (wrap at 72 chars).
Reference issues with "Fixes #123" or "Related to #456".

Example:
[FEATURE] Add product filtering by category
Implements category dropdown on products page. Users can now
filter jewelry by type (rings, necklaces, bracelets, etc.).

Fixes #42
```

#### Creating Your Pull Request:

1. Push your branch to your fork
2. Open a Pull Request against the `main` branch
3. Use this template:

```markdown
## Description
Brief description of your changes

## Type of Change
- [ ] Bug fix (non-breaking change fixing an issue)
- [ ] New feature (non-breaking change adding functionality)
- [ ] Breaking change (fix or feature causing existing functionality to change)
- [ ] Documentation update

## How Has This Been Tested?
Describe the tests you ran and how to reproduce them.

## Screenshots (if applicable)
Add images/GIFs of UI changes

## Checklist:
- [ ] My code follows the style guidelines
- [ ] I have performed a self-review of my own code
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] My changes generate no new warnings
- [ ] I have tested on multiple browsers
- [ ] I have tested on mobile devices
```

## Development Setup

### Local Development:

```bash
# Clone your fork
git clone https://github.com/YOUR-USERNAME/Black_diamond_store.git
cd Black_diamond_store

# Create a feature branch
git checkout -b feature/your-feature-name

# Make your changes, then test locally
# Option 1: Open index.html directly
# Option 2: Use a local server
python -m http.server 8000
# or
npx http-server
```

### File Structure Guidelines:

- **HTML:** Semantic markup, proper nesting, accessibility attributes
- **CSS:** Keep styles organized, use classes (not IDs), follow naming conventions
- **JavaScript:** Use modern ES6+, add comments for complex logic, avoid global variables

## Coding Standards

### HTML:
- Use semantic tags (`<header>`, `<nav>`, `<main>`, `<footer>`, etc.)
- Proper indentation (2 spaces)
- Include `alt` text for images
- Use descriptive `id` and `class` names

```html
<!-- Good -->
<header class="site-header">
  <nav class="main-navigation">
    <a href="/" class="logo">Black Diamond</a>
  </nav>
</header>

<!-- Avoid -->
<div id="header1">
  <div id="nav">
    <a href="/" id="l">BD</a>
  </div>
</div>
```

### CSS:
- Use BEM naming convention for classes
- Keep selectors simple and efficient
- Group related styles together
- Use variables for repeated values

```css
/* Good */
.product-card {
  padding: 1rem;
}

.product-card__image {
  width: 100%;
}

.product-card__title {
  font-size: 1.2rem;
}

/* Avoid */
.product-card div img {
  width: 100%;
}

.pc_t {
  font-size: 1.2rem;
}
```

### JavaScript:
- Use descriptive variable and function names
- Add comments for complex logic
- Follow camelCase convention
- Avoid global variables
- Use arrow functions where appropriate

```javascript
// Good
const addToCart = (productId, quantity) => {
  // Add product to cart logic
  const product = getProductById(productId);
  cart.addItem(product, quantity);
};

// Avoid
function add(id) {
  // ...
}
window.global_cart = [];
```

## Testing Your Changes

### Browser Testing Checklist:
- [ ] Chrome/Edge (latest)
- [ ] Firefox (latest)
- [ ] Safari (latest)
- [ ] Mobile browsers (iOS Safari, Chrome Mobile)

### Responsive Design Checklist:
- [ ] Desktop (1920px+)
- [ ] Tablet (768px - 1024px)
- [ ] Mobile (320px - 767px)

### Functionality Checklist:
- [ ] All links work correctly
- [ ] Forms submit properly
- [ ] Images load and display correctly
- [ ] No console errors or warnings
- [ ] Page loads within 3 seconds

## Review Process

1. A maintainer will review your PR within 2-7 days
2. You may be asked for changes or clarifications
3. Once approved, your PR will be merged
4. Your contribution will be celebrated! 🎉

### Tips for a Smoother Review:
- Keep PRs focused (don't mix multiple unrelated changes)
- Add clear descriptions of what changed and why
- Include visual evidence (screenshots/videos)
- Respond to feedback promptly and professionally

## Getting Help

- **Questions?** Open a discussion or issue
- **Need guidance?** Check existing code and comments
- **Stuck?** Reach out to maintainers
- **Community:** Be respectful and supportive

## Attribution

Contributors will be:
- Listed in the project (if you'd like)
- Credited in commit history
- Thanked in release notes

## License

By contributing to Black Diamond Store, you agree that your contributions will be licensed under the same license as the project (MIT License).

---

**Thank you for making Black Diamond Store better! 💎**

Questions? Open an issue or reach out to the maintainers.
