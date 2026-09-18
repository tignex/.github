# .github

Organization-wide defaults for [Tignex](https://tignex.com).

Two things live here, and they are served to different places:

| Path | Where GitHub shows it |
|------|----------------------|
| [`profile/README.md`](profile/README.md) | The organization page at [github.com/tignex](https://github.com/tignex) |
| [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md), [`CONTRIBUTING.md`](CONTRIBUTING.md), [`SECURITY.md`](SECURITY.md), [`SUPPORT.md`](SUPPORT.md) | Every public repository in the organization that does not ship its own copy |
| [`.github/ISSUE_TEMPLATE/`](.github/ISSUE_TEMPLATE), [`.github/PULL_REQUEST_TEMPLATE.md`](.github/PULL_REQUEST_TEMPLATE.md) | The issue and pull request forms of repositories without their own templates |

A repository that publishes its own version of any of these wins — the files
here are the floor, not a ceiling. Projects with a different licence, threat
model or release cadence are expected to override them.

## Editing

Changes here are visible on the public organization page and inherited by every
repository in the organization, so treat a change as a publish rather than a
commit:

- Relative links break outside this repository. Anything a health file links to
  must be an absolute URL, because the file is rendered in the context of the
  repository that inherits it, not this one.
- The images in `profile/assets/` are referenced by absolute `raw.githubusercontent.com`
  URL for the same reason; renaming one breaks the organization page.
- Project claims — supported providers, languages, brokers, licences — mirror
  each project's own documentation. When a project changes, the profile page is
  not the source of truth; fix it there first, then here.

## Licence

[MIT](LICENSE) — deliberately permissive, because the templates here are meant
to be copied. Take what is useful into your own organization; the projects
themselves carry their own licences.
