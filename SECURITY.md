```console
┌──(test㉿afuckingco)-[~]
└─$ cat SECURITY.md
```

# Security Policy

> Responsible disclosure keeps everyone safe. If you've found a vulnerability, thank you — please report it privately so it can be fixed before it's public.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ gh api repos/:owner/:repo --jq .supported_versions
```

## Supported Versions

| Version / Branch | Supported |
|---|---|
| `main` (latest) | ✅ |
| Older tagged releases | ⚠️ Best-effort only |
| Archived / deprecated repos | ❌ Not maintained |

> For consolidated monorepos, this policy applies to each subproject's `main`-tracked code.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ report --vulnerability --private
```

## Reporting a Vulnerability

**Do not open a public GitHub issue for security vulnerabilities.**

Instead, report privately through one of these channels:

1. **Preferred:** [GitHub Security Advisories](../../security/advisories/new) for this repository
2. **Email:** anotherwaltzcompany@gmail.com — include `[SECURITY]` in the subject line

### What to include

- A clear description of the vulnerability
- Steps to reproduce (PoC code or commands if applicable)
- Affected version, commit hash, or subproject (for monorepos)
- Potential impact (what an attacker could do)
- Your suggested fix, if you have one (optional)

---

```console
┌──(test㉿afuckingco)-[~]
└─$ watch --response-timeline
```

## Response Timeline

| Stage | Target |
|---|---|
| Acknowledge report | Within 72 hours |
| Initial assessment | Within 7 days |
| Fix & disclosure coordination | Case-by-case, based on severity |

You will be credited in the fix's release notes / changelog unless you request otherwise.

---

```console
┌──(test㉿afuckingco)-[~]
└─$ echo $SCOPE
```

## Scope

**In scope:**
- Code vulnerabilities in this repository (or, for monorepos, any subproject folder)
- Dependency vulnerabilities introduced by this project's configuration
- CI/CD pipeline security issues

**Out of scope:**
- Vulnerabilities in third-party dependencies themselves (report upstream instead)
- Issues requiring physical access to a user's device
- Social engineering attacks
- Denial-of-service via resource exhaustion on non-production demo instances

---

```console
┌──(test㉿afuckingco)-[~]
└─$ echo $THANKS
```

```text
Security research makes software better for everyone.
Thank you for reporting responsibly.
```
