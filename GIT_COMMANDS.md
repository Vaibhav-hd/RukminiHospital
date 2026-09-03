# 📝 Git Commands Guide - GitHub Deployment

## First Time Setup

### 1. Configure Git (One time only)
```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@gmail.com"
```

### 2. Clone Your Repository
```bash
git clone https://github.com/YOUR-USERNAME/rukmini-hospital.git
cd rukmini-hospital
```

### 3. Copy Files to Folder
- Place these files in the `rukmini-hospital` folder:
  - `index.html`
  - `thankyou.html`
  - `logo.png`
  - `doctor.jpg`
  - `README.md`
  - `QUICKSTART.md`
  - `.gitignore`

---

## Upload Files to GitHub (First Time)

### Step 1: Check Status
```bash
git status
```
**Expected Output:**
```
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        thankyou.html
        logo.png
        doctor.jpg
        README.md
```

### Step 2: Add All Files
```bash
git add .
```

### Step 3: Create Commit
```bash
git commit -m "Initial commit: Add Rukmini Hospital website v2.0"
```

### Step 4: Push to GitHub
```bash
git push -u origin main
```

**Expected Output:**
```
Counting objects: 6, done.
Delta compression using up to 4 threads.
Compressing objects: 100% (5/5), done.
Writing objects: 100% (6/6), 2.45 MiB | 500 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To https://github.com/YOUR-USERNAME/rukmini-hospital.git
 * [new branch]      main -> main
Branch 'main' set up to track remote branch 'main' from 'origin'.
```

---

## Update Website (After Changes)

### For Small Changes (Text, Colors)

```bash
# 1. View changes
git status

# 2. Add changes
git add .

# 3. Commit with message
git commit -m "Update doctor information and contact details"

# 4. Push to GitHub
git push origin main
```

**Changes will be live in 1-2 minutes!**

---

## Update Website (For Specific Files)

### Update Only One File
```bash
# Add specific file
git add index.html

# Commit
git commit -m "Update appointment form styling"

# Push
git push origin main
```

### Update Multiple Specific Files
```bash
# Add specific files
git add index.html thankyou.html

# Commit
git commit -m "Update homepage and thank you page"

# Push
git push origin main
```

---

## Useful Git Commands

### View Commit History
```bash
git log --oneline
```

### View All Changes
```bash
git status
```

### Show Detailed Changes
```bash
git diff
```

### Revert Last Commit
```bash
git reset --soft HEAD~1
```

### Remove a File from Tracking
```bash
git rm --cached filename.txt
```

### Change Last Commit Message
```bash
git commit --amend -m "New commit message"
```

### View Remote URL
```bash
git remote -v
```

---

## Common Scenarios

### Scenario 1: Update Doctor Image

```bash
# Replace doctor.jpg with new image
# (Save new image as doctor.jpg)

# Then run:
git add doctor.jpg
git commit -m "Update doctor profile image"
git push origin main
```

### Scenario 2: Update Phone Number

```bash
# Edit index.html
# Search and replace: 918669369486

git add index.html
git commit -m "Update contact phone number"
git push origin main
```

### Scenario 3: Add New Service

```bash
# Edit index.html
# Add new service card in services section

git add index.html
git commit -m "Add new physiotherapy service"
git push origin main
```

### Scenario 4: Update Email

```bash
# Edit index.html
# Change: vaikunthviewdoc@gmail.com

git add index.html
git commit -m "Update hospital email address"
git push origin main
```

---

## Troubleshooting Git

### Error: "fatal: not a git repository"
**Solution:**
```bash
# Navigate to correct folder
cd rukmini-hospital

# Or re-clone
git clone https://github.com/YOUR-USERNAME/rukmini-hospital.git
```

### Error: "Permission denied (publickey)"
**Solution:**
```bash
# Use HTTPS instead of SSH
git remote set-url origin https://github.com/YOUR-USERNAME/rukmini-hospital.git
git push origin main
```

### Error: "failed to push some refs"
**Solution:**
```bash
# Pull latest changes first
git pull origin main

# Then try again
git push origin main
```

### Error: "The file is too large"
**Solution:**
```bash
# For GitHub's 100MB limit
# Use Git LFS for large files
git lfs install
git lfs track "*.jpg"
git add .gitattributes
git add doctor.jpg
git commit -m "Update large image"
git push origin main
```

