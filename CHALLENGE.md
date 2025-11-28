# CI with GitHub Actions — NestJS Exercise
## Task: Automate Testing & Linting with GitHub Actions
Your goal is to add CI (Continuous Integration) to a NestJS project using GitHub Actions. The CI pipeline should automatically lint, build, and test the app every time someone pushes or opens a pull request.

1. Create a `.github/workflows/ci.yml` file
2. Define a GitHub Action that runs on:

- `push` to `main`
- any pull_request

## ✅ Success Criteria

| Requirement | Complete? |
|-------------|-----------|
| CI workflow runs on push/PR | ✅ |
| Workflow includes lint, build, test steps | ✅ |
| NestJS app runs without errors | ✅ |
| All tests passes | ✅ |

## ⭐ Bonus Challenges (Optional)
- Add a status badge to your README:
```yaml
![CI](https://github.com/<your-username>/<repo-name>/actions/workflows/ci.yml/badge.svg)
```
- Add caching to speed up builds:
```yaml
- name: Cache Node modules
  uses: actions/cache@v3
  with:
    path: ~/.npm
    key: $-node-$
```