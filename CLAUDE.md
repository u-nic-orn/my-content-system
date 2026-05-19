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
├── CLAUDE.md                        # This file — Claude instructions
├── memory.md                        # Persistent memory across sessions
├── learning-log.md                  # Append-only chronological learning log
├── skills/
│   ├── tone-checker.md
│   └── learn.md
└── style-guide/
    ├── voice.md                     # Brand personality and voice chart
    ├── style.md                     # Style rules (abbreviations, formats, UI copy etc.)
    ├── typographical-signs.md       # Correct typographical characters and keyboard shortcuts
    ├── glossary.md                  # Glossary overview and usage guide
    └── master-glossary.csv          # Full term list: de-CH, fr-CH, it-CH, en-GB
```

> **Pending:** `style-guide/voice.md` references `../assets/personality_chart.svg` — image not yet provided.

## Notes for Claude
- Consult `memory.md` at the start of each session for accumulated context
- Check `style-guide/style.md` and `style-guide/master-glossary.csv` before writing or reviewing copy
- Use the `learn` skill to capture new patterns or insights during work
- Use the `tone-checker` skill before finalizing any content
- After every response, check if anything new was confirmed, decided, or discovered. If yes, update `memory.md` and append to `learning-log.md` as part of that same response — do not defer it. If nothing new, skip. (The Stop hook will also prompt this check automatically.)
- After producing any written output or writing suggestions, run the tone-checker skill.
