# 🚀 Quick Commands Reference

Essential commands for managing your Automate repository.

## 📦 Development

```bash
# Install dependencies
pnpm install

# Start development mode (hot reload)
pnpm dev

# Build for production
pnpm build

# Type checking
pnpm type-check

# Linting
pnpm lint

# Format code
pnpm prettier

# Run tests
pnpm test
pnpm -F chrome-extension test  # Specific workspace

# E2E tests
pnpm e2e

# Create distribution zip
pnpm zip

# Clean build artifacts
pnpm clean
pnpm clean:bundle        # Just build outputs
pnpm clean:install       # Full clean + reinstall
```

## 🔄 Git Workflow

```bash
# Create feature branch
git checkout -b feature/amazing-feature

# Stage changes
git add .

# Commit with conventional commit format
git commit -m "feat: add amazing new feature"
git commit -m "fix: resolve issue with navigation"
git commit -m "docs: update user guide"

# Push branch
git push -u origin feature/amazing-feature

# Update from main
git checkout main
git pull
git checkout feature/amazing-feature
git merge main

# Squash commits (interactive rebase)
git rebase -i HEAD~3
```

## 🏷️ Release Process

```bash
# Update version in package.json files
pnpm update-version

# Commit version bump
git add .
git commit -m "chore: bump version to 0.2.0"

# Create and push tag
git tag -a v0.2.0 -m "Release v0.2.0"
git push origin v0.2.0

# GitHub Actions will automatically:
# - Build extension
# - Create release
# - Upload distribution zip
```

## 📊 Repository Management

```bash
# View repository info
gh repo view

# List issues
gh issue list

# Create new issue
gh issue create

# List pull requests
gh pr list

# Create pull request
gh pr create --title "Add feature" --body "Description"

# View CI/CD status
gh run list
gh run view [run-id]

# Create release manually
gh release create v0.2.0 dist-zip/*.zip --title "Release 0.2.0" --notes "Release notes"
```

## 🏗️ Workspace Commands

```bash
# List all workspaces
pnpm -r list

# Run command in specific workspace
pnpm -F chrome-extension build
pnpm -F pages/side-panel dev
pnpm -F packages/ui lint

# Run command in all workspaces
pnpm -r build
pnpm -r test
```

## 🐛 Debugging

```bash
# Check extension in Chrome
# 1. chrome://extensions/
# 2. Enable Developer mode
# 3. Load unpacked from dist/

# View logs
# Open side panel → F12 → Console

# Check background service worker
# chrome://extensions/ → Inspect views: service worker

# Reload extension
# chrome://extensions/ → Reload button
```

## 📝 Documentation

```bash
# Generate API docs (if configured)
pnpm docs:generate

# Serve docs locally (if configured)
pnpm docs:serve

# Update changelog
# Edit CHANGELOG.md manually following Keep a Changelog format
```

## 🔍 Useful Git Commands

```bash
# View commit history
git log --oneline --graph --all

# Find specific commit
git log --grep="keyword"

# Show changes in a file
git log -p filename

# Blame (see who changed what)
git blame filename

# Cherry-pick a commit
git cherry-pick <commit-hash>

# Stash changes
git stash
git stash pop
git stash list

# Revert commit
git revert <commit-hash>

# Reset (careful!)
git reset --soft HEAD~1   # Keep changes
git reset --hard HEAD~1   # Discard changes
```

## 🎯 GitHub CLI Shortcuts

```bash
# View repository on GitHub
gh repo view --web

# Open issue in browser
gh issue view 123 --web

# Open PR in browser
gh pr view 456 --web

# Check out PR locally
gh pr checkout 456

# Merge PR
gh pr merge 456 --squash

# Create discussion
gh discussion create --title "Topic"

# View workflows
gh workflow list
gh workflow view ci.yml
```

## 📈 Analytics & Monitoring

```bash
# GitHub traffic stats
gh api repos/:owner/:repo/traffic/views

# Clone stats
gh api repos/:owner/:repo/traffic/clones

# Popular content
gh api repos/:owner/:repo/traffic/popular/paths

# Referrers
gh api repos/:owner/:repo/traffic/popular/referrers
```

## 🔐 Security

```bash
# Check for security vulnerabilities
pnpm audit

# Fix vulnerabilities
pnpm audit --fix

# Update dependencies
pnpm update

# Check outdated packages
pnpm outdated
```

## 💡 Tips

- Use conventional commits: `feat:`, `fix:`, `docs:`, `chore:`, etc.
- Run `pnpm type-check && pnpm lint` before committing
- Test extension build before releasing
- Keep commits atomic and focused
- Write descriptive commit messages
- Review changes before pushing: `git diff`

## 📚 More Info

- [pnpm documentation](https://pnpm.io)
- [GitHub CLI manual](https://cli.github.com/manual/)
- [Git documentation](https://git-scm.com/doc)
- [Conventional Commits](https://www.conventionalcommits.org)

---

**Save this file for quick reference!** 🔖
