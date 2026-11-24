<!--
Title: Conventional Commits, it becomes the squash commit.
  <type>(<scope>)?: <description>   e.g. feat(api): add invoice export
  types: feat fix docs chore ci refactor test build perf style revert
  Breaking change: add ! after the type and explain it below.
-->

## Summary

<!-- What changes and why. One logical change. -->

## Test plan

<!-- Commands run and results; say what was not tested. Never leave it empty. -->

## Checklist

<!-- Tick only when true. Link evidence when it exists (CI run, scan, screenshot, PR). If an item doesn't apply, tick it and add n/a with a reason. -->

- [ ] Commits are signed.
- [ ] No secrets, keys or tokens (point to where they live instead).
- [ ] No real personal data in code, fixtures, logs or screenshots: synthetic data only.
- [ ] New or changed workflows: a shared reusable workflow was considered first; if this one stays in the repo, the reason is below.
- [ ] Docs updated if behaviour or setup changed.

## After merge

<!-- Manual steps for someone else, each linked to its page. Delete this section when there are none. -->

Refs #<issue> / Closes #<issue>
