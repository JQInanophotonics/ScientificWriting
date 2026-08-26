# Example 1: The introduction is a scenario

## Paper

Grégory Moille *et al.*, [*Self-aligned optical microcomb emerging between
octave separated lasers*](https://arxiv.org/abs/2602.05151), arXiv:2602.05151
(2026). [PDF](https://arxiv.org/pdf/2602.05151) |
[DOI](https://doi.org/10.48550/arXiv.2602.05151)

This example applies **The Introduction Is a Scenario** from the
[main guide](../README.md).

## TL;DR

The introduction follows this sequence. Read the table from top to bottom.

| Order | Scenario element | How it appears in the introduction |
|---:|---|---|
| 1 | **Setting** | Integrated frequency combs promise deployable precision metrology. |
| 2 | **Protagonist** | On-chip comb self-referencing, specifically CEO detection and locking. |
| 3 | **Objective** | Provide a field-deployable optical-to-microwave link. |
| 4 | **Perturbation** | Outward-cascading DKS combs produce weak and noisy octave-spaced signals. |
| 5 | **Stakes** | CEO locking remains confined to complex laboratory demonstrations. |
| 6 | **Proposed resolution** | Generate a self-aligned PDCS between two strong, octave-separated pumps. |
| 7 | **Challenge** | Prove self-alignment, CEO locking, and useful metrology operation. |
| 8 | **Resolution** | A robust, self-referenced on-chip comb that performs the core tasks of frequency metrology. |

The annotated sections below show the sentences used to construct each step.

## Annotated introduction

### Setting: what the field currently accepts

> Chip-integrated DKS combs can span an octave and are compatible with
> mass-scale foundry fabrication and low power consumption.

The accepted approach is to miniaturize the table-top comb architecture: start
from one pump and generate the comb outward.

The paper establishes that this approach is useful before challenging it.

### Protagonist and objective: what is trying to succeed

> Optical frequency combs [...] with evenly spaced markers and a known
> zero-frequency offset [...] provide a coherent optical to microwave two-way
> link for ultra-high precision optical frequency measurement, synthesis, and
> ultra-low noise microwave generation.

> Reducing the size, weight, power, and cost of OFCs through mass-scale
> fabrication can enable field deployment [...]

The protagonist is on-chip comb self-referencing, specifically the ability to
define, detect, and lock the CEO.

Its objective is to provide the complete optical-to-microwave link of a
self-referenced frequency comb in a compact, field-deployable system.

### Perturbation: what the paper contradicts

> However, while DKS combs have proven their effectiveness [...] their outward
> cascading from a low-power seed pump laser leads to fundamental metrology
> limitations.

The paper contradicts the assumption that miniaturizing the conventional
outward-cascading architecture is sufficient for practical on-chip
self-referencing.

The word "However" marks the transition from the established situation to the
problem.

### Stakes: why the contradiction matters

> Octave-spaced signals at the comb edges are typically very weak and noisy
> [...] which critically hinders the detection and stabilization of the CEO.

The introduction connects the architecture to the consequence:

```text
outward cascading
-> weak and noisy octave-spaced signals
-> difficult CEO detection and locking
-> complex laboratory demonstrations
-> no deployable on-chip self-referencing
```

The weak signals matter because they prevent the protagonist from reaching its
objective.

### Proposed resolution: what the paper changes

> Fundamentally departing from conventional comb generation architectures that
> rely on cascading outwards from a single pump [...]

The paper replaces outward generation from one pump with inward generation
between two strong, octave-separated pumps. The resulting PDCS self-aligns with
those pumps.

The proposed resolution acts directly on the architectural cause identified in
the perturbation.

### Challenge: what the paper must prove

> [...] the ability to generate on-chip PDCS combs with two octave-separated
> pumps [...]

> [...] a generated PDCS comb can nonlinearly align itself with the pumps,
> resulting in a single frequency grid [...]

Competent readers can now challenge four points:

1. Do the octave-separated pumps generate the PDCS?
2. Does the PDCS self-align onto one frequency grid?
3. Does this solve the CEO-locking problem?
4. Is the resulting system useful for frequency metrology?

These questions define the evidence that the rest of the paper must provide.

### Resolution: what changes if the evidence is accepted

> The same self-aligned PDCS can perform the three core tasks of self-referenced
> OFCs [...]

The protagonist reaches its objective: the self-aligned PDCS provides robust
on-chip self-referencing and operates as a versatile frequency-metrology tool.

## The writing move

Do not begin by introducing the PDCS.

First establish the accepted route to on-chip self-referencing. Show precisely
why that route prevents robust CEO locking. Only then introduce the self-aligned
PDCS as the necessary change.

This example covers the introduction. The progression of the evidence through
the figures belongs in a separate example.
