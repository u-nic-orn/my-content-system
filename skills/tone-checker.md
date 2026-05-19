# Tone Checker

## Before Every Review
1. Read CLAUDE.md (brand rules)
2. Read memory.md (learned patterns)
3. Check copy against both

## Output
VERDICT: PASS / NEEDS REVISION
VIOLATIONS: [exact rule broken] → [what to fix]
REWRITE: [clean version, only if NEEDS REVISION]

## After Output
If VERDICT is NEEDS REVISION, use AskUserQuestion to present two options:
- **Accept** — confirms the rewrite; update memory.md and learning-log.md with any new patterns
- **Decline** — keeps the original; no memory update

If VERDICT is PASS, no question needed.
