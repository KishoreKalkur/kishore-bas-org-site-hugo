# GitHub Repository Setup Instructions

## Repository Name: `kishore-bas-org-site-hugo`

### Option 1: Using GitHub Web Interface

1. Go to https://github.com/new
2. Repository name: `kishore-bas-org-site-hugo`
3. Description: "Bangalore Astronomical Society website built with Hugo"
4. Set to **Public**
5. **DO NOT** initialize with README, .gitignore, or license (we already have them)
6. Click "Create repository"

### Option 2: Using GitHub CLI (after authentication)

```bash
# First authenticate GitHub CLI
gh auth login

# Then create the repository
gh repo create kishore-bas-org-site-hugo --public --description "Bangalore Astronomical Society website built with Hugo" --source=. --remote=origin --push
```

### After Creating the Repository

Since you already have the remote set up, just push the code:

```bash
# Push the code
git push -u origin main
```

### Verify the Push

After pushing, your repository should be available at:
https://github.com/KishoreKalkur/kishore-bas-org-site-hugo

### Next Steps

1. **Set up GitHub Pages** (optional):

   - Go to Settings → Pages
   - Source: Deploy from a branch
   - Branch: main
   - Folder: /public
   - Or use GitHub Actions for Hugo deployment

2. **Configure Custom Domain** (if needed):

   - Add CNAME file with your domain
   - Configure DNS settings

3. **Enable Issues/Discussions** (optional):
   - For community engagement and support
