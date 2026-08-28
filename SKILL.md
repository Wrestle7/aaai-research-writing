---
name: aaai-research-writing
description: |
  Revise English AI/ML research-paper prose in the distilled writing style of four AAAI papers from Peng Cui's research group: Stable Learning via Sample Reweighting (2020), Stable Adversarial Learning under Distributional Shifts (2021), Stable Learning via Sparse Variable Independence (2023), and Covariate-Shift Generalization via Random Sample Weighting (2023). Use when drafting or improving an abstract, introduction, contributions, method motivation, experimental narrative, response to reviewers, or title for an AI/ML paper that needs concise problem-driven, claim-evidence writing. Do not use to imitate any individual author or to invent experimental results, theoretical guarantees, or citations.
---

# AAAI Research Writing

Use the reference guide at `references/style-guide.md` before revising substantive prose.

## Core workflow

1. Identify the section's job: abstract, introduction, contributions, method, experiments, or response.
2. Preserve the author's technical claims, scope, notation, citations, and evidence. Do not add facts.
3. Rebuild the paragraph around a logical chain: real setting → specific failure mode → limitation of existing approaches → precise intervention → supported consequence.
4. Make every sentence perform one job. Prefer a concrete mechanism over a broad adjective.
5. Return two parts: revised prose, then a brief `Key edits` list explaining structural changes and flagging unsupported claims.

## Section patterns

### Abstract

Write 5–7 compact moves in this order:

1. Name the problem and its consequence.
2. State why existing methods are inadequate in this setting.
3. Introduce the method with its essential mechanism.
4. State the strongest verified theoretical claim.
5. State the empirical scope and result without exaggeration.

Use `we propose`, `we show`, and `experiments on ... demonstrate/validate`. Name the setting, not just the task.

### Introduction

Start from a practical assumption failure, then narrow to the paper's setting. Group prior work by what it requires or fails to handle; do not merely enumerate citations. Explain the bottleneck causally, use one concrete illustrative example only when it sharpens the distinction, then transition with `Motivated by this observation` or an equivalent evidence-linked bridge.

End with 2–3 contributions. Each item must pair a contribution with its role or evidence: theory, method, or evaluation.

### Method motivation

State the ideal condition first, explain why it is too strict in the finite-data or real-world setting, and relax it with the proposed mechanism. Define notation only when it will be used immediately. Interpret formal results in plain language after the theorem; never restate equations word for word.

### Experiments

Open with the question being tested. Map each dataset or setting to the claim it evaluates. Report directional, qualified takeaways tied to evidence; distinguish observed results from explanations. Do not claim generality beyond the evaluated distribution shifts, tasks, or metrics.

## Language rules

- Prefer active, compact verbs: `assume`, `characterize`, `construct`, `differentiate`, `leverage`, `alleviate`, `validate`.
- Prefer qualified precision: `under appropriate conditions`, `in the finite-sample setting`, `may`, `can`, `is likely to`.
- Replace vague praise (`novel`, `powerful`, `significant`) with mechanism or measured effect.
- Use `however`, `in contrast`, `therefore`, and `motivated by` only for an explicit logical transition.
- Keep acronym introduction to first use and keep terminology stable.
- Use `we` for author actions; use impersonal constructions for established facts when clearer.

## Guardrails

- Do not fabricate citations, theorem conditions, baseline behavior, statistical significance, or numerical improvements.
- Do not turn correlation into causation or an empirical result into a guarantee.
- Do not make the prose sound like a named author. This is a research-writing framework distilled from public papers, not person imitation.
- If source material is missing, write `[evidence needed]` rather than filling the gap.
