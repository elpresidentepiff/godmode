# GodMode — Project Fleet Command Centre

A personal command-centre dashboard and MCP server built on top of [God's Eye View](https://github.com/bilawalsidhu/gods-eye-view) — the #1 GitHub Trending 3D globe MCP server.

GodMode extends the globe into a **live project fleet monitor** for Carlos's active projects: ML pipelines, AI companions, facilities systems, and learning games — all visible on one surface.

## What It Does

- **3D Globe** powered by God's Eye View, with project nodes pinned to their geographic/logical home
- **MCP Server** exposing tools to query project health, run status, and next actions
- **Live Fleet Status** per project: pipeline state, open PRs, Railway deploy health, Supabase row counts
- **Extensible** — add new projects via `godmode.config.json`, new tools via `tools/`

## Active Projects

| Project | Stack | Status |
|---|---|---|
| Velo Oracle Prime | Railway + Supabase, GBM/NB | Daily scoring live |
| Continuity Companion | Private repo, Supabase | PRs pending merge |
| UCM Agent | Supabase + Jobber | Mission Control live |
| Sovereign AI | Phase 1 repo | Pre-deploy |
| Level/Levelup | Learning game | World 1 active |

## Quick Start

```bash
npm install
npm run dev        # start the God's Eye View globe + GodMode overlay
npm run mcp        # start the MCP server
```

## Configuration

Edit `godmode.config.json` to add or update projects. Each entry drives both the globe pin and the MCP tool surface.

## Tools

See `TOOLS.md` for the full catalogue of new MCP tools and skills discovered for this stack.

## Architecture

```
godmode/
  godmode.config.json     # project fleet definition
  projects/               # per-project JSON state
  tools/                  # MCP tool implementations
  src/                    # globe overlay + dashboard UI
```

Built on [God's Eye View](https://github.com/bilawalsidhu/gods-eye-view) (MIT licence).
