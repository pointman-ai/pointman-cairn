# cairn

A Pointman agent profile: **Cairn**, a project manager. Cairn turns asks into epics and tasks with owners and
real dates, closes them with evidence, and says plainly what's left.

```
pointman add cairn                 # on the machine its agents run on
/spawn cairn --profile cairn       # in any thread: makes @cairn
/spawn pm2 --profile cairn         # another agent like it
/spawn pm3 codex --profile cairn   # on Codex CLI instead of its default, Claude Code
```

## What's in it

| File | What |
|---|---|
| `extension.toml` | The manifest: `[agent]` (clients, model, description, face, wakes) and its dependencies |
| `AGENT.md` | The persona: the board's shape, closing with evidence, how it works and writes. The node adds it to each of its agents' runs |
| `avatar.webp` | Its face on the board |
| `memory/` | Starting notes, copied once into each agent's own memory: the board's shape, closing with evidence, sweeping, dating from pace, tool quirks |

Cairn uses only Pointman's own project tools, so it runs on Claude Code, Codex CLI or Gemini CLI.

## What it needs

Nothing: with no extensions it runs Pointman's native projects. Each of these is optional.

| Extension | | Why |
|---|---|---|
| `linear` | optional | Projects connected to Linear teams and projects |
| `github` | optional | GitHub Projects boards, and evidence: a commit that says `Fixes <ref>` moves its item |
| `spacesheep` | optional | Plans and roadmaps as pages |

**Permission rules:** none. **Wakes:** it introduces itself in `#projects`, and sweeps the open items at 07:00
on weekdays.

## Releasing

Bump `version` in `extension.toml`, then publish a GitHub release tagged with it (`v0.1.0`). Core fetches the
tag's files and packs them; nothing is built.
