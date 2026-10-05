<p align="center">
  <img src="https://raw.githubusercontent.com/tignex/.github/main/profile/assets/tignex.png" alt="" width="80" height="80">
</p>

<h1 align="center">Tignex</h1>

<p align="center">
  <em>Open-source tools, infrastructure and standards for developers<br>who value control, interoperability and solid engineering.</em>
</p>

<p align="center">
  <a href="https://tignex.com">tignex.com</a> &nbsp;·&nbsp;
  <a href="https://tignex.com/projects/">Projects</a> &nbsp;·&nbsp;
  <a href="https://tignex.com/engineering/">How we engineer</a> &nbsp;·&nbsp;
  <a href="https://tignex.com/notes/">Notes</a> &nbsp;·&nbsp;
  <a href="https://tignex.com/about/">About</a>
</p>

---

Tignex is an independent open-source organization that develops tools,
infrastructure, protocols, standards, libraries and system components for
developers and software teams. The purpose is software that gives developers
more control, takes interoperability seriously, creates no unnecessary vendor
lock-in, and can be self-hosted when that is what a team needs.

It is not tied to a single product, programming language or technology. What
holds it together is a way of working — transparent behaviour, solid
engineering, a production-oriented bias, and a preference for practical problem
solving over ambitious architecture.

## Projects

Each project keeps its own name, identity, domain and GitHub organization.
Tignex is their shared engineering organization and publisher — the place the
standards, the review habits and the release discipline come from, not a brand
stamped on the front of each one.

### [CommitBrief](https://github.com/CommitBrief) · [commitbrief.com](https://commitbrief.com)

**AI code reviews. Right in your terminal.** A provider-agnostic, local-first Go
CLI that reviews your staged changes, a commit range or a whole GitHub pull
request — before your colleagues do. No server, no account, no telemetry; ten
model providers, including Ollama for reviews that never leave your hardware.

`Go` · `GPL-3.0` · [Docs](https://commitbrief.com/docs/)

### [BabelQueue](https://github.com/BabelQueue) · [babelqueue.com](https://babelqueue.com)

**Polyglot queues, simplified.** One canonical JSON envelope that PHP, Python,
Go, Node.js, Java and .NET produce and consume identically, routed by URN rather
than class name — over the brokers you already run. Not a broker, not a sidecar:
the shape of the message, written down so another language can read it.

`PHP` `Python` `Go` `JavaScript` `Java` `C#` · `MIT` · [Docs](https://babelqueue.com/docs/) · [Specification](https://babelqueue.com/docs/spec/1.x/introduction/)

### [QueryProxy](https://github.com/QueryProxy) · [queryproxy.com](https://queryproxy.com)

**Production data access, without production credentials.** A self-hosted
database access control and query approval system: a developer submits SQL, an
AST parser inspects it, a DBA approves from the web UI or straight from Slack or
Teams, and the result comes back masked and audited. Runs on your own
infrastructure in front of PostgreSQL, MySQL, MariaDB, SQL Server or SQLite.

`PHP` · `AGPL-3.0` · [Docs](https://queryproxy.com/docs/)

## How we engineer

Four commitments every project under the organization is expected to keep,
whether it is a CLI tool, a specification or a piece of server infrastructure.

- **Control stays with you.** Everything is open source and runnable on your own
  machines. Nothing published here is a client for a service we operate, because
  that is the shortest path to a dependency you cannot remove. Self-hosting is
  the first-class path, not a paid tier, and leaving is a supported operation.
- **Interoperable by design.** Open formats and documented protocols over
  convenient private ones, even when the private one would ship sooner. If
  another team cannot write a second implementation from the specification
  alone, the specification is not finished.
- **Production-oriented.** The target is software that survives contact with
  systems that are already running: real data, real load, real migrations, and
  an operator who was not in the room when it was designed.
- **Transparent by default.** Decisions, trade-offs and limits are written down
  where they can be argued with — including the unflattering parts: what a
  project does badly, what it has not solved yet, and what we decided not to do.

Taken seriously, these remove options. No telemetry we would not want pointed at
us. No open-core feature walls in the middle of a protocol. No release that
depends on infrastructure only we can run.

## Contributing

Issues, corrections and pull requests are welcome on any project. Start with the
repository you are reading about; the organization-wide
[contributing guide](https://github.com/tignex/.github/blob/main/CONTRIBUTING.md),
[code of conduct](https://github.com/tignex/.github/blob/main/CODE_OF_CONDUCT.md)
and [security policy](https://github.com/tignex/.github/blob/main/SECURITY.md)
apply everywhere a project does not publish its own.

## Contact

Questions, corrections and contributions are all welcome — write to
[info@muhammetsafak.com](mailto:info@muhammetsafak.com), or open an issue
on the project you are reading about.

---

<p align="center">
  <sub><a href="https://tignex.com">Tignex</a> was founded by <a href="https://muhammetsafak.com/">Muhammet Şafak</a>.</sub>
</p>
