# Neo-Brutalist Paper

Skill for generating UI with white paper surfaces, heavy black borders, offset shadows, bold hierarchy, and controlled primary-color accents.

## Contents

- `SKILL.md` - main skill entrypoint
- `input/` - support files used during analysis
- `outputs/` - generated analysis and final skill documents
- `logs/` - Codex execution logs
- `agents/openai.yaml` - optional skill metadata

## Repository snapshot

- Detected framework hints: Next.js, Tailwind CSS, shadcn/ui, Charts, Radix/Lucide
- Candidate design files found: 64

## How to refresh the skill

Run the generator script again from the repository root.

## Recommended workflow

1. Regenerate after major UI refactors.
2. Review `outputs/02-design-extraction.md` and `.json`.
3. Fine-tune `SKILL.md` if you want stricter rules for a specific product area.
