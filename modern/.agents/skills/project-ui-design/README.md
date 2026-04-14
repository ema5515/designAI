# Project UI Design

This skill was generated automatically from the current repository using Codex CLI.

## Contents

- `SKILL.md` - main skill entrypoint
- `input/` - support files used during analysis
- `outputs/` - generated analysis and final skill documents
- `logs/` - Codex execution logs
- `agents/openai.yaml` - optional skill metadata

## Repository snapshot

- Detected framework hints: Next.js, Tailwind CSS, shadcn/ui, Charts, Radix/Lucide
- Candidate design files found: 89

## What this version improves

- Stronger extraction of radius and spacing as identity traits
- Stronger visual hierarchy and typography-as-UX guidance
- Better interaction-state reasoning
- Conservative inference of missing components such as forms, cards, tables, and dialogs
- Better anti-drift protection when adapting from one UI category to another

## How to refresh the skill

Run the generator script again from the repository root.

## Recommended workflow

1. Regenerate after major UI refactors.
2. Review `outputs/02-design-extraction.md` and `.json`.
3. Fine-tune `SKILL.md` if you want stricter rules for a specific product area.
