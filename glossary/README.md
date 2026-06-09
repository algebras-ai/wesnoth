# Wesnoth Translation Glossary

## Format

**`concepts.tsv`** — Language-agnostic term definitions.
Columns: `id | term | definition | domain | notes`

**`terms/<lang>.tsv`** — Translations per language (one file per locale code).
Columns: `term_id | term | canonical_translation | notes | confidence`

- `confidence`: `high` / `medium` / `low`
- `notes`: flag inconsistencies, forbidden alternatives, regional variants, or empty if clean

## Domains
- `faction` — Playable faction names (multiplayer + campaigns)
- `race` — Unit race categories
- `alignment` — Lawful / Neutral / Chaotic / Liminal
- `time_of_day` — The six time-of-day phases
- `mechanics` — Core gameplay terms (village, gold, ZoC, etc.)
- `ability` — Unit special abilities
- `terrain` — Map terrain types

## Rules
- Proper names that are untranslatable (Wesnoth, Weldyn, Wesmere, Knalga, character names) are NOT in this glossary — leave them as-is in translations.
- Faction names should be translated consistently across all domains.
- Ability names appear in unit descriptions; use the same form in all domains.
- Time-of-day names must not be confused with common words (e.g. "Morning" ≠ "warning/alert").
