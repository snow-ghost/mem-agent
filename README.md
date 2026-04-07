# mem-agent — LLM-Powered Memory Companion for AI Coding Agents

`mem-agent` captures significant events from your coding sessions, extracts principles, builds skill recipes, and injects context — all powered by an LLM backend.

Works with **Claude Code**, **OpenCode**, and **Codex** out of the box.

> **Note**: This is the LLM-dependent version. For standalone memory management without LLM dependency, see [mem](https://github.com/snow-ghost/mem).

## Install

```bash
go install github.com/snow-ghost/mem-agent/cmd/mem@latest
```

Or download from [Releases](https://github.com/snow-ghost/mem-agent/releases).

## Quick Start

```bash
cd your-project
mem status          # auto-initializes .memory/
mem extract         # capture events (requires LLM backend)
mem consolidate     # synthesize principles
mem inject          # output context for next session
```

## Backends

Auto-detects: `claude` > `opencode` > `codex`. Or set explicitly:

```bash
export MEM_BACKEND=opencode
```

See full docs in the codebase.

## License

MIT
