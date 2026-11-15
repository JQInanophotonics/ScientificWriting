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

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-purpose.svg"/><img src="assets/banner-purpose.svg" width="97%" alt="A Paper Must Have a Purpose"/></picture>

A paper does not report what you did. It changes how a community understands a problem. Full page: [01 — Purpose](Writing/01-Purpose.md).

- New and original is not enough. A result becomes knowledge only when a competent community challenges and accepts it.
- Write: what the field accepts, the consequential problem in it, the change you propose, and why the evidence should convince the reader.
- Do not write the history of the project. Keep in the main text only what advances the argument; procedures go to Methods, secondary results to the Supplementary.
- Each paragraph has one purpose: claim, evidence or reasoning, interpretation, consequence.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-introduction.svg"/><img src="assets/banner-introduction.svg" width="97%" alt="The Introduction Is a Scenario"/></picture>

The introduction tells a story in the order the reader needs it. Full page: [02 — The introduction is a scenario](Writing/02-Introduction.md), with an [annotated example](Examples/01-IntroductionAsScenario.md).

- Setting, protagonist, objective, perturbation, stakes, proposed resolution, challenge, resolution.
- Begin with something the reader already values, not a definition or a history.
- The protagonist is the theory, technology or system, never the authors.
- Give the reader a reason to care before the background.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-figures.svg"/><img src="assets/banner-figures.svg" width="97%" alt="Figures Construct the Argument"/></picture>

Data do not speak. Figures build meaning through selection, comparison and annotation. Full page: [03 — Figures construct the argument](Writing/03-Figures.md).

- Each figure answers one necessary question, with panels in a logical order.
- Order the figures by the questions a skeptical reader asks, not by when the experiments were done.
- The abstract, figures and captions are enough to follow the main argument.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-results.svg"/><img src="assets/banner-results.svg" width="97%" alt="The Results Section"/></picture>

Show one result at a time, without repetition. Full page, with examples from published papers and a worked bad/good example: [04 — The Results section](Writing/04-Results.md).

- One section per result, and its title states the result.
- State what is expected before the measurement, and start every measurement with why it is done.
- End every measurement with the number, compared to what was expected, and what it confirms.
- Describe the device once. Details go to Methods or the Supplementary; in an abstract, keep them as short as possible.
- One name per object and one symbol per quantity. Define every symbol, then write the symbol instead of the words.
- Define an acronym only if you use it again, then write only the acronym.
- ν for signal frequencies (optical or microwave), f only for the Fourier frequency.
- Always `\cref`, and every claim cites its figure panel: `(\cref{fig:2}b)`.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-style.svg"/><img src="assets/banner-style.svg" width="97%" alt="Style"/></picture>

Readers cannot challenge an argument they cannot follow. Full page: [05 — Style](Writing/05-Style.md).

- Follow Strunk and White: omit needless words, use concrete language, keep related words together, put the important words at the end.
- Begin with the setup, end with the result. The authors do not automatically become the subject.
- Use the same terms, symbols, units, colors and line styles throughout. Never swap a precise term for a synonym.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-notation.svg"/><img src="assets/banner-notation.svg" width="97%" alt="Notation and Units"/></picture>

Write every number, unit and symbol the same way. Full page, with the `siunitx` setup and checks to run before submission: [06 — Notation and units](Writing/06-NotationAndUnits.md).

- Every value with a unit goes through `\qty{}{}`, with unit macros (`\nm`, `\THz`, `\mW`), never typed by hand.
- The symbol and the relation go inside `\qty`: `\qty{\nu_0 \approx 283}{\THz}`.
- Approximately equal is `\simeq` or `\approx`, never `\sim`. No e-notation.
- Frequency first, wavelength in parentheses: `\qty{\approx 283}{\THz} (\qty{1060}{\nm})`.
- Math mode: sub- and superscripts on a symbol use `_` and `^`, with descriptive labels upright: `$\nu_\mathrm{rep}$`.
- Text mode: sub- and superscripts on a word use `\textsubscript` and `\textsuperscript`: `TE\textsubscript{0}`, `k\textsuperscript{th}`.
- Chemical formulas and isotopes use `\ce{}`: `\ce{Si3N4}`, `\ce{^{87}Rb}`.

<a id="pages"></a>

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-pages.svg"/><img src="assets/banner-pages.svg" width="97%" alt="Pages"/></picture>

| Page | What it covers |
|------|-----------------|
| [01 — Purpose](Writing/01-Purpose.md) | Why a paper exists, and what belongs in the main text |
| [02 — The introduction is a scenario](Writing/02-Introduction.md) | The eight steps of an introduction |
| [03 — Figures construct the argument](Writing/03-Figures.md) | What a figure does and how the figures progress |
| [04 — The Results section](Writing/04-Results.md) | Structure of each result, names and symbols, references, and a worked bad/good example |
| [05 — Style](Writing/05-Style.md) | Strunk and White, the active-voice exception, and consistency |
| [06 — Notation and units](Writing/06-NotationAndUnits.md) | The `siunitx` setup, `\qty`, approximation signs, sub- and superscripts, `\ce`, and pre-submission checks |
| [Example 1: The introduction is a scenario](Examples/01-IntroductionAsScenario.md) | Annotated introduction from the self-aligned PDCS paper |

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-repo-layout.svg"/><img src="assets/banner-repo-layout.svg" width="97%" alt="What's in This Repo"/></picture>

```text
ScientificWriting/
├── README.md
├── Writing/
│   ├── 01-Purpose.md
│   ├── 02-Introduction.md
│   ├── 03-Figures.md
│   ├── 04-Results.md
│   ├── 05-Style.md
│   └── 06-NotationAndUnits.md
└── Examples/
    └── 01-IntroductionAsScenario.md
```

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-see-also.svg"/><img src="assets/banner-see-also.svg" width="97%" alt="See Also"/></picture>

References:

- Larry McEnerney, [*The Craft of Writing Effectively*](https://www.youtube.com/watch?v=vtIzMaLkCaM), University of Chicago.
- William Strunk Jr. and E. B. White, *The Elements of Style*.

Related JQInanophotonics guides:

- [ScientificPresentations](https://github.com/JQInanophotonics/ScientificPresentations) for structuring a talk and presenting its argument.
- [ScientificGraphicDesign](https://github.com/JQInanophotonics/ScientificGraphicDesign) for plotting and publication-quality figures.
- [ScientificDataManagement](https://github.com/JQInanophotonics/ScientificDataManagement) for organizing the data and code behind a paper.
