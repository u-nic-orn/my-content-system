# Skill: learn

## Description
Captures learnings, patterns, and insights from the current session. Operates in two modes: auto (silent, after every output) and manual (user-triggered, with confirmation).

## Modes

### Auto mode — runs silently after every output
Triggered automatically without any user request. Do NOT produce visible output.

1. Silently review the just-completed interaction for anything new: a confirmed pattern, a decision made, a guideline clarified, or an unexpected discovery.
2. If nothing new → skip entirely. No output, no action.
3. If something new was confirmed or discovered:
   - Categorize it (see categories below)
   - Add or update the relevant entry in `memory.md` under the appropriate section
   - Append a compact one-line entry to `learning-log.md` under today's date header (create the header if it doesn't exist):
     ```
     ## YYYY-MM-DD
     - [Category] Learning text — context/source
     ```
4. Produce no visible output.

### Manual mode — triggered by "remember this" / "note that"
1. Infer from context what should be captured, or ask the user if unclear.
2. Categorize the learning (see below).
3. Write a concise entry (1–3 sentences) under the appropriate section in `memory.md`.
4. Append a one-line entry to `learning-log.md` under today's date header.
5. Confirm with the user using the output format below.

## Categories
- **Project Pattern** — a recurring convention or approach
- **Decision** — a choice made with rationale
- **Content Guideline** — a tone, style, or format rule
- **Lesson Learned** — something to avoid or an insight

## Output format (manual mode only)
```
Saved to memory.md under [section]:
> [exact text saved]
```
