# Contributing

This guide applies to every repository in the Polinom.io organization that does not have its own `CONTRIBUTING.md`.

## Branches

- `main` is the only long-lived branch. Work on a short-lived branch and open a pull request.
- Name branches `<type>/<kebab-slug>`, for example `fix/login-redirect`. Types: `feat`, `fix`, `docs`, `chore`, `ci`, `refactor`, `test`, `build`, `perf`, `style`, `revert`. Other names are rejected.

## Commits and pull requests

- Every commit must be signed. Unsigned commits are rejected on every branch.
- Pull requests are squash-merged: the PR title becomes the commit on `main`, so it must follow [Conventional Commits](https://www.conventionalcommits.org/), for example `feat(api): add invoice export`. Mark breaking changes with `!`.
- A code owner reviews every pull request. Resolve all review threads before merging.
- Force-pushing and rewriting published history are not allowed. To fix a branch, push new commits or open a new branch.

## Security and data

- Never commit secrets, keys or tokens. Reference where they live instead.
- Use synthetic data in code, tests, fixtures, logs and screenshots. Never real personal data.
- Report vulnerabilities privately, as described in [SECURITY.md](SECURITY.md). Do not open public issues for them.

## Workflows

Before adding a GitHub Actions workflow, check the organization's shared reusable workflows. Repositories call them pinned by full commit SHA instead of copying them. Starter workflows are available under **Actions → New workflow**. If a workflow must stay in the repository, explain why in the pull request.

## Releases

Repositories with release automation version from the Conventional Commits on `main`: merging the release PR creates the tag, the changelog entry and the release.
