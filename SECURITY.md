# Security policy

This is the organization-wide policy for [Tignex](https://tignex.com)
projects. A repository that ships its own `SECURITY.md` overrides it.

## Reporting a vulnerability

**Do not open a public issue.** Report it privately, in either of these ways:

1. **GitHub private vulnerability reporting** — on the affected repository, open
   the *Security* tab and choose *Report a vulnerability*. This is preferred: it
   keeps the report, the fix and the advisory in one place.
2. **Email** — [info@muhammetsafak.com.tr](mailto:info@muhammetsafak.com.tr)
   with `SECURITY` in the subject line.

Please include, as far as you can:

- The project and version affected, and the platform it was running on
- What an attacker gains — the impact, not only the defect
- Steps to reproduce, or a proof of concept
- Any mitigation you already found

## What happens next

| Stage | Target |
|-------|--------|
| Acknowledgement of your report | within 72 hours |
| Initial assessment — confirmed, needs more information, or not a vulnerability | within 7 days |
| Fix released, or a dated plan if it needs longer | within 90 days |

You will be told which way the assessment went, including when the answer is
"this is working as designed" and why. A report that turns out not to be a
vulnerability is still worth the time it took you to write.

## Disclosure

Coordinated disclosure: a fix ships first, then an advisory naming the versions
affected and the upgrade path. Credit goes to the reporter unless you would
rather stay anonymous — say which when you report.

There is no bug bounty programme.

## Scope

**In scope** — anything in the source of a project published by the
organization, its release artefacts and its published specifications. That
includes flaws in default configuration, because a default that is unsafe for
someone who never reads the manual is a defect.

**Out of scope** — findings against the marketing sites that are not exploitable
(missing headers with no demonstrated impact, version disclosure), automated
scanner output with no analysis behind it, vulnerabilities in a dependency
already fixed upstream where the fix is an ordinary version bump, and anything
requiring an attacker who already holds the credentials or host access the
system trusts.

A note on QueryProxy specifically: it sits in front of production databases and
its threat model assumes a hostile submitter but a trusted operator. A finding
that requires operator-level access is usually documented behaviour rather than
a vulnerability — report it anyway if you think the documentation is wrong.

## Supported versions

Security fixes land on the latest released minor of each project. Backports to
an older line are decided case by case; each repository's release documentation
states what it maintains.
