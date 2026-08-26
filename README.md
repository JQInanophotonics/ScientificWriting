<div align="center">

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/header.svg"/><img src="assets/header.svg" width="97%" alt="Scientific Writing"/></picture>

<a href="#pages"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/PAGES-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/PAGES-ffffff?style=flat-square&logoColor=1a1a1a" alt="Pages"/></picture></a>
<a href="https://github.com/JQInanophotonics/ScientificPresentations"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/PRESENTATIONS-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/PRESENTATIONS-ffffff?style=flat-square&logoColor=1a1a1a" alt="Scientific Presentations"/></picture></a>
<a href="https://github.com/JQInanophotonics/ScientificGraphicDesign"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/GRAPHIC%20DESIGN-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/GRAPHIC%20DESIGN-ffffff?style=flat-square&logoColor=1a1a1a" alt="Scientific Graphic Design"/></picture></a>
<a href="https://github.com/JQInanophotonics/ScientificDataManagement"><picture><source media="(prefers-color-scheme: dark)" srcset="https://img.shields.io/badge/DATA%20MANAGEMENT-0d1117?style=flat-square&logoColor=ffffff"/><img src="https://img.shields.io/badge/DATA%20MANAGEMENT-ffffff?style=flat-square&logoColor=1a1a1a" alt="Scientific Data Management"/></picture></a>

</div>

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-forewords.svg"/><img src="assets/banner-forewords.svg" width="97%" alt="Forewords"/></picture>

This repository is the group's concise guide to writing a scientific paper.
The README states the guidelines. The worked examples show how one guideline
appears in a real paper through short excerpts and direct annotations.

Read the guide first, then use the examples to see each rule applied. The
current example is [The introduction is a
scenario](Examples/01-IntroductionAsScenario.md).

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-purpose.svg"/><img src="assets/banner-purpose.svg" width="97%" alt="A Paper Must Have a Purpose"/></picture>

A scientific paper does not exist to report what you did. Its purpose is to change how a scientific community understands a problem.

