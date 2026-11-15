<div align="center">

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/header.svg"/><img src="assets/header.svg" width="97%" alt="Scientific Writing"/></picture>

<a href="#pages"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/PAGES-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/PAGES-ffffff?style=flat-square&logoColor=1a1a1a" alt="Pages"/></picture></a>
<a href="https://github.com/JQInanophotonics/ScientificPresentations"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/PRESENTATIONS-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/PRESENTATIONS-ffffff?style=flat-square&logoColor=1a1a1a" alt="Scientific Presentations"/></picture></a>
<a href="https://github.com/JQInanophotonics/ScientificGraphicDesign"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/GRAPHIC%20DESIGN-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/GRAPHIC%20DESIGN-ffffff?style=flat-square&logoColor=1a1a1a" alt="Scientific Graphic Design"/></picture></a>
<a href="https://github.com/JQInanophotonics/ScientificDataManagement"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/DATA%20MANAGEMENT-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/DATA%20MANAGEMENT-ffffff?style=flat-square&logoColor=1a1a1a" alt="Scientific Data Management"/></picture></a>

</div>

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-forewords.svg"/><img src="assets/banner-forewords.svg" width="97%" alt="Forewords"/></picture>

This repository is the group's concise guide to writing a scientific paper.
Each topic has its own page in `Writing/`, numbered in the order a paper is written.
This README summarizes each page and links it. The examples in `Examples/` show
how a rule appears in a real paper, through short excerpts and direct annotations.

<a id="write-only-what-matters"></a>

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-write-only.svg"/><img src="assets/banner-write-only.svg" width="97%" alt="Write Only What Matters"/></picture>

> [!IMPORTANT]
> **Write only what matters.** This is the most important rule of the guide; every page that follows applies it.
>
> **Do not write the history of the project. Write the argument the reader needs.**

The reader does not care how long an experiment took, how difficult it was, or when the result appeared. Effort does not determine scientific importance.

A result belongs in the main text only if it advances the argument or supplies evidence required to support it. Months of work may deserve one sentence or a supplementary figure. A simple control may deserve a central panel if it closes the argument.

Keep only the ideas that carry the story in the main text. Put procedures in the Methods and supporting derivations, controls, and secondary results in the Supplementary Information.

Each paragraph should have one purpose:

> **Claim, evidence or reasoning, interpretation, consequence.**

Remove anything that does not perform one of those jobs.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-purpose.svg"/><img src="assets/banner-purpose.svg" width="97%" alt="A Paper Must Have a Purpose"/></picture>

A paper does not report what you did. It changes how a community understands a problem. Full page: [01 — A paper must have a purpose](Writing/01-Purpose.md).

- New and original is not enough. A result becomes knowledge only when a competent community challenges and accepts it.
- Write: what the field accepts, the consequential problem in it, the change you propose, and why the evidence should convince the reader.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-introduction.svg"/><img src="assets/banner-introduction.svg" width="97%" alt="The Introduction Is a Scenario"/></picture>

The introduction tells a story in the order the reader needs it. Full page: [02 — The introduction is a scenario](Writing/02-Introduction.md), with an [annotated example](Examples/01-IntroductionAsScenario.md).

- Setting, protagonist, objective, perturbation, stakes, proposed resolution, challenge, resolution.
- Begin with something the reader already values, not a definition or a history.
- The protagonist is the theory, technology or system, never the authors.
- Give the reader a reason to care before the background.
- The last paragraph states the claims in the order the Results show them.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-figures.svg"/><img src="assets/banner-figures.svg" width="97%" alt="Figures Construct the Argument"/></picture>

Data do not speak. Figures build meaning through selection, comparison and annotation. Full page: [03 — Figures construct the argument](Writing/03-Figures.md). Worked example: [Example 4](Examples/04-Figures.md).

- Each figure answers one necessary question. Order the figures by the questions a skeptical reader asks, not by when the experiments were done.
- Figure 1 is the concept, often the conventional approach next to the new one.
- One figure per Results section, named with the same words. The setup, simplified, is panel a of the figure that uses it.
- One color per physical object (a pump, a regime, a locking path), the same in every figure, setup drawings included. Never reuse a color for something else.
- Measured data are markers, simulations and theory are lines.
- The bold caption title states the message. The caption defines every color, marker and line.
- The abstract, figures and captions are enough to follow the main argument.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-results.svg"/><img src="assets/banner-results.svg" width="97%" alt="The Results Section"/></picture>

Show one result at a time, without repetition. Full page: [04 — The Results section](Writing/04-Results.md), with bad sentences next to their published version in [Example 2](Examples/02-ResultsSentences.md).

- Each claim of the last introduction paragraph becomes one section, in the same order and with the same words. Each section opens with what the previous one established; the Discussion restates the claim as demonstrated.
- One section per result. If the format has titles, the title states the result.
- State what is expected before the measurement, and start every measurement with why it is done.
- End every measurement with the number, compared to what was expected, and what it confirms.
- Describe the device once. Details go to Methods or the Supplementary; in an abstract, keep them as short as possible.
- One name per object and one symbol per quantity. Define every symbol, then write the symbol instead of the words.
- Define an acronym only if you use it again, then write only the acronym.
- ν for signal frequencies (optical or microwave), f only for the Fourier frequency.
- Always `\cref`, and every claim cites its figure panel: `(\cref{fig:2}b)`.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-conclusion.svg"/><img src="assets/banner-conclusion.svg" width="97%" alt="The Conclusion"/></picture>

The conclusion mirrors the introduction: it answers the problem the introduction raised, then says what the answer makes possible. Full page: [05 — The conclusion closes the loop and opens](Writing/05-Conclusion.md). Worked example: [Example 3](Examples/03-ConclusionMirrorsIntroduction.md).

