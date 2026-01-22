# baiv-test-git-wf

Test repository for GitHub workflow automation before deploying to PF-Core-BAIV.

## Purpose

This repository is used to safely test GitHub Actions workflows that automate:
- Auto-adding issues/PRs to GitHub Projects
- Auto-linking PRs to issues via branch naming
- Creating issues for orphan PRs
- Creating branches from issues

## Test Project

All automation targets: https://github.com/users/ajrmooreuk/projects/22

## Test Plan

See the test plan for validation steps before production deployment.

## Workflows

- `auto-add-to-project.yml` - Adds issues/PRs to Project 22
- `auto-link-issue.yml` - Links PRs to issues via branch name pattern
- `create-issue-for-orphan-pr.yml` - Creates issues for PRs without references
- `create-branch-from-issue.yml` - Creates branches when issues are labeled ready-to-develop
test change
orphan test
