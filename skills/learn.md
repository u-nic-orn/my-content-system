# Skill: learn

## Description
Captures learnings, patterns, and insights from the current session and saves them to `memory.md` for future reference.

## Trigger
Use this skill when:
- A recurring pattern is confirmed
- A decision is made that should persist
- Something unexpected is discovered that's worth remembering
- The user says "remember this" or "note that"

## Instructions
1. Ask the user (or infer from context) what should be captured
2. Categorize the learning into one of:
   - **Project Pattern** — a recurring convention or approach
   - **Decision** — a choice made with rationale
   - **Content Guideline** — a tone, style, or format rule
   - **Lesson Learned** — something to avoid or an insight
3. Write a concise entry (1–3 sentences) under the appropriate section in `memory.md`
4. Confirm with the user what was saved

## Output Format
After saving, reply:
```
Saved to memory.md under [section]:
> [exact text saved]
```
