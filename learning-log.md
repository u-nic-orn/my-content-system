# Learning Log

Append-only chronological log of confirmed patterns, decisions, and discoveries.
Format: `- [Category] Learning text — context/source`
Categories: `Project Pattern`, `Decision`, `Content Guideline`, `Lesson Learned`

---

- [Content Guideline] Italian (it-CH) formal possessives (Lei form) must be capitalised: "il Suo", "i Suoi", "la Sua" — caught in tone-check of AI chat UI strings, 2026-05-13
- [Content Guideline] "Ciao" is informal register in Italian — use "Salve" for greetings when body copy uses formal Lei form — caught in tone-check of MESSAGES.EMPTY_TITLE, 2026-05-13
- [Content Guideline] Italian button labels use informal imperative (tu) or infinitive regardless of overall formal register — consistent with glossary (continua, elimina, modifica, mostra etc.) — confirmed 2026-05-13
- [Content Guideline] "AI" → "l'IA" in running Italian text; "IA di bexio" is the full glossary form — confirmed from master-glossary.csv, 2026-05-13
- [Lesson Learned] The auto-learn step after each output has not been running in practice — user flagged this 2026-05-13; must be applied manually until the skill trigger is reliable
- [Decision] Fixed auto-learn reliability with two changes: (1) Stop hook in `.claude/settings.json` injects a LEARN-CHECK reminder after every response; (2) CLAUDE.md updated to drop "silently" and require logging in the same response, not deferred — 2026-05-13
- [Content Guideline] fr-CH status "pending" = "en suspens" (not "en attente") — confirmed from master-glossary.csv, 2026-05-18
- [Content Guideline] fr-CH status "paid" = "payée" without "déjà" — "déjà" is redundant; use bare past participle — confirmed 2026-05-18
