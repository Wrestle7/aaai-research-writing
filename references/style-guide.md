# Distilled AAAI Research Writing Guide

## Source basis

This guide synthesizes public AAAI papers from Peng Cui's research group:

1. *Stable Learning via Sample Reweighting* (AAAI 2020).
2. *Stable Adversarial Learning under Distributional Shifts* (AAAI 2021).
3. *Stable Learning via Sparse Variable Independence* (AAAI 2023).
4. *Covariate-Shift Generalization via Random Sample Weighting* (AAAI 2023).

The synthesis concerns recurring scholarly conventions, not an attempt to reproduce any author's voice.

## Expression DNA

### Rhetorical posture

- Formal, restrained, and mechanism-first.
- Problems are introduced as an assumption mismatch in a realistic setting.
- Claims are scoped by assumptions, data regime, or evaluation setting.
- A method earns novelty by resolving a named limitation, rather than through superlatives.

### Recurrent argument architecture

`setting → failure mechanism → gap in prior approaches → observation/theory → proposed method → evidence`

Typical transitions:

- `However, ...`
- `In many real applications, ...`
- `The essential problem lies in ...`
- `Motivated by this observation/theoretical finding, ...`
- `To address this problem, we propose ...`
- `Empirical studies/experiments ... validate/demonstrate ...`

Use transitions only when the preceding sentence supplies the premise.

## How each section works

### Abstract

Each source abstract has a compact four-part structure:

1. Problem and concrete instability or limitation.
2. Why the nearest literature fails or requires unavailable conditions.
3. Method name plus operative mechanism.
4. Theory plus empirical validation, both bounded by their scope.

Preferred sequence:

`[Problem] often leads to [failure], especially under [condition]. Existing [family] relies on [requirement] / suffers from [limitation]. We propose [method], which [mechanism]. We show that [bounded theorem claim]. Experiments on [scope] demonstrate [measured conclusion].`

### Introduction

1. Begin with a familiar learning objective or assumption.
2. Show why it becomes fragile in the real application setting.
3. Narrow from the broad topic to the paper's exact shift, bias, or regime.
4. Categorize related work by assumptions and failure mode.
5. Isolate one essential bottleneck and, if helpful, ground it with one example.
6. State the central observation, then introduce the method.
7. Close with contributions ordered as theory, method, experiments.

### Contributions

Write 2–3 parallel bullets. Each bullet begins with an author action and contains a checkable output.

- `We theoretically analyze [phenomenon] and establish [bounded result].`
- `Motivated by the analysis, we propose [method], which [mechanism and target setting].`
- `We conduct extensive experiments on [scope] to validate [claim].`

Avoid mixing three claims in one bullet or claiming `state-of-the-art` without the comparison protocol.

### Method and theory

Use an ideal-to-practical pivot:

`Under [ideal condition], [desired property] holds. However, [why the condition fails in practice]. We therefore introduce [relaxation/design], which [mechanism].`

After each important equation or theorem, write a short interpretation:

`The term [symbol] measures [meaning]. Thus, Theorem X implies that [operational consequence] under [condition].`

### Experimental narrative

Introduce each experiment with its diagnostic purpose, not its dataset name alone.

- `We first evaluate whether [method] can [target behavior] under [controlled regime].`
- `The results show that [qualified observation].`
- `This is consistent with [mechanistic explanation], although [boundary].`

## Micro-style rules

| Prefer | Avoid |
|---|---|
| a named mechanism | generic praise such as `effective`, `powerful`, or `novel` without explanation |
| `may`, `can`, `under ...` | universal claims from a single experiment |
| `we propose/show/construct/characterize` | inflated verbs such as `revolutionize` |
| one technical term used consistently | multiple near-synonyms for the same object |
| explicit contrast between methods | citation lists with no comparison |
| a result followed by its scope | unqualified causal interpretation |

## Revision checks

Before returning revised text, verify:

- Does every paragraph have a single argumentative function?
- Does every `however` identify a real contrast?
- Does the method directly answer the limitation that preceded it?
- Does every theoretical statement retain its conditions?
- Does every empirical claim name its evaluated scope?
- Are claims no stronger than the supplied evidence?
