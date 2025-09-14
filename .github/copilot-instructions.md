# GitHub Profile Documentation Repository

**ALWAYS follow these instructions first and fallback to additional search and
context gathering ONLY if the information in these instructions is incomplete
or found to be in error.**

This is a documentation and profile repository for BoozeLee (AI/ML engineer)
and the Bakery Street Project organization. This repository contains profile
README files, documentation, and branding materials rather than traditional
application code.

## Working Effectively

### Repository Structure

- **Root README.md**: Personal GitHub profile for @BoozeLee
- **Bakery-street-projct/README.md**: Organization profile for
  @Bakery-street-projct
- **BoozeLee/README.md**: Additional personal profile content
- **GITHUB_UPGRADE_PLAN.md**: Strategic planning document for profile
  enhancement
- **payment_setup.md**: Payment and monetization setup documentation
- **logo.png**: Profile branding asset

### Required Tools Installation

Install markdown validation tools that are REQUIRED for this repository:

```bash
npm install -g markdownlint-cli markdown-link-check
```

- **NEVER CANCEL**: Installation takes 30-45 seconds. Set timeout to 60+
  seconds.
- **Validation**: Run `markdownlint --version` and
  `markdown-link-check --version` to confirm installation

### Documentation Validation Workflow

Run these validation commands for ALL markdown changes:

1. **Markdown Linting** (REQUIRED before commits):

```bash
markdownlint *.md
markdownlint Bakery-street-projct/README.md
markdownlint BoozeLee/README.md
```

- **Timing**: Takes 2-5 seconds per file
- **Action Required**: Fix ALL linting errors before committing
- **Common Issues**: Line length (80 chars), missing blank lines around
  headings/lists

1. **Link Validation** (REQUIRED for external links):

```bash
markdown-link-check README.md
markdown-link-check Bakery-street-projct/README.md
markdown-link-check BoozeLee/README.md
```

- **NEVER CANCEL**: Takes 15-30 seconds per file depending on network. Set
  timeout to 60+ seconds.
- **Expected Behavior**: Many badge/shield URLs may show as "dead links" due
  to network restrictions - this is NORMAL
- **Action Required**: Verify that GitHub repository links and major service
  links are working

### Development and Testing Commands

**ALWAYS run validation before making changes:**

```bash
# Test current state
markdownlint *.md Bakery-street-projct/README.md BoozeLee/README.md
```

**ALWAYS run validation after making changes:**

```bash
# Validate all markdown files
markdownlint *.md Bakery-street-projct/README.md BoozeLee/README.md
# Check critical links (external validation may timeout - this is normal)
markdown-link-check README.md
```

### File Editing Guidelines

**When editing markdown files:**

- Keep lines under 80 characters when possible
- Add blank lines before and after all headings
- Add blank lines before and after all lists
- Use proper markdown link syntax instead of bare URLs
- Test locally before committing

**Profile Content Guidelines:**

- Maintain professional tone and branding consistency
- Ensure all GitHub repository links point to actual repositories
- Keep contact information current
- Use consistent emoji and formatting patterns

## Validation Scenarios

**CRITICAL**: After making any changes to documentation, ALWAYS test these
complete scenarios:

### Scenario 1: Markdown Validation

1. Run markdownlint on all files:
   `markdownlint *.md Bakery-street-projct/README.md BoozeLee/README.md`
2. Verify NO errors are reported
3. If errors exist, fix them before proceeding

### Scenario 2: Link Validation

1. Run link checker on main README: `markdown-link-check README.md`
2. Verify GitHub repository links are accessible (404 errors indicate missing
   repos)
3. Note that badge/shield URLs may timeout - this is expected behavior

### Scenario 3: Profile Display

1. View each README file in a markdown preview
2. Verify formatting appears correctly
3. Check that images display properly
4. Ensure all sections are properly structured

## Common Tasks

### Adding New Documentation

1. Create markdown file following existing structure
2. Run `markdownlint <filename>.md` to validate syntax
3. Run `markdown-link-check <filename>.md` to validate links
4. Fix any issues before committing

### Updating Profile Information

1. Edit appropriate README.md file (root, Bakery-street-projct/, or BoozeLee/)
2. Maintain consistent formatting and emoji usage
3. Validate with markdownlint
4. Test link accessibility
5. Commit changes

### Managing Assets

- Images should be placed in repository root
- Use relative paths for local images: `![Alt text](logo.png)`
- Optimize images for web display
- Maintain consistent branding

## Timing Expectations

- **Markdown linting**: 2-5 seconds per file
- **Link checking**: 15-30 seconds per file (NEVER CANCEL - network timeouts
  are normal)
- **Tool installation**: 30-45 seconds (NEVER CANCEL)
- **File editing**: No build time - immediate

## Repository Information Cache

### Root Directory Contents

```text
.
├── .github/
├── Bakery-street-projct/
│   └── README.md
├── BoozeLee/
│   └── README.md
├── GITHUB_UPGRADE_PLAN.md
├── README.md
├── logo.png
└── payment_setup.md
```

### Key File Purposes

- **README.md**: Main personal profile (122 lines)
- **Bakery-street-projct/README.md**: Organization profile (208 lines)
- **BoozeLee/README.md**: Additional personal content (126 lines)
- **GITHUB_UPGRADE_PLAN.md**: Strategic documentation (276 lines)
- **payment_setup.md**: Business setup guide (62 lines)

### Validation Status

- **Markdown Linting**: Multiple formatting issues exist (line length,
  spacing)
- **Link Checking**: Several broken GitHub repository links (404 errors)
- **Badge URLs**: Network timeouts expected for shield.io badges

## NEVER Do These Things

- **NEVER skip markdown validation** - always run markdownlint before
  committing
- **NEVER ignore linting errors** - fix all formatting issues
- **NEVER cancel long-running link checks** - network timeouts are expected
- **NEVER commit without testing** - validate changes locally first
- **NEVER break existing formatting patterns** - maintain consistency

## Critical Reminders

- **This is NOT a code repository** - no compilation, building, or traditional
  testing
- **Focus on documentation quality** - content and formatting are primary
  concerns
- **External link failures are normal** - many URLs may be blocked or timeout
- **Validation is MANDATORY** - always run linting and link checking
- **NEVER CANCEL validation commands** - set appropriate timeouts (60+
  seconds)
