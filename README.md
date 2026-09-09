# Branch Protection Demo

This repository demonstrates how GitHub branch protection rules prevent
force-pushes and unreviewed code from reaching the `main` branch.

## Objective

Protect the `main` branch from:
- Direct force-pushes (`git push --force`)
- Merges without at least 1 review approval
- Merges when CI status checks are failing

## Branch Protection Rules (on `main`)

- ✅ Require a pull request before merging
- ✅ Require at least 1 approval before merging
- ✅ Require status checks to pass before merging (`CI` workflow)
- ✅ Do not allow bypassing the above settings (applies to admins too)
- ❌ Force pushes disabled

## CI
