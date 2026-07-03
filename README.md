# vortim-claude-marketplace

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) maintained by **Vortim**.

The manifest lives at [`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json).

## Plugins

| Plugin | Description |
|--------|-------------|
| [`game-sounds`](https://github.com/Vortim/game-sounds) | 552 game sound effects for Claude Code — 63 packs (Warcraft, StarCraft, Batman, Matrix, Mega Man & more). |

## Install

### Inside Claude Code

```
/plugin marketplace add Vortim/vortim-claude-marketplace
/plugin install game-sounds@vortim
```

Then restart Claude Code.

### Terminal CLI

```bash
claude plugin marketplace add Vortim/vortim-claude-marketplace
claude plugin install game-sounds@vortim
```

> If the repos are private, add the marketplace over SSH instead so git uses your key:
> ```bash
> claude plugin marketplace add git@github.com:Vortim/vortim-claude-marketplace.git
> ```

## Updating

Bump the plugin `version` in `.claude-plugin/marketplace.json` when you cut a new
`game-sounds` release (or drop the `version` field to always track the latest commit
on its default branch), then run:

```bash
claude plugin marketplace update vortim
```
