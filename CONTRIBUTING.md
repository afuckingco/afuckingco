```console
┌──(test㉿afuckingco)-[~]
└─$ cat CONTRIBUTING.md
```

# Contributing Guidelines

> Thank you for considering contributing! This guide applies across all repositories under this account, including monorepos that bundle multiple subprojects in different languages.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ git log --before-you-start
```

- Check [existing issues](../../issues) to avoid duplicate work.
- For major changes, open an issue first to discuss what you'd like to change.
- If this repo is a **consolidated monorepo** (contains multiple subdirectories, each a separate project), scope your PR to a single subproject unless the change is repo-wide (e.g. CI config, README).

---

```console
┌──(test㉿afuckingco)-[~]
└─$ git checkout -b feat/your-feature
```

## How to contribute

1. Fork the repository.
2. Create a feature branch from `main`:
```bash
   git checkout -b feat/your-feature
```
   Or, for monorepos, scope the branch name to the subproject:
```bash
   git checkout -b feat/<subproject>/your-feature
```
3. Set up your local environment according to the subproject's own README (each subproject/repo specifies its own language and toolchain — see below).
4. Make your changes, following the code style for that project's language.
5. Write or update tests for your changes.
6. Ensure all checks pass locally (see Code Style below).
7. Write clear, descriptive commit messages (see Commit Messages below).
8. Push your branch and open a Pull Request targeting `main`.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ lint --check-all-languages
```

## Code style

<div align="center">

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![Go](https://img.shields.io/badge/Go-00add8?style=flat&logo=go&logoColor=white)
![Rust](https://img.shields.io/badge/Rust-B7410E?style=flat&logo=rust&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

</div>

This account maintains projects across several languages. Apply the relevant tooling for the language you're touching:

| Language | Format | Lint | Test |
|---|---|---|---|
| Python | `black --check .` | `flake8 .` | `pytest -v` |
| Go | `gofmt -l .` | `go vet ./...` | `go test ./...` |
| Rust | `cargo fmt --check` | `cargo clippy` | `cargo test` |
| JavaScript / TypeScript | `npx prettier --check .` | `npx eslint .` | `npm test` |

> Run the formatter and linter for your language **before committing**. CI will reject PRs that fail either check.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ git commit -m "feat: describe your change"
```

## Commit messages

All repos follow [Conventional Commits](https://www.conventionalcommits.org/):

```text
feat: add new anomaly detection endpoint
fix: correct off-by-one error in log parser
docs: update installation instructions
chore: bump dependency versions
refactor: simplify token validation logic
test: add coverage for edge cases in parser
```

For monorepos, optionally scope the type:
```text
feat(sift): add entropy threshold config option
fix(dockguard): correct false positive on multi-stage builds
```

---

```console
┌──(test㉿afuckingco)-[~]
└─$ pytest -v --check-coverage
```

## Testing

Run the test suite for the language/subproject you changed (see table above). New features should include corresponding tests. Bug fixes should include a regression test where practical.

---

## ✅ Pull Request Checklist

- [ ] Code passes the formatter and linter for its language
- [ ] Tests pass locally
- [ ] New/changed behavior has test coverage
- [ ] Documentation updated (README, docstrings, comments)
- [ ] Commit messages follow Conventional Commits
- [ ] PR description explains **what** changed and **why**
- [ ] If this is a monorepo, PR is scoped to one subproject (unless repo-wide)

---

```console
┌──(test㉿afuckingco)-[~]
└─$ report --type=security
```

## Reporting Bugs / Security Issues

| Type | Where |
|------|-------|
| Regular bugs | Open a GitHub [issue](../../issues) with clear steps to reproduce |
| Security vulnerabilities | ⚠️ **Do not** open a public issue — see [SECURITY.md](./SECURITY.md) for responsible disclosure |

---

## 🤝 Code of Conduct

> Be respectful and constructive. Harassment or abusive behavior toward maintainers or other contributors will not be tolerated.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ echo $THANKS
```

```text
We appreciate your effort — every contribution, big or small, helps.
Think. Research. Build. Test. Ship. Repeat.
```
