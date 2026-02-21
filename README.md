# claude-codebase-memory

A template for Claude Code to accumulate codebase knowledge per domain across sessions.

## What This Does

- **`/document`** slash command — run after a work session to capture what you learned
- **`memory/INDEX.md`** — index of all documented systems, loaded at session start
- **Domain files** (`memory/*.md`) — one file per system/domain, selectively loaded when relevant

## Setup

Copy the files into your project:

```bash
# Option 1: Copy directly
cp -r CLAUDE.md .claude/ memory/ /path/to/your/project/

# Option 2: Git submodule
cd /path/to/your/project
git submodule add https://github.com/yulcat/claude-codebase-memory.git
# Then copy or symlink the files you need
```

If your project already has a `CLAUDE.md`, append the contents from this template's `CLAUDE.md` to yours.

## Usage

1. Work on your project as usual with Claude Code
2. When done, run `/document`
3. Claude reviews what it touched and writes/updates domain files in `memory/`
4. Next session, Claude reads `INDEX.md` and loads only what's relevant

## File Structure

```
memory/
├── INDEX.md          # File → description mapping
├── combat.md         # Example: combat system docs
├── gacha.md          # Example: gacha system docs
└── auth.md           # Example: auth system docs
```

Each domain file follows a consistent structure: Overview, Key Classes, Patterns, and Gotchas.

## License

MIT