### Changes Not Appearing on Website
**Solution:**
```bash
# Hard refresh browser
# Windows: Ctrl + Shift + R
# Mac: Cmd + Shift + R

# Or clear cache in browser settings
# Then wait 1-2 minutes for deployment
```

---

## Best Practices

### 1. Meaningful Commit Messages
✅ **Good:**
```bash
git commit -m "Update appointment form validation and styling"
```

❌ **Bad:**
```bash
git commit -m "update"
git commit -m "changes"
```

### 2. Commit Frequently
```bash
# Make small, logical commits
git add index.html
git commit -m "Update hero section text"

git add style.css
git commit -m "Add hover effects to buttons"
```

### 3. Check Before Pushing
```bash
# Always check status first
git status

# Review changes
git diff

# Then commit and push
git add .
git commit -m "Description"
git push origin main
```

### 4. Keep Commit Messages Short
```bash
# First line should be short (50 chars)
# Optional: Add detailed description below
git commit -m "Update doctor info

- Changed credentials
- Updated bio
- Added new services"
```

---

## Workflow Example

### Complete Update Workflow

```bash
# 1. Navigate to project
cd rukmini-hospital

# 2. Check status
git status

# 3. Make your changes (edit files)
# - Update index.html
# - Update logo.png
# - etc.

# 4. View what changed
git status

# 5. Add changes
git add .

# 6. Commit with message
git commit -m "Update hospital information and branding"

# 7. Push to GitHub
git push origin main

# 8. Check online (wait 1-2 minutes)
# Open: https://YOUR-USERNAME.github.io/rukmini-hospital/
```

---

## GitHub Web Interface (Alternative to Git Commands)

### Upload Files via GitHub Website

1. Go to your repository: `github.com/YOUR-USERNAME/rukmini-hospital`
2. Click **Add file** → **Upload files**
3. Drag and drop your files
4. Click **Commit changes**

### Edit Files via GitHub Website

1. Click on file (e.g., `index.html`)
2. Click ✏️ **Edit** button
3. Make changes
4. Scroll down → Click **Commit changes**

### Delete Files via GitHub Website

1. Click on file
2. Click **...** menu
3. Click **Delete** file
4. Click **Commit changes**

---

## Pro Tips

### Tip 1: Create New Branches (Advanced)
```bash
# Create feature branch
git checkout -b feature/new-services

# Make changes and commit
git add .
git commit -m "Add new services section"

# Push branch
git push origin feature/new-services

# Merge to main in GitHub (via Pull Request)
```

### Tip 2: Revert Changes
```bash
# Undo uncommitted changes
git checkout -- index.html

# Undo last commit (keep changes)
git reset --soft HEAD~1

# Undo last commit (discard changes)
git reset --hard HEAD~1
```

### Tip 3: Stash Changes
```bash
# Save changes temporarily
git stash

# Bring back saved changes
git stash pop
```

### Tip 4: View Branch Info
```bash
# See current branch
git branch

# Switch branch
git checkout main

# See all branches
git branch -a
```

---

## Git Cheat Sheet

| Command | Purpose |
|---------|---------|
| `git clone URL` | Copy repository |
| `git status` | Check changes |
| `git add .` | Add all files |
| `git add file.txt` | Add specific file |
| `git commit -m "msg"` | Create commit |
| `git push origin main` | Push to GitHub |
| `git pull origin main` | Pull from GitHub |
| `git log --oneline` | View history |
| `git diff` | Show changes |
| `git reset HEAD~1` | Undo commit |

---

## Deploy Your Website

### First Deployment (from scratch)
1. Create GitHub account
2. Create repository
3. Run git commands above
4. Enable GitHub Pages
5. Wait 1-2 minutes
6. Visit: `https://YOUR-USERNAME.github.io/rukmini-hospital/`

### Update Deployment
1. Make changes to files
2. Run: `git add .`
3. Run: `git commit -m "description"`
4. Run: `git push origin main`
5. Wait 1-2 minutes
6. Refresh website

---

## Support

**GitHub Help:** https://docs.github.com/
**Git Documentation:** https://git-scm.com/doc
**GitHub Pages:** https://pages.github.com/

---

## Quick Reference Card

```
FIRST TIME:
git clone [URL]
git add .
git commit -m "message"
git push -u origin main

UPDATES:
git add .
git commit -m "message"
git push origin main

CHECK:
git status
git log --oneline
```

---

**Happy Coding! 🚀**

For Rukmini Hospital Website v2.0
