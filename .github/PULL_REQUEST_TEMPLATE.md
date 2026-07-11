```console
┌──(test㉿afuckingco)-[~]
└─$ cat PULL_REQUEST_TEMPLATE.md
```

## Summary

> Describe what this PR does in 1-2 sentences.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ git log --related-issue
```

## Related Issue

Closes #(issue number) — or `N/A` if none.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ git diff --changes-made
```

## Changes Made

- 
- 
- 

> For monorepos: which subproject(s) does this touch? `(e.g. sift/, dockguard/)`

---

```console
┌──(test㉿afuckingco)-[~]
└─$ pytest -v --testing-performed
```

## Testing Performed

> How did you verify this works? (unit tests, manual testing, screenshots, etc.)

---

```console
┌──(test㉿afuckingco)-[~]
└─$ checklist --pre-merge
```

## ✅ Checklist

- [ ] Code passes the formatter and linter for its language (see CONTRIBUTING.md)
- [ ] Tests pass locally
- [ ] New/changed behavior has test coverage
- [ ] Documentation updated (README, docstrings, comments)
- [ ] Commit messages follow Conventional Commits
- [ ] PR is scoped to one subproject (if this is a monorepo), unless repo-wide

---

```console
┌──(test㉿afuckingco)-[~]
└─$ echo $NOTES
```

## Additional Notes

> Anything reviewers should know — breaking changes, migration steps, screenshots, etc.
