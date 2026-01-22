# baiv-test-git-wf

Test repository for GitHub workflow automation before deploying to PF-Core-BAIV.

## Purpose

This repository is used to safely test GitHub Actions workflows that automate:
- Auto-adding issues/PRs to GitHub Projects
- Auto-linking PRs to issues via branch naming
- Creating issues for orphan PRs
- Creating branches from issues

## Documentation

📚 **[Complete Documentation & Installation Guide](./DOCUMENTATION.md)**

Includes:
- Architecture diagrams
- Detailed workflow descriptions
- Step-by-step installation instructions
- Deployment & testing procedures
- Troubleshooting guide
- Security considerations

## Quick Links

- **Test Project Board:** https://github.com/users/ajrmooreuk/projects/22
- **GitHub Actions:** https://github.com/ajrmooreuk/baiv-test-git-wf/actions

## Workflows

| Workflow | Status | Purpose |
|----------|--------|----------|
| `auto-add-to-project.yml` | ✅ Tested | Adds issues/PRs to Project 22 |
| `auto-link-issue.yml` | ✅ Tested | Links PRs to issues via branch name pattern |
| `create-issue-for-orphan-pr.yml` | ✅ Tested | Creates issues for PRs without references |
| `create-branch-from-issue.yml` | ✅ Tested | Creates branches when issues are labeled `ready-to-develop` |

## Quick Start

### For Developers

1. **Create an issue** for your work
2. **Add label** `ready-to-develop` → branch created automatically
3. **Checkout branch** and make changes
4. **Push and create PR** → automatically linked to issue and added to project

### Branch Naming Convention

```
issue-{number}-{description}
```

Examples:
- `issue-42-fix-login-bug`
- `issue-123-add-user-profile`

## Testing Status

All workflows have been successfully tested:

- ✅ Auto-add to Project - Issues/PRs automatically added to project board
- ✅ Auto-link PR to Issue - PRs with `issue-X` branches linked correctly
- ✅ Create Issue for Orphan PR - Orphan PRs get auto-generated issues
- ✅ Create Branch from Issue - Branches created from labeled issues

## Next Steps

1. Review [complete documentation](./DOCUMENTATION.md)
2. Follow migration checklist for production deployment
3. Deploy to PF-Core-BAIV repository
