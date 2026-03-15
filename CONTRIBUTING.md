# Contributing Guidelines

## Commit Convention

This project follows [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <description>

[optional body]

[optional footer]
```

### Types

| Type | Description |
|------|-------------|
| `feat` | New feature |
| `fix` | Bug fix |
| `docs` | Documentation only |
| `refactor` | Code change without fix or feature |
| `chore` | Maintenance, deps, CI changes |
| `infra` | Infrastructure / platform change |
| `perf` | Performance improvement |
| `revert` | Revert a previous commit |

### Examples

```
feat(helm): add resource limits to all deployments
fix(postgres): correct replication lag threshold in alerts
infra(k8s): upgrade cluster to 1.30
docs(runbook): add backup restore procedure
```

## Branching Strategy

| Branch | Purpose |
|--------|---------|
| `main` | Production-ready code |
| `develop` | Integration branch |
| `feat/<name>` | New features |
| `fix/<name>` | Bug fixes |
| `infra/<name>` | Infrastructure changes |

## Pull Requests

- Keep PRs focused — one logical change per PR
- Reference the related issue in the PR description
- Ensure CI passes before requesting review
- Squash commits when merging feature branches

## Code Review

- Be constructive and specific
- Approve only when all checklist items are satisfied
- Use `[nit]` prefix for non-blocking style suggestions
