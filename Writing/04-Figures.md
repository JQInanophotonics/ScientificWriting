# 04 — Figures construct the argument

"Let the data speak for themselves" is wrong. Data do not speak.

A figure creates meaning through selection, comparison, organization, annotation, and visual hierarchy. It tells a story that the data alone cannot.

Each figure should answer one necessary question, with panels in a logical order. The figure presents the evidence. The text states what it demonstrates and why it matters.

The abstract, figures, and captions should be enough to follow the main argument.

## Make the evidence progress naturally

Arrange the figures according to the questions a skeptical reader will ask. Do not arrange them according to the order in which the experiments were performed.

A common progression is:

> **Concept, mechanism, experimental proof, control, performance, application.**

This is not a formula. Every figure should establish something required by the next one. If two can be exchanged without affecting the argument, their roles may be unclear.

The introduction proposes a resolution. The figures test it. The discussion states what changes if it is accepted.

## Rules

### The set of figures

1. **Figure 1 is the concept.** It is a schematic of the mechanism, and it often draws the conventional approach next to the new one, so the reader sees the perturbation of the introduction.
2. **One figure per Results section, with the same words.** The figure title and the section title, or its first sentence, name the same result.
3. **The experimental setup is panel a of the figure that uses it, and it is simplified.** Only the parts the result needs are drawn; the full setup goes to Methods or the Supplementary.
4. **A color, marker or line style keeps the same meaning in every figure.** Measured data are markers, simulations and theory are lines.

### The caption

5. **The bold title states the message of the figure,** not the type of plot.
6. **Each panel starts with its bold letter, then what is plotted.**
7. **The caption defines every color, marker and line style,** in parentheses next to what they show.
8. **The caption gives the conditions needed to read the panel:** pump frequencies, mode numbers, simulation parameters.
9. **A panel ends with what it shows or confirms** when that is not obvious from the plot.

How a figure looks (fonts, line widths, colors, export) is covered in [ScientificGraphicDesign](https://github.com/JQInanophotonics/ScientificGraphicDesign).

## In published papers

**Figure 1 as the concept, with the conventional approach next to the new one (rule 1).**

| Paper | Figure 1 |
|---|---|
| All-optical noise quenching, Optica 2025 | "DKS thermo-refractive noise and its circumvention through Kerr-induced synchronization (KIS)": **(a)** single pump scenario, then KIS |
| Dynamic tuning of soliton microcomb repetition rate, Opt. Lett. 2025 | "Kerr-induced synchronization for dynamic comb repetition rate tuning": **a** typical approach for repetition rate tuning, **b** dynamic-KIS |
| DKS self-balancing, PRA 2026 | "Soliton self-balancing mechanism through spectral energy redistribution under Kerr-induced synchronization": **a** single-pump DKS, **b** KIS regime |

**One figure per Results section, with the same words (rule 2).** DKS self-balancing, PRA 2026:

| Results section | Figure title |
|---|---|
| Self-balancing in purely quadratic dispersion resonators | Self-balancing in a pure quadratic integrated dispersion microresonator. |
| Self-balancing effect in presence of a dispersive wave | Demonstration of self-balancing effect in the presence of a single DW. |
| Dispersive wave enhancement with quartic dispersion | Numerical demonstration of DW power enhancement due to self-balancing. |

In the self-aligned PDCS paper (Nature 2026), the section "Self-aligned PDCS metrology: microwave to optical link and vice versa" has two figures, "Microwave-to-optical link: …" and "Optical-to-microwave link: …".

**The setup as panel a (rule 3).**

> **a** Simplified experimental setup for optical frequency synthesis using a self-aligned PDCS microcomb.
>
> — Self-aligned PDCS, Nature 2026, Fig. 4

**A bold title that states the message (rule 5).**

> **Wafer-scale self-aligned PDCS yield and active thermal tuning**
>
> — Self-aligned PDCS, Nature 2026, Fig. 3

Not "Optical spectra of ten devices".

**Markers, lines and colors defined in the caption, and kept across figures (rules 4 and 7).**

> OPO frequency mismatch $\Delta\nu$ (circles: measured, solid line: simulation) […] PDCS integrated dispersion $D_{\mathrm{int}}(n-n_0)$ (squares: measured, dashed line: simulation)
>
> — Self-aligned PDCS, Nature 2026, Fig. 2a

In DKS self-balancing (PRA 2026), blue is "with KIS" and purple is "without KIS" in Figs. 2, 3 and 4.

**The panel ends with what it confirms (rule 9).**

> For 10 devices sampled across the wafer with purposely different coupler designs, […] the corresponding self-aligned PDCS optical spectrum is shown alongside the repetition rate variation against $\delta\nu_-$ (inset), confirming self-alignment and robustness against coupling variations, thickness variations, and wafer-scale fabrication imperfections […]
>
> — Self-aligned PDCS, Nature 2026, Fig. 3a
