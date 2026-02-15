# Contributing to Sentinel

Thank you for your interest in contributing to Sentinel! This guide will help you understand how to contribute effectively to this documentation project.

## Table of Contents

- [Code of Conduct](#code-of-conduct)
- [How Can I Contribute?](#how-can-i-contribute)
- [Getting Started](#getting-started)
- [Documentation Standards](#documentation-standards)
- [Style Guide](#style-guide)
- [Submission Guidelines](#submission-guidelines)
- [Review Process](#review-process)
- [Recognition](#recognition)

---

## Code of Conduct

### Our Pledge

We are committed to providing a welcoming and inclusive environment for all contributors. We expect all participants to:

- Be respectful and considerate in communication
- Accept constructive criticism gracefully
- Focus on what is best for the community
- Show empathy towards other community members
- Respect differing viewpoints and experiences

### Unacceptable Behavior

- Harassment, discrimination, or intimidation of any kind
- Trolling, insulting comments, or personal attacks
- Publishing others' private information without permission
- Any conduct that could reasonably be considered inappropriate

### Enforcement

Instances of unacceptable behavior may be reported to the project maintainer at [hey@mechobliterate.com](mailto:hey@mechobliterate.com). All complaints will be reviewed and investigated promptly and fairly.

---

## How Can I Contribute?

### Reporting Issues

**Found a bug or outdated information?**

1. Check if the issue already exists in the [issue tracker](https://github.com/mechobliterate/Sentinel/issues)
2. If not, create a new issue with:
   - Clear, descriptive title
   - Detailed description of the problem
   - App name and version number
   - Steps to reproduce (if applicable)
   - Screenshots or screen recordings (if helpful)
   - Date you verified the information

**Example Issue Title:** `[Instagram] Privacy Settings Moved in v250.0`

### Suggesting New Apps

Want documentation for an app not yet covered?

1. Open an issue with the "app request" label
2. Include:
   - App name and category
   - Why this app should be documented (popularity, privacy concerns)
   - Link to the app's official website
   - Any known privacy issues or controversies

### Updating Existing Documentation

Apps frequently update their privacy settings. Help us keep documentation current:

1. Verify the current app version
2. Check all settings mentioned in the guide
3. Note any changes, additions, or removals
4. Update the guide accordingly
5. Update the "Last Updated" date and version number

### Adding New Documentation

Ready to document a new app? Great!

1. Check the [documentation template](templates/app-template.md)
2. Research the app's privacy settings thoroughly
3. Take clear screenshots of each setting
4. Test the settings yourself
5. Note any functionality trade-offs
6. Be honest about what data is still collected

---

## Getting Started

### Prerequisites

- GitHub account
- Markdown knowledge (basic formatting)
- The application you're documenting installed and accessible
- Screenshot capability

### Fork and Clone

1. Fork the repository to your GitHub account
2. Clone your fork locally:
   ```bash
   git clone https://github.com/mechobliterate/Sentinel.git
   cd Sentinel
   ```
3. Create a new branch for your work:
   ```bash
   git checkout -b feature/app-name-guide
   ```

### Development Workflow

1. Make your changes in the appropriate directory
2. Test that all markdown renders correctly
3. Commit your changes with clear messages:
   ```bash
   git add .
   git commit -m "Add Instagram privacy guide for v250.0"
   ```
4. Push to your fork:
   ```bash
   git push origin feature/app-name-guide
   ```
5. Open a pull request to the main repository

---

## Documentation Standards

### File Naming

- Use lowercase with hyphens: `app-name.md`
- Be specific: `google-drive.md` not `drive.md`
- For OS versions, include number: `ios-26.md`

### Directory Structure

Place your documentation in the appropriate category:

```
Operating Systems/    # OS-level privacy settings
social-media/        # Social networking platforms
Browsers/            # Web browsers
Communication/       # Messaging and video chat apps
Cloud Services/      # Cloud storage and email
Streaming/           # Music and video streaming
```

### Required Sections

Every guide must include:

1. **Title and Overview**
   - App name
   - Brief description
   - Key privacy concerns

2. **Quick Settings Checklist**
   - Actionable checkboxes
   - Most important settings first

3. **Detailed Configuration**
   - Step-by-step instructions
   - Clear section headings
   - Screenshots for complex settings

4. **What Data Is Still Collected**
   - Be transparent about limitations
   - Explain required data collection

5. **Last Updated**
   - Date (YYYY-MM-DD format)
   - App version number

### Screenshot Guidelines

**Quality Requirements:**
- Use high-resolution screenshots (minimum 1080p)
- Crop to show only relevant content
- Highlight the setting being discussed (use red boxes or arrows)
- Use consistent device/theme when possible
- Remove or blur personal information

**File Management:**
- Save as PNG format
- Name descriptively: `instagram-account-privacy-settings.png`
- Store in `images/[category]/[app-name]/` directory
- Keep file sizes reasonable (compress if needed)
- Include alt text in markdown for accessibility

**Example:**
```markdown
![Instagram account privacy toggle highlighted in red](images/social-media/instagram/account-privacy-toggle.png)
```

### Accessibility

- Use clear, plain language
- Avoid jargon when possible
- Define technical terms when first used
- Use descriptive alt text for images
- Ensure proper heading hierarchy (h1 → h2 → h3)
- Provide text alternatives for visual information

---

## Style Guide

### Writing Style

**Tone:**
- Professional but approachable
- Empowering, not fear-mongering
- Clear and concise
- Avoid marketing language or hyperbole

**Voice:**
- Use second person ("you") when addressing readers
- Use active voice: "Disable this setting" not "This setting should be disabled"
- Be direct and specific

**Example - Good:**
> Navigate to Settings > Privacy > Activity Status and toggle off "Show Activity Status" to prevent others from seeing when you're online.

**Example - Poor:**
> You might want to think about possibly disabling the activity status feature if you're concerned about privacy, which can be found somewhere in the settings area.

### Formatting

**Headers:**
```markdown
# App Name Privacy Settings (h1 - title only)

## Main Sections (h2)

### Subsections (h3)

#### Minor Subsections (h4)
```

**Emphasis:**
- **Bold** for UI elements, button names, menu items
- *Italics* for emphasis sparingly
- `Code formatting` for file paths, commands, technical terms

**Lists:**
- Use numbered lists for sequential steps
- Use bullet points for non-sequential items
- Keep list items parallel in structure

**Links:**
- Use descriptive link text: [Instagram Privacy Policy](https://instagram.com/privacy)
- Not: Click [here](https://instagram.com/privacy)

**Warnings and Notes:**

```markdown
⚠️ **Warning:** Disabling this will prevent the app from functioning properly.

💡 **Note:** This setting may not be available in all regions.

✅ **Tip:** Consider using this alternative approach for better privacy.
```

### Technical Accuracy

- Always specify app version numbers
- Test settings yourself before documenting
- Provide exact paths to settings: Settings > Privacy > Data & Personalization
- Use exact UI text as it appears in the app
- Note platform differences (iOS vs Android, etc.)

### Completeness Checklist

Before submitting, ensure:

- [ ] All sections from the template are included
- [ ] Settings are current and verified
- [ ] Screenshots are clear and properly labeled
- [ ] Links are working and point to official sources
- [ ] Spelling and grammar are correct
- [ ] App version and date are specified
- [ ] Limitations are honestly disclosed
- [ ] Alternative approaches are mentioned when applicable

---

## Submission Guidelines

### Pull Request Process

1. **Before Submitting:**
   - Review your changes for accuracy
   - Run a markdown linter if available
   - Check that all links work
   - Verify screenshots are clear and properly referenced

2. **Pull Request Template:**

```markdown
## Description
Brief description of what this PR adds or changes

## Type of Change
- [ ] New app documentation
- [ ] Update to existing documentation
- [ ] Bug fix (typo, broken link, etc.)
- [ ] Translation
- [ ] Other (please describe)

## App Information
- App Name: [e.g., Instagram]
- App Version: [e.g., 250.0]
- Platform: [e.g., iOS 26, Android 15]
- Date Verified: [YYYY-MM-DD]

## Checklist
- [ ] I have tested these settings myself
- [ ] Screenshots are clear and properly labeled
- [ ] All links are working
- [ ] Documentation follows the style guide
- [ ] Last Updated date is current
- [ ] I have disclosed any limitations or trade-offs

## Additional Context
Any additional information reviewers should know
```

3. **Commit Message Format:**

```
type(scope): brief description

Longer description if needed

Examples:
- feat(instagram): add privacy guide for version 250.0
- fix(firefox): update tracking protection settings path
- docs(readme): correct broken links in resources section
- update(ios): refresh for iOS 26 release
```

Types: `feat`, `fix`, `docs`, `update`, `refactor`, `test`, `chore`

### Review Timeline

- Initial review: Within 7 days
- Follow-up reviews: Within 3-5 days
- Maintainers may request changes or clarifications
- Be responsive to feedback and questions

### After Your PR Is Merged

- Your contribution will be added to the changelog
- You'll be recognized in the contributors list
- Consider watching the repository for future updates
- Help review other contributions if you're interested

---

## Review Process

### What We Look For

**Accuracy:**
- Settings are correctly described
- Instructions work as written
- Information is current and verified

**Completeness:**
- All required sections are included
- Instructions are detailed enough to follow
- Edge cases and limitations are noted

**Quality:**
- Writing is clear and professional
- Screenshots are high-quality
- Formatting is consistent with existing docs

**Usability:**
- A non-technical person could follow the guide
- Potential issues are called out
- Alternative approaches are mentioned

### Common Reasons for Requested Changes

- Missing screenshots or unclear images
- Outdated information or wrong app version
- Incomplete instructions or skipped steps
- Inconsistent formatting or style
- Broken links or missing references
- Spelling or grammatical errors
- Missing disclosure of trade-offs

---

## Recognition

### Contributors

All contributors are recognized in:
- The repository's Contributors page
- The Acknowledgments section of the README
- The git history

### Significant Contributions

Contributors who make substantial contributions may be:
- Highlighted in release notes
- Given reviewer access (if interested)
- Consulted on major project decisions

We value all contributions, regardless of size. Every typo fix, every updated screenshot, and every new guide helps protect people's privacy.

---

## Questions?

- **General questions:** Open a discussion on GitHub
- **Specific issues:** Create an issue with the "question" label  
- **Private matters:** Contact the maintainer directly

---

## Translation Guidelines

### Starting a Translation

1. Create a new directory: `translations/[language-code]/`
2. Translate the README.md first
3. Maintain the same directory structure as the English version
4. Keep file names in English for consistency

### Translation Standards

- Maintain the same tone and style
- Adapt examples to be culturally relevant when appropriate
- Keep technical terms consistent
- Note if certain settings aren't available in specific regions
- Add yourself to translators list in the translated README

### Updating Translations

- Translations may become outdated as the English version is updated
- Use Git to track which commits need to be translated
- Add "Translation Status" section noting last English commit translated

---

## License Agreement

By contributing to Sentinel, you agree that your contributions will be licensed under the same license as the project. You retain copyright of your contributions but grant rights as specified in the [LICENSE](LICENSE) file.

You also affirm that:
- Your contribution is your original work
- You have the right to submit the contribution
- You understand the contribution becomes part of the public repository

---

## Getting Help

**New to Git/GitHub?**
- [GitHub's Hello World Guide](https://guides.github.com/activities/hello-world/)
- [Git Handbook](https://guides.github.com/introduction/git-handbook/)
- [Markdown Guide](https://www.markdownguide.org/)

**New to Privacy Documentation?**
- Review existing guides to understand our approach
- Start with small updates before tackling complete guides
- Ask questions - we're here to help!

**Technical Issues?**
- Check the [Issues](https://github.com/mechobliterate/Sentinel/issues) page
- Ask in Discussions
- Contact maintainers if stuck

---

Thank you for contributing to Sentinel! Your efforts help protect privacy for users around the world.

**Last Updated:** February 15, 2026
