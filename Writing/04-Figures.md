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

1. **Figure 1 is the concept.**
   It is a schematic of the mechanism, not data. It shows the reader, before any measurement, what the paper does and why it is different.
   - Draw the conventional approach next to the new one: panel a the established scheme with its limitation, panel b the new scheme. The reader then sees the perturbation of the introduction in one glance.
   - Keep it free of experimental detail. The concept must be readable by someone outside the subfield.
   - The introduction cites Fig. 1 when it states the problem and the proposed resolution.

2. **One figure per Results section, with the same words.**
   The figure is the evidence for one result, so it carries the same claim as its section.
   - The figure title and the section title, or the first sentence of the section when there are no titles, name the same result with the same words.
   - If a section needs two figures, both titles name the same result and say which side of it each shows.
   - A figure whose message cannot be matched to a section is either a Supplementary figure or a missing section.

3. **The experimental setup is panel a of the figure that uses it, and it is simplified.**
   The reader needs to know what is measured and how the signal is obtained, not the full bench.
   - Draw only the parts the result needs: the lasers, the device, the detection. Leave out amplifiers, polarization controllers and attenuators unless the result depends on them.
   - The full setup, with part numbers, goes to Methods or the Supplementary.
   - Put the setup next to the data it produces, not in a separate setup figure.

4. **A color, marker or line style keeps the same meaning in every figure.**
   The reader learns the code once, in the first figure, and reuses it.
   - Assign a color to each physical object or condition (for example, with and without synchronization) and keep it in every figure.
   - Measured data are markers; simulations and theory are lines. A reader then tells measurement from model without reading the caption.
   - Never reuse a color for a different meaning in a later figure.

### The caption

5. **The bold title states the message of the figure,** not the type of plot.
   Write the result the figure demonstrates, as a statement: what is shown to work, scale or differ. Not "Optical spectra" or "Noise measurements". A reader who reads only the titles of the figures should get the argument of the paper.

6. **Each panel starts with its bold letter, then what is plotted.**
   Start with the quantity on the plot, then against what: "**b** Repetition rate against the pump detuning". The reader looks at the panel while reading the caption and must find the axes first.

7. **The caption defines every color, marker and line style,** in parentheses right after what they show: "(circles: measured, solid line: simulation)". No separate legend paragraph at the end of the caption, and no symbol left for the reader to guess.

8. **The caption gives the conditions needed to read the panel:** pump frequencies and powers, mode numbers, simulation parameters. The figure must be understandable without the text. Give only the conditions that change the reading of the panel; the rest belongs in Methods.

9. **A panel ends with what it shows or confirms** when that is not obvious from the plot. One short clause: "confirming the self-alignment" or "in agreement with the simulation".

How a figure looks (fonts, line widths, colors, export) is covered in [ScientificGraphicDesign](https://github.com/JQInanophotonics/ScientificGraphicDesign).

## Worked example

[Example 4: Figures in published papers](../Examples/04-Figures.md) shows each rule in the group's published figures and captions.
