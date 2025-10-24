# GitHub Copilot Instructions for github-slideshow

This repository is a GitHub Learning Lab slideshow project built with Jekyll and reveal.js for teaching GitHub basics.

## Project Overview
- **Purpose**: Interactive presentation/slideshow for learning GitHub fundamentals
- **Framework**: Jekyll static site generator with reveal.js presentation library
- **Deployment**: Configured for GitHub Pages
- **Primary Language**: Ruby (Jekyll), with HTML, CSS, JavaScript (reveal.js), and Markdown (content)

## Coding Standards

### Ruby/Jekyll
- Follow Ruby community style guide conventions
- Maintain compatibility with GitHub Pages' Jekyll version
- Keep plugins minimal and only use those supported by GitHub Pages

### YAML Configuration
- Use 2-space indentation in `_config.yml` and YAML frontmatter
- Quote string values containing special characters
- Maintain alphabetical ordering of top-level keys where practical
- Comment complex or non-obvious configuration options

### Markdown Content
- Use standard Markdown syntax for slide content in `_posts/` directory
- Follow Jekyll post naming convention: `YYYY-MM-DD-title.md`
- Include proper YAML frontmatter in all post files
- Keep slide content concise and focused

### HTML/JavaScript
- Preserve existing reveal.js configuration and customization
- Use semantic HTML5 elements
- Maintain accessibility standards (WCAG 2.1 AA)
- Keep JavaScript modifications minimal and well-commented

## Dependencies
- **Jekyll**: Static site generator (GitHub Pages compatible version)
- **reveal.js**: HTML presentation framework
- **jemoji**: Jekyll plugin for GitHub-flavored emoji support
- **Ruby gems**: Managed via `Gemfile` and `Gemfile.lock`

## File Structure
```
├── .github/              # GitHub-specific configuration
├── _config.yml           # Jekyll configuration
├── _includes/            # Reusable template components
├── _layouts/             # Page layouts
├── _posts/               # Slide content (Markdown files)
├── index.html            # Main presentation entry point
├── Gemfile               # Ruby dependencies
└── README.md             # Project documentation
```

## Testing Requirements

### Before Committing
1. **YAML Validation**: Ensure all YAML files are syntactically valid
2. **Jekyll Build**: Test that `jekyll build` completes without errors
3. **Link Checking**: Verify all internal and external links work
4. **Browser Testing**: Check presentation renders correctly in modern browsers

### Build Commands
```bash
# Install dependencies
bundle install

# Build the site
bundle exec jekyll build

# Serve locally for testing
bundle exec jekyll serve
```

## Security Guidelines
- Never commit sensitive data (API keys, tokens, credentials)
- Validate and sanitize any user input if interactive features are added
- Keep dependencies up to date with security patches
- Review Dependabot alerts and apply fixes promptly

## Style Guidelines

### Code Formatting
- Use consistent indentation (2 spaces for YAML, HTML; 4 spaces for Ruby/Markdown)
- Keep lines under 100 characters where practical
- Add comments only when necessary to explain non-obvious logic

### Slide Content
- Use clear, concise language appropriate for beginners
- Include relevant emoji where they enhance understanding
- Break complex topics into multiple slides
- Maintain consistent visual style across slides

### Git Workflow
- Write clear, descriptive commit messages
- Keep commits focused on single logical changes
- Reference issue numbers in commit messages when applicable
- Follow conventional commit format when appropriate

## reveal.js Configuration
- Slide transitions should be smooth and professional
- Maintain keyboard navigation support
- Preserve mobile/touch device compatibility
- Keep default reveal.js settings unless there's a specific pedagogical reason to change them

## Documentation
- Update README.md when adding new features or changing setup procedures
- Document any non-standard configuration in comments
- Keep setup instructions beginner-friendly
- Include troubleshooting tips for common issues

## Additional Notes
- This is a learning project - prioritize clarity and educational value
- Changes should not break existing GitHub Learning Lab workflows
- Consider accessibility for users with disabilities
- Test changes with both GitHub Pages and local Jekyll builds
