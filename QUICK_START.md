# 🚀 Quick Reference - Deploy Your GitHub Org Profile

## ⚡ 5-Minute Deploy

```bash
# 1. Navigate to directory
cd O:\GithubPages\.github

# 2. Initialize git
git init
git add .
git commit -m "Add Aethyrion organization profile"
git branch -M main

# 3. Create .github repo on GitHub first, then:
git remote add origin https://github.com/AethyrionAI/.github.git

# 4. Push
git push -u origin main

# 5. Visit github.com/AethyrionAI to see it live!
```

---

## ✅ Pre-Push Checklist

Update these in `profile/README.md` before pushing:

- [ ] Discord invite link: `https://discord.gg/aethyrion` → your actual link
- [ ] Twitter handle: `https://twitter.com/aethyrionai` → your actual handle
- [ ] Support email: `support@aethyrion.org` → your actual email
- [ ] Conduct email: `conduct@aethyrion.org` → your actual email

---

## 📋 First Day Tasks

### 1. Create Empty Repos (5 min each)
For Observatory, Conduit, Spectra:
```
1. Go to github.com/orgs/AethyrionAI/repositories
2. Click "New repository"
3. Name it (e.g., "Observatory")
4. Set to Public
5. Add description: "Self-hosted observability platform - free alternative to Datadog"
6. Initialize with README (you'll replace it later)
7. Create repository
```

### 2. Pin Repositories (2 min)
```
1. Go to github.com/AethyrionAI
2. Click "Customize your pins"
3. Select: Helix, Prism, Observatory, Conduit, Spectra
4. Arrange in that order
5. Save
```

### 3. Add Topics to Each Repo (3 min per repo)
```
Repo → About section (top right) → ⚙️ gear icon

Suggested topics:
- developer-tools
- free-alternative
- open-source
- [specific tech: react, typescript, electron]
- [category: code-generation, observability, api-testing]
```

---

## 🎨 Files You Have

| File | Purpose | Action Needed |
|------|---------|---------------|
| `.github/profile/README.md` | **Organization profile** | Update social links, then push |
| `SETUP_INSTRUCTIONS.md` | Detailed setup guide | Read for full context |
| `REPO_README_TEMPLATE.md` | Template for repo READMEs | Customize per repo |
| `CONTRIBUTING.md` | Contributor guidelines | Copy to each repo |
| `CODE_OF_CONDUCT.md` | Community standards | Copy to each repo |
| `README_START_HERE.md` | Comprehensive overview | Read for strategy |

---

## 🔧 Common Commands

### Update Profile After Changes
```bash
cd O:\GithubPages\.github
git add .
git commit -m "Update organization profile"
git push
```

### Create New Repo with Templates
```bash
# After creating repo on GitHub
git clone https://github.com/AethyrionAI/NewRepo.git
cd NewRepo

# Copy templates
cp O:\GithubPages\REPO_README_TEMPLATE.md README.md
cp O:\GithubPages\CONTRIBUTING.md .
cp O:\GithubPages\CODE_OF_CONDUCT.md .

# Edit README.md with your tool details, then:
git add .
git commit -m "Add documentation"
git push
```

---

## 📊 Badge Quick Reference

Copy these into your READMEs and customize:

```markdown
<!-- Status Badge -->
![Status](https://img.shields.io/badge/Status-Live-10b981?style=for-the-badge&labelColor=0f172a)
![Status](https://img.shields.io/badge/Status-Beta-8b5cf6?style=for-the-badge&labelColor=0f172a)
![Status](https://img.shields.io/badge/Status-Coming_Soon-94a3b8?style=for-the-badge&labelColor=0f172a)

<!-- License Badge -->
![License](https://img.shields.io/badge/License-MIT-10b981?style=for-the-badge&labelColor=0f172a)

<!-- Stars Badge (auto-updates) -->
![Stars](https://img.shields.io/github/stars/AethyrionAI/RepoName?style=for-the-badge&labelColor=0f172a&color=f59e0b)

<!-- Tech Stack Badges -->
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)
```

---

## 🎯 Today's Goal

**Get the org profile live and looking professional.**

That means:
1. ✅ Push profile to .github repo
2. ✅ Create placeholder repos for unfinished tools
3. ✅ Pin repositories in correct order
4. ✅ Add topics to all repos

**Time estimate:** 30-45 minutes total

---

## 🆘 Quick Troubleshooting

**Profile not showing?**
- Repo must be named `.github` exactly (with dot)
- Must be public
- File must be at `profile/README.md`
- Wait 5 mins, clear cache, refresh

**Can't push?**
- Make sure repo exists on GitHub first
- Check remote URL: `git remote -v`
- May need to authenticate (use token, not password)

**Badge not working?**
- Check repo name spelling
- Make sure repo is public
- Shields.io might be slow (wait a min)

---

## 💡 Pro Tip

Before you start, have these ready:
- Your GitHub personal access token (for authentication)
- Your Discord server invite link (if you have one)
- Your Twitter handle (if you have one)
- 30 minutes of uninterrupted time

If you don't have Discord/Twitter yet, that's fine! You can update links later. The profile works perfectly without them.

---

## 📞 Need Help?

I'm here! Just ask if you:
- Hit any errors during setup
- Want to customize something differently
- Need help with git commands
- Want to brainstorm next steps

---

<div align="center">

**Let's ship this! 🚀**

*Your organization profile is ready - time to make it live!*

</div>