In the University of Chicago lecture [*The Craft of Writing Effectively*](https://www.youtube.com/watch?v=vtIzMaLkCaM), Larry McEnerney states:

> "Nothing will be accepted as knowledge or understanding until it has been challenged by someone competent to challenge it."

A new dataset is **not knowledge**. A new experiment is **not knowledge**. A new demonstration is **not knowledge**. New and original are not enough.

McEnerney makes this point with two examples. Counting the people in a room produces information that nobody previously possessed. It is new and original. It is not knowledge because nobody finds it valuable. He also describes a researcher who discovered and studied previously unread travel journals. Her work was original, but her committee rejected it because she had not shown why anyone in the field should care.

A result must be useful to a specific scientific community, survive challenges from competent readers, and be accepted by that community. A paper makes the case for that acceptance.

Academic readers are not passive recipients. Their professional role is to challenge your claim. Therefore, do not write:

> Here is what I discovered.

Write:

> Here is what this field currently accepts. However, there is a consequential problem in that understanding. Here is the change I propose, why it matters to you, and why the evidence should convince you.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-introduction.svg"/><img src="assets/banner-introduction.svg" width="97%" alt="The Introduction Is a Scenario"/></picture>

The introduction presents a result to the community and gives it a chance to become knowledge. Like any story, it needs a setting, a protagonist, an objective, a perturbation, and a resolution.

1. **The setting.** Establish what the field currently accepts. Do not begin with a definition or general history. Begin with something your readers already value.
2. **The protagonist.** Introduce the theory, technology, physical system, or established approach. The protagonist is not the author. The paper is not about us.
3. **The objective.** State what the protagonist should provide and why it matters to the reader.
4. **The perturbation.** Create tension with a limitation, contradiction, anomaly, tradeoff, or failed assumption. Words such as *but*, *however*, *although*, and *despite* often mark this turn. Inverting an established approach is one tool, not a requirement.
5. **The stakes.** State what the problem prevents the community from understanding or doing. Without a consequence, the result may be new, but it is not valuable.
6. **The proposed resolution.** Introduce the work as a direct response: *Here, we show...* It must not appear as an unrelated demonstration.
7. **The challenge.** Anticipate what competent readers will doubt and state the evidence needed to answer them.
8. **The resolution.** State what changes if the claim survives those tests.

Scientific storytelling is not fiction or project history. It is the order in which the reader must encounter the ideas for the argument to make sense.

Do not begin by explaining everything you know. First give the reader a reason to care. Then provide the background needed to understand the problem.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-write-only.svg"/><img src="assets/banner-write-only.svg" width="97%" alt="Write Only What Matters"/></picture>

The reader does not care how long an experiment took, how difficult it was, or when the result appeared. Effort does not determine scientific importance.

A result belongs in the main text only if it advances the argument or supplies evidence required to support it. Months of work may deserve one sentence or a supplementary figure. A simple control may deserve a central panel if it closes the argument.

Keep only the ideas that carry the story in the main text. Put procedures in the Methods and supporting derivations, controls, and secondary results in the Supplementary Information.

> **Do not write the history of the project. Write the argument the reader needs.**

Each paragraph should have one purpose:

> **Claim, evidence or reasoning, interpretation, consequence.**

Remove anything that does not perform one of those jobs.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-figures.svg"/><img src="assets/banner-figures.svg" width="97%" alt="Figures Construct the Argument"/></picture>

"Let the data speak for themselves" is wrong. Data do not speak.

A figure creates meaning through selection, comparison, organization, annotation, and visual hierarchy. It tells a story that the data alone cannot.

Each figure should answer one necessary question, with panels in a logical order. The figure presents the evidence. The text states what it demonstrates and why it matters.

The abstract, figures, and captions should be enough to follow the main argument.

### Make the evidence progress naturally

Arrange the figures according to the questions a skeptical reader will ask. Do not arrange them according to the order in which the experiments were performed.

A common progression is:

> **Concept, mechanism, experimental proof, control, performance, application.**

This is not a formula. Every figure should establish something required by the next one. If two can be exchanged without affecting the argument, their roles may be unclear.

The introduction proposes a resolution. The figures test it. The discussion states what changes if it is accepted.

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-strunk-white.svg"/><img src="assets/banner-strunk-white.svg" width="97%" alt="Follow Strunk and White"/></picture>

The sentence-level rules in this guide come from William Strunk Jr. and E. B. White, *The Elements of Style*. Read the book.

Apply these rules throughout the paper:

- **Omit needless words.**
- **Use definite, specific, concrete language.**
- **State ideas positively.**
- **Keep related words together.**
- **Use parallel structure for parallel ideas.**
- **Place the important words at the end of the sentence.**
- **Give each paragraph one purpose.**

Readers cannot challenge an argument they cannot follow.

### A scientific exception to active voice

Strunk and White advise writers to use the active voice. This should not be an absolute rule in a scientific paper.

Begin with the setup, system, condition, or information already known to the reader. Move toward the new result. The authors should not automatically become the subject.

Write:

> The Kerr nonlinearity synchronizes the soliton to the reference field.

Do not automatically write:

> We show that the Kerr nonlinearity synchronizes the soliton to the reference field.

Use passive voice when it preserves this order or when the actor does not matter.

> **Begin with the setup. End with the result.**

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-consistency.svg"/><img src="assets/banner-consistency.svg" width="97%" alt="Be Consistent"/></picture>

Use the same terminology, symbols, units, colors, fonts, and visual conventions throughout the paper. Do not replace a precise term with a synonym to avoid repetition. A color, line style, or symbol must retain the same meaning in every figure. The reader should evaluate the science, not decode its presentation.

<a id="pages"></a>

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-pages.svg"/><img src="assets/banner-pages.svg" width="97%" alt="Pages"/></picture>

| Page | What it covers |
|------|-----------------|
| [Main guide](README.md) | Purpose, narrative, selection, figures, sentence-level writing, and consistency |
| [Example 1: The introduction is a scenario](Examples/01-IntroductionAsScenario.md) | Annotated introduction from the self-aligned PDCS paper |

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-repo-layout.svg"/><img src="assets/banner-repo-layout.svg" width="97%" alt="What's in This Repo"/></picture>

```text
ScientificWriting/
├── README.md
├── Examples/
│   └── 01-IntroductionAsScenario.md
└── assets/
    └── dark/
```

<picture><source media="(prefers-color-scheme: dark)" srcset="assets/dark/banner-see-also.svg"/><img src="assets/banner-see-also.svg" width="97%" alt="See Also"/></picture>

References:

- Larry McEnerney, [*The Craft of Writing Effectively*](https://www.youtube.com/watch?v=vtIzMaLkCaM), University of Chicago.
- William Strunk Jr. and E. B. White, *The Elements of Style*.

Related JQInanophotonics guides:

- [ScientificPresentations](https://github.com/JQInanophotonics/ScientificPresentations) for structuring a talk and presenting its argument.
- [ScientificGraphicDesign](https://github.com/JQInanophotonics/ScientificGraphicDesign) for plotting and publication-quality figures.
- [ScientificDataManagement](https://github.com/JQInanophotonics/ScientificDataManagement) for organizing the data and code behind a paper.
