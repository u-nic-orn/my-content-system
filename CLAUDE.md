# my-content-system

## Project Overview
A content management and creation system. This file provides Claude with project-level context, conventions, and commands.

## Conventions
- All content files are written in Markdown
- Tone should be clear, concise, and professional unless otherwise specified
- Use sentence case for headings
- Skills are defined in `skills/` and follow the standard skill format

## Key Commands
<!-- Add commonly used commands here -->
- `git status` — check working tree
- `git log --oneline` — review commit history

## Project Structure
```
my-content-system/
├── CLAUDE.md       # This file — Claude instructions
├── memory.md       # Persistent memory across sessions
└── skills/
    ├── tone-checker.md
    └── learn.md
```

## Notes for Claude
- Consult `memory.md` at the start of each session for accumulated context
- Use the `learn` skill to capture new patterns or insights during work
- Use the `tone-checker` skill before finalizing any content
