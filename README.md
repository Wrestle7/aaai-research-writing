# AAAI Research Writing Skill

A private Codex Skill for revising English AI/ML research-paper prose in a concise, problem-driven, claim--evidence style distilled from selected AAAI papers.

## What it does

- Revises abstracts, introductions, contribution statements, method motivation, experimental narratives, titles, and reviewer responses.
- Preserves technical claims, notation, citations, formulas, and empirical scope.
- Organizes prose around a clear logical chain: setting, failure mode, limitation, intervention, and evidence.
- Flags unsupported claims instead of inventing results or citations.

## Repository structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── style-guide.md
```

## Installation

Clone this private repository into a local Skill root configured for Codex, or copy the repository directory there without changing its internal structure.

```bash
git clone <private-repository-url> aaai-research-writing
```

Restart or refresh the Codex session after installation so the Skill catalog is reloaded.

## Example prompts

```text
$aaai-research-writing Revise this abstract while preserving all numerical results.
```

```text
Use the AAAI research-writing skill to improve this experiments section. Keep every LaTeX formula, citation key, label, and reference unchanged.
```

## Guardrails

- Do not fabricate citations, numerical improvements, theorem conditions, or statistical significance.
- Do not reproduce the voice of a named author.
- Do not commit source-paper PDFs, API keys, access tokens, private manuscripts, or patient data to this repository.

## Source note

The Skill contains a high-level synthesis of recurring scholarly conventions. It does not include or redistribute the full text of the source papers. See [NOTICE.md](NOTICE.md).