- Letters and conference abstracts: an "In conclusion" paragraph (one or two sentences in an abstract). Long articles: a Discussion, without a recap of the Results.
- Answer the problem of the introduction, in its words, and take back each limitation it listed, now removed, with the number.
- In letters, recap each result once, in the order of the Results, with its number and its cause.
- Return to the applications of the first paragraph of the introduction.
- State the limitation that remains and why it is not fundamental.
- Open: say what the work now makes possible, from the nearest step to the farthest, each with its mechanism.
- No new result.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-style.svg"/><img src="assets/banner-style.svg" width="97%" alt="Style"/></picture>

Readers cannot challenge an argument they cannot follow. Full page: [06 — Style](Writing/06-Style.md). Worked example: [Example 5](Examples/05-Style.md).

- Follow Strunk and White: omit needless words, use concrete language, keep related words together, put the important words at the end.
- Begin with the setup or condition, end with the result. Make the physics the subject, not "we".
- Make the logic explicit (*because*, *therefore*), and state what is new against what is known (*unlike*, *in contrast*).
- Replace qualitative words with numbers.
- Use the same terms, symbols, units, colors and line styles throughout. Never swap a precise term for a synonym.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-notation.svg"/><img src="assets/banner-notation.svg" width="97%" alt="Notation and Units"/></picture>

Write every number, unit and symbol the same way. Full page, with the `siunitx` setup and checks to run before submission: [07 — Notation and units](Writing/07-NotationAndUnits.md).

- Every value with a unit goes through `\qty{}{}`, with unit macros (`\nm`, `\THz`, `\mW`), never typed by hand.
- The symbol and the relation go inside `\qty`: `\qty{\nu_0 \approx 283}{\THz}`.
- SI units only: `\qty{100}{\mm}` wafer, never "four-inch". dBm is not SI: in figures, the axis is in dB and the caption says "normalized to 1 mW (dBm)".
- Approximately equal is `\simeq` or `\approx`, never `\sim`. No e-notation.
- Frequency first, wavelength in parentheses: `\qty{\approx 283}{\THz} (\qty{1060}{\nm})`.
- Math mode: sub- and superscripts on a symbol use `_` and `^`, with descriptive labels upright: `$\nu_\mathrm{rep}$`.
- Text mode: sub- and superscripts on a word use `\textsubscript` and `\textsuperscript`: `TE\textsubscript{0}`, `k\textsuperscript{th}`.
- Chemical formulas and isotopes use `\ce{}`: `\ce{Si3N4}`, `\ce{^{87}Rb}`.

<a id="pages"></a>

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-pages.svg"/><img src="assets/banner-pages.svg" width="97%" alt="Pages"/></picture>

| Page | What it covers |
|------|-----------------|
| [01 — A paper must have a purpose](Writing/01-Purpose.md) | Why a paper exists |
| [02 — The introduction is a scenario](Writing/02-Introduction.md) | The eight steps of an introduction |
| [03 — Figures construct the argument](Writing/03-Figures.md) | What a figure does and how the figures progress |
| [04 — The Results section](Writing/04-Results.md) | From the introduction to the Results, structure of each result, names and symbols, and references |
| [05 — The conclusion closes the loop and opens](Writing/05-Conclusion.md) | How the conclusion answers the introduction, the two formats, and what the work opens |
| [06 — Style](Writing/06-Style.md) | Strunk and White, the active-voice exception, and consistency |
| [07 — Notation and units](Writing/07-NotationAndUnits.md) | The `siunitx` setup, `\qty`, approximation signs, sub- and superscripts, `\ce`, and pre-submission checks |
| [Example 1: The introduction is a scenario](Examples/01-IntroductionAsScenario.md) | Annotated introduction from the self-aligned PDCS paper |
| [Example 2: Results sentences, bad and published](Examples/02-ResultsSentences.md) | Sentences written badly on purpose next to their published version in the self-aligned PDCS paper |
| [Example 3: The conclusion mirrors the introduction](Examples/03-ConclusionMirrorsIntroduction.md) | Introduction and conclusion side by side in published papers |
| [Example 4: Figures in published papers](Examples/04-Figures.md) | Each figure rule in the group's published figures and captions |
| [Example 5: Style, bad and published](Examples/05-Style.md) | Sentences written badly on purpose next to their published version, one per style rule |

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-repo-layout.svg"/><img src="assets/banner-repo-layout.svg" width="97%" alt="What's in This Repo"/></picture>

```text
ScientificWriting/
├── README.md
├── Writing/
│   ├── 01-Purpose.md
│   ├── 02-Introduction.md
│   ├── 03-Figures.md
│   ├── 04-Results.md
│   ├── 05-Conclusion.md
│   ├── 06-Style.md
│   └── 07-NotationAndUnits.md
└── Examples/
    ├── 01-IntroductionAsScenario.md
    ├── 02-ResultsSentences.md
    ├── 03-ConclusionMirrorsIntroduction.md
    ├── 03-Figures.md
    └── 05-Style.md
```

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-see-also.svg"/><img src="assets/banner-see-also.svg" width="97%" alt="See Also"/></picture>

References:

- Larry McEnerney, [*The Craft of Writing Effectively*](https://www.youtube.com/watch?v=vtIzMaLkCaM), University of Chicago.
- William Strunk Jr. and E. B. White, *The Elements of Style*.

Related JQInanophotonics guides:

- [ScientificPresentations](https://github.com/JQInanophotonics/ScientificPresentations) for structuring a talk and presenting its argument.
- [ScientificGraphicDesign](https://github.com/JQInanophotonics/ScientificGraphicDesign) for plotting and publication-quality figures.
- [ScientificDataManagement](https://github.com/JQInanophotonics/ScientificDataManagement) for organizing the data and code behind a paper.
