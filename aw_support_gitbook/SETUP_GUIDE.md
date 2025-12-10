# GitBook Setup Guide

This guide will help you set up the A+W Support documentation with GitHub and GitBook.

## Prerequisites

- GitHub account
- GitBook account (free or paid)
- Git installed locally

## Step 1: Create GitHub Repository

### Option A: GitHub Web Interface

1. Go to [GitHub](https://github.com)
2. Click "New repository"
3. Name it: `aw-support-docs` (or your preferred name)
4. Set to Public or Private
5. Do NOT initialize with README (we already have one)
6. Click "Create repository"

### Option B: GitHub CLI

```bash
gh repo create aw-support-docs --public --source=. --remote=origin
```

## Step 2: Push to GitHub

```bash
# Navigate to the gitbook directory
cd aw_support_gitbook

# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: A+W Support Documentation"

# Add remote (replace YOUR_USERNAME)
git remote add origin https://github.com/YOUR_USERNAME/aw-support-docs.git

# Push to GitHub
git branch -M main
git push -u origin main
```

## Step 3: Connect to GitBook

### Create GitBook Space

1. Go to [GitBook](https://www.gitbook.com)
2. Sign in or create account
3. Click "New Space"
4. Choose "Import from GitHub"

### Connect GitHub Repository

1. Authorize GitBook to access GitHub
2. Select your repository: `aw-support-docs`
3. Choose branch: `main`
4. GitBook will automatically sync

### Configure Sync

GitBook will automatically:
- Detect `SUMMARY.md` for navigation
- Use `README.md` as homepage
- Apply `.gitbook.yaml` configuration
- Sync on every push to main branch

## Step 4: Customize GitBook

### Space Settings

1. Go to Space Settings
2. Set:
   - **Name:** A+W Support Documentation
   - **Description:** Comprehensive support resources for A+W Software
   - **Visibility:** Public or Private
   - **Domain:** (optional custom domain)

### Appearance

1. Choose theme (Light/Dark)
2. Upload logo (A+W logo)
3. Set primary color
4. Configure header/footer

### Integrations

Optional integrations:
- Google Analytics
- Intercom
- Slack notifications
- Custom scripts

## Step 5: Test the Documentation

1. Visit your GitBook space URL
2. Verify navigation structure
3. Test internal links
4. Check page formatting
5. Test search functionality

## Step 6: Ongoing Updates

### Making Changes

```bash
# Make changes to markdown files
# Then commit and push

git add .
git commit -m "Update documentation"
git push origin main
```

GitBook will automatically sync within minutes.

### Adding New Pages

1. Create new markdown file in appropriate folder
2. Add entry to `SUMMARY.md`
3. Commit and push

### Reorganizing

1. Move files to new locations
2. Update links in affected pages
3. Update `SUMMARY.md`
4. Commit and push

## GitBook Features

### Search

GitBook provides full-text search automatically.

### Versioning

Create versions for different releases:
1. Go to Versions
2. Create new version
3. Link to different branches

### PDF Export

Export documentation as PDF:
1. Go to Space Settings
2. Click "Export as PDF"
3. Download

### Analytics

Track usage with built-in analytics:
- Page views
- Search queries
- Popular pages
- User locations

## Troubleshooting

### Sync Not Working

1. Check GitHub connection in GitBook settings
2. Verify `.gitbook.yaml` is valid
3. Check GitBook sync logs
4. Re-authorize GitHub access

### Broken Links

1. Use relative links for internal pages
2. Ensure file paths match SUMMARY.md
3. Check for typos in links

### Navigation Issues

1. Verify SUMMARY.md syntax
2. Check indentation (use spaces, not tabs)
3. Ensure all referenced files exist

## Best Practices

### Content

- Keep pages focused and concise
- Use clear headings
- Include examples
- Add images where helpful
- Cross-reference related pages

### Organization

- Group related pages in folders
- Use descriptive filenames
- Maintain consistent structure
- Update SUMMARY.md when adding pages

### Maintenance

- Review and update regularly
- Fix broken links promptly
- Archive outdated content
- Respond to feedback

## Support

### GitBook Support

- [GitBook Documentation](https://docs.gitbook.com)
- [GitBook Community](https://github.com/GitbookIO/gitbook/discussions)
- [GitBook Support](https://www.gitbook.com/support)

### A+W Documentation Team

Contact the A+W Documentation Team for:
- Content questions
- Access requests
- Technical issues

---

**Next Steps:**
1. Follow this guide to set up GitHub and GitBook
2. Customize appearance and settings
3. Invite team members
4. Start adding detailed content
5. Share with users

**Questions?** Contact the A+W Digital Innovation Team
