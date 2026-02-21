Review the code you worked on this session and document your findings in `memory/`.

The user may have provided a domain hint: $ARGUMENTS
If a hint is given (e.g. `SystemPopup`), focus documentation on that domain.
If no hint is given, infer the relevant domain(s) from what you actually worked on.

## Rules

1. **Domain-based files only.** No shared files like `patterns.md` or `gotchas.md`. Each file covers one domain (e.g., `memory/system-popup.md`, `memory/gacha.md`, `memory/combat.md`).

2. **Only document what you actually touched.** If you read it or changed it this session, document it. Don't speculate about code you haven't seen.

3. **File structure:**

```markdown
# [Domain Name]

## Overview
Brief description of the domain (1-2 paragraphs).

## Key Classes
| Class | Role | Notes |
|-------|------|-------|

## Patterns
Reusable patterns found in this domain.

## Gotchas
Pitfalls, surprises, things that will bite you.
```

Omit empty sections. Keep entries concise — use multiple lines only when complexity demands it.

4. **Update `memory/INDEX.md`** — add or update the entry for each file you created or changed. One file per row, one-line description.

5. **Correct, don't accumulate.** If feedback or new findings contradict existing entries, update them in place. Don't append conflicting information.

6. **Create new files** for new domains. **Update existing files** when you learn more about a documented domain.
