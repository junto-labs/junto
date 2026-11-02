# Junto Community Edition

Junto is a trust-first platform for work that humans and agents share, with a verifiable record of who did what and under whose authority. The Community Edition is free to use under the [Junto Community Edition License](LICENSE). Junto's source is private; this repo holds releases, the Claude Code plugin marketplace and issues.

More at [juntolabs.dev](https://juntolabs.dev).

## Knowtorious (`kt`)

Scoped knowledge for people and agents, read from a `.knowtorious/` markdown vault. Agents load only a table of contents at session start and fetch the entries they need, rather than reading knowledge out of `AGENTS.md` or `CLAUDE.md`.

**Install.** Download the archive for your platform from [Releases](https://github.com/junto-labs/junto/releases) (tags `knowtorious-v*`), unpack it, and put `kt` on your `PATH`. Check the download against `checksums.txt`. Each archive includes the licence and a NOTICE file listing third-party licences.

**Claude Code plugin.** With `kt` on your `PATH`:

```
/plugin marketplace add junto-labs/junto
/plugin install knowtorious@junto
```

The plugin adds a session-start table of contents (entry ids and titles, never content) and an MCP server with `list`, `get` and `search`. Without `kt` or a vault, it does nothing.

## Issues and feedback

Report bugs and request features in [Issues](https://github.com/junto-labs/junto/issues). For security problems, see [SECURITY.md](https://github.com/junto-labs/.github/blob/main/SECURITY.md) and don't open a public issue.
