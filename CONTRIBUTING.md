# Contributing to a Tignex project

Thanks for considering it. This is the organization-wide guide; a repository
that ships its own `CONTRIBUTING.md` overrides it, and its version wins.

Projects under [Tignex](https://tignex.com) keep their own names, licences and
release cadences, so the specifics — build commands, test layout, supported
versions — live in each repository's `README`. What follows is what holds
everywhere.

## Before you write code

**Open an issue first for anything beyond a small fix.** A typo, a broken link
or a one-line bug fix can go straight to a pull request. A new feature, a change
in behaviour, a new dependency or a change to a published format needs a
conversation before it needs an implementation — it is the cheapest point to
find out that the answer is no, or that it should be solved somewhere else.

**Check the project's own limits.** Every project documents what it is
deliberately not — CommitBrief does not gate merges, BabelQueue is not a broker,
QueryProxy is not a bastion host. A proposal that crosses one of those lines is
not rejected for being a bad idea; it is rejected for being a different product.

## Pull requests

- **One concern per pull request.** A refactor bundled with a fix makes both
  harder to review and impossible to revert separately.
- **Describe the behaviour, not the diff.** What changes for someone using the
  project, and why. The diff is already in the pull request.
- **Tests come with the change.** A bug fix gets a test that fails without it; a
  feature gets tests for the path someone will actually take.
- **Match the surrounding code.** Naming, comment density and structure of the
  file you are editing beat any general style preference, including your own.
- **Update the documentation in the same pull request.** A new command, flag,
  environment variable, configuration key or changed behaviour is not done until
  the README, the docs site and the specification say so.
- **Green before review.** Run the project's full check command locally. If the
  repository documents one (`make check`, `npm run check`, `go test ./...`),
  that is the gate, and a red pipeline is a round trip nobody enjoys.

## Commit messages

Write them for the person running `git log` in two years:

```
Short imperative summary, under ~72 characters

Why the change was needed and what it does about it. Wrap at 72.
Reference issues as "Fixes #123" on their own line.
```

No tool signatures, no generated-by trailers, no co-author lines for
automation. If a person co-authored the work, `Co-Authored-By` for that person
is welcome.

## Specifications and published formats

BabelQueue's envelope — and any other format a second implementation could be
written against — is versioned, and a change to it is a specification change
before it is a code change. Propose it as such: what breaks, what the migration
looks like, and which version it lands in. An SDK that quietly accepts a shape
the specification does not describe is a bug in the SDK.

## Licensing of contributions

Each project carries its own licence — `GPL-3.0-or-later` for CommitBrief, `MIT`
for BabelQueue, `AGPL-3.0-only` for QueryProxy, and whatever a given repository's
`LICENSE` file states elsewhere. Opening a pull request means your contribution
is offered under that repository's licence.

## Conduct

The [Code of Conduct](https://github.com/tignex/.github/blob/main/CODE_OF_CONDUCT.md) applies to every space the
organization runs — issues, pull requests, discussions and email.
