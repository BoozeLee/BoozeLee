# BoozeLee GitHub Profile Repository

This is a GitHub profile repository containing markdown documentation for
BoozeLee's professional profile and the Bakery Street Project organization.
The repository contains profile READMEs, planning documents, and assets rather
than executable code.

**ALWAYS follow these instructions first and only fallback to additional search
and context gathering if the information here is incomplete or found to be in
error.**

## Working Effectively

### Bootstrap and Validation Setup

Run these commands to set up validation tools (takes ~30 seconds):

```bash
npm install -g markdownlint-cli markdown-link-check
```

### Validate Documentation

ALWAYS run validation before making changes:

**Markdown Linting** (takes ~2 seconds):

```bash
cd /home/runner/work/BoozeLee/BoozeLee
markdownlint *.md **/*.md
```

**Link Checking** (takes ~60 seconds per file - NEVER CANCEL):

```bash
cd /home/runner/work/BoozeLee/BoozeLee  
timeout 120 markdown-link-check README.md
timeout 120 markdown-link-check BoozeLee/README.md
timeout 120 markdown-link-check Bakery-street-projct/README.md
```

**Note**: External link validation often fails in sandboxed environments due
to network restrictions. This is expected and documented behavior.

### Repository Structure

```text
/home/runner/work/BoozeLee/BoozeLee/
├── README.md                      # Main BoozeLee profile
├── BoozeLee/README.md            # Secondary profile README  
├── Bakery-street-projct/README.md # Organization profile
├── GITHUB_UPGRADE_PLAN.md        # GitHub strategy document
├── payment_setup.md              # Payment configuration guide
├── logo.png                      # Logo asset
└── .github/copilot-instructions.md # This file
```

## Validation

### Manual Validation Requirements

After making any changes to documentation:

1. **ALWAYS run markdown linting** - Fix all linting errors before proceeding
2. **Run link checking** - Note that external links may fail due to network
   restrictions
3. **Review content accuracy** - Ensure all information is current and accurate
4. **Check formatting** - Verify headers, lists, and emphasis render correctly
5. **Validate assets** - Ensure images and files exist and are accessible

### Known Working Commands

The following commands are validated to work in this environment:

**Tool Installation** (30 seconds):

```bash
npm install -g markdownlint-cli markdown-link-check
```

**Markdown Validation** (2 seconds):

```bash
markdownlint *.md **/*.md
```

**Link Validation** (60-120 seconds per file - NEVER CANCEL):

```bash
markdown-link-check README.md
```

**Git Operations**:

```bash
git --no-pager status
git --no-pager diff
git --no-pager log --oneline -5
```

### Expected Timing

- **Tool installation**: 30 seconds
- **Markdown linting**: 2 seconds for all files
- **Link checking**: 60-120 seconds per file - NEVER CANCEL
- **Git operations**: Instant

## Common Tasks

### Updating Profile Documentation

1. **Edit markdown files** using str_replace_editor
2. **Run markdown linting**: `markdownlint *.md **/*.md`
3. **Fix any linting errors** before proceeding
4. **Test link checking**: `markdown-link-check [filename]` (expect external
   link failures)
5. **Review content** for accuracy and formatting
6. **Commit changes** using report_progress

### Adding New Content

1. **Follow existing markdown patterns** in the repository
2. **Use consistent emoji and formatting** style
3. **Validate all markdown** before committing
4. **Update related documents** if necessary (e.g., upgrade plan references)

### Fixing Documentation Issues

1. **Identify the issue** through linting or manual review
2. **Make minimal changes** to fix the specific issue
3. **Validate the fix** with appropriate tools
4. **Test that no new issues** were introduced

## Limitations and Known Issues

### Network Restrictions

- **External link validation fails** - This is expected in sandboxed
  environments
- **Badge/image URLs may not validate** - shields.io and external images are
  often blocked
- **Social media links fail** - Twitter, LinkedIn, PayPal links will show as
  broken

### No Traditional Build System

- **No package.json** - This is not a Node.js project
- **No requirements.txt** - This is not a Python project  
- **No executable code** - Repository contains only documentation
- **No tests to run** - Validation is done through linting tools only

### Working Validation Process

Since external links often fail validation:

1. **Focus on markdown linting** as primary validation
2. **Check internal links and file references** work correctly
3. **Manually verify critical external links** in issues/comments when possible
4. **Document known broken links** in commit messages if they cannot be fixed

## Repository Context

### Purpose

This repository serves as:

- **GitHub profile showcase** for BoozeLee (AI researcher/developer)
- **Organization profile** for Bakery Street Project  
- **Professional portfolio** with project descriptions and contact information
- **Business information** including services and payment options

### Key Files

- **README.md**: Main profile with comprehensive information about BoozeLee's
  work
- **BoozeLee/README.md**: Alternative profile format with additional details
- **Bakery-street-projct/README.md**: Organization profile for the research
  organization
- **GITHUB_UPGRADE_PLAN.md**: Detailed strategy for improving GitHub presence
- **payment_setup.md**: Configuration guide for payment processing setup

### Maintenance Focus

- **Keep content current** - Update achievements, projects, and contact
  information
- **Maintain consistent branding** - Ensure all profiles align with
  professional image
- **Validate markdown quality** - Run linting tools before any commits
- **Monitor link health** - Check for broken links and update as needed

## Critical Reminders

- **NEVER CANCEL long-running commands** - Link checking takes 60-120 seconds
  per file
- **ALWAYS run markdown linting** - Fix style issues before committing  
- **External link failures are expected** - Focus on content accuracy over link
  validation
- **Make minimal changes** - This is a documentation repository, preserve
  existing working content
- **Validate before committing** - Run all available validation tools first

The goal is to maintain high-quality, professional documentation that
represents BoozeLee's work effectively while ensuring the markdown is clean
and well-formatted.
