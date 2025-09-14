# BoozeLee Profile Repository - GitHub Copilot Instructions

Always reference these instructions first and fallback to search or bash commands only when you encounter unexpected information that does not match the info here.

## Repository Overview

The BoozeLee repository is a **profile and documentation repository** for an AI researcher and developer, not a traditional codebase. This repository contains:
- Personal and organizational profile documentation
- Service and payment information  
- Project showcases and portfolio content
- Marketing and professional presentation materials

**CRITICAL**: This is NOT a development codebase with build systems, tests, or runnable applications. All actual development work happens in separate repositories under the Bakery-street-projct organization.

## Working Effectively

### Repository Structure Validation
Always verify the current repository structure before making changes:
```bash
cd /home/runner/work/BoozeLee/BoozeLee
ls -la
# Expected structure:
# - README.md (main profile)
# - logo.png (profile image)
# - payment_setup.md (payment configuration)
# - GITHUB_UPGRADE_PLAN.md (upgrade strategy)
# - Bakery-street-projct/ (organization profile directory)
# - BoozeLee/ (personal profile directory)
# - .github/ (this instructions file)
```

### Documentation Editing Workflow
- **ALWAYS** validate markdown syntax after editing any .md files
- **ALWAYS** check all links work after updates
- **ALWAYS** maintain consistency between main README.md and subdirectory READMEs
- Use proper markdown formatting and emoji for visual consistency

### Link Validation (REQUIRED)
Before committing any changes, validate all external links:
```bash
# Test key external links - NEVER CANCEL, wait for completion (timeout: 60 seconds)
curl -I -s -L "https://paypal.me/REALbakerstreet221b" | head -3
curl -I -s -L "https://github.com/Bakery-street-projct" | head -3
curl -I -s -L "https://github.com/Bakery-street-projct/githubupdater-tools" | head -3
curl -I -s -L "https://github.com/Bakery-street-projct/dynamic-asynchronous-data-streamliner" | head -3
```

**NEVER CANCEL**: Link validation may take 30-60 seconds per link. Always wait for completion.

**Expected Results**:
- PayPal link: Should return HTTP 200 OK
- Bakery-street-projct organization: Should return HTTP 200 OK  
- Individual project repositories: May return HTTP 404 Not Found (repositories may be private or planned)
- Stripe test links: Expected to work (test environment)

**IMPORTANT**: 404 responses for project repositories are normal and expected - these may be private repositories or planned projects not yet created.

## Key Components and Maintenance

### 1. Profile Documentation Files
- **README.md**: Main profile showcase (personal brand)
- **Bakery-street-projct/README.md**: Organization profile
- **BoozeLee/README.md**: Personal subdirectory profile
- **GITHUB_UPGRADE_PLAN.md**: Strategic planning document

### 2. Payment and Service Information
- **payment_setup.md**: Payment configuration and setup
- **README.md sections**: Service pricing and payment buttons
- **Stripe links**: Test environment links (prefix: test_)
- **PayPal link**: https://paypal.me/REALbakerstreet221b

### 3. Project References
All project links reference external repositories in the Bakery-street-projct organization:
- Poly-AI Framework: https://github.com/Bakery-street-projct/githubupdater-tools
- DYADS Framework: https://github.com/Bakery-street-projct/dynamic-asynchronous-data-streamliner  
- Voidshatter Echo: https://github.com/Bakery-street-projct/voidshatterecho
- PeakyBlenders: https://github.com/Bakery-street-projct/PeakyBlenders

## Validation Requirements

### Manual Content Validation (REQUIRED)
After any changes, manually verify:
1. **Markdown Rendering**: Use GitHub's markdown preview
2. **Link Functionality**: Test all external links manually
3. **Badge Consistency**: Ensure all shields.io badges render correctly
4. **Content Consistency**: Verify information matches across all README files
5. **Contact Information**: Ensure all email, social media, and payment links are current

### Content Consistency Checklist
When updating profile information, ensure consistency across:
- [ ] Main README.md
- [ ] Bakery-street-projct/README.md  
- [ ] BoozeLee/README.md
- [ ] payment_setup.md
- [ ] Contact information (email, social media)
- [ ] Service pricing and descriptions
- [ ] Project descriptions and links

## Common Tasks

### Updating Profile Information
1. Edit the main README.md for personal brand updates
2. Update corresponding sections in subdirectory READMs
3. Validate all links still work
4. Check markdown formatting renders correctly
5. Ensure consistency across all profile documents

### Adding New Projects
1. Add project to Bakery-street-projct/README.md first
2. Add reference in main README.md
3. Update BoozeLee/README.md if showcasing personally
4. Validate external repository link exists and is public
5. Ensure project description is consistent across references

### Payment Information Updates
1. Edit payment_setup.md for configuration changes
2. Update payment sections in README.md
3. Test all payment links manually
4. Verify Stripe test environment links work
5. Confirm PayPal link redirects correctly

### Badge and Image Updates
All badges use shields.io format. When updating:
1. Use consistent style: `for-the-badge`
2. Maintain color consistency with existing badges
3. Test badge rendering after changes
4. Verify logo.png displays correctly in GitHub

## Critical Reminders

### What This Repository Is NOT
- **NOT a development codebase**: No source code to build or test
- **NOT a deployment target**: No applications to run or deploy  
- **NOT a CI/CD pipeline**: No automated builds or tests
- **NOT a package**: No installation or dependency management

### What This Repository IS
- **Profile showcase**: Personal and organizational branding
- **Documentation hub**: Information about services and projects
- **Payment portal**: Service pricing and payment processing
- **Professional presence**: Marketing and business development

### Content Guidelines
- Use imperative tone in service descriptions: "Contact for consultation", "Book development services"
- Maintain professional business language throughout
- Keep technical details high-level and accessible
- Focus on business value and outcomes
- Include clear calls-to-action for potential clients

### Emergency Content Issues
If payment links break or contact information becomes invalid:
1. **IMMEDIATELY** update payment_setup.md with corrected information
2. Update all README files with correct information
3. Test all links thoroughly before committing
4. Consider adding backup payment methods if primary fails

## Repository References

This profile repository showcases work that happens in these external repositories:
- **Bakery-street-projct organization**: https://github.com/Bakery-street-projct
- **Main development repositories**: Listed in project references above
- **Personal projects**: https://github.com/BoozeLee (separate from this profile repo)

Always reference the actual development repositories when discussing technical implementation details, as this repository only contains marketing and profile information.

## Final Note

Remember: This is a business profile and marketing repository. Changes should focus on professional presentation, accurate contact information, current service offerings, and compelling project showcases. Technical development work happens elsewhere and should only be referenced, not implemented here.