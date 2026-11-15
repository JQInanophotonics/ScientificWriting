# 05 — The Results section

The Results section shows, one result at a time, the evidence the introduction promised. Every sentence either says why a measurement is made, what is expected, what is measured, or what it confirms. Anything else is repetition or belongs in Methods.

## From the introduction to the Results

The last paragraph of the introduction is the table of contents of the Results, and the Discussion closes it. This is what makes the paper read as one argument.

1. **The last paragraph of the introduction states each claim in the order the Results show it.** Each claim becomes one Results section.
2. **Each section reuses the words of its claim.** In the title when the format has titles, otherwise in the first sentence of the section.
3. **Each section opens with what the previous one established and what is still open.**
4. **The Discussion opens by restating the claim of the introduction, now as demonstrated, in the same words.** See [06 — The conclusion closes the loop and opens](06-Conclusion.md).

The claims of the introduction and the sections of the Results in *Toward chaotic group velocity hopping of an on-chip DKS* (PRL 2025):

| Last paragraph of the introduction | Results section |
|---|---|
| "we demonstrate the second-order Adler equation's validity for KIS" | Phase-Modulated Adler Model |
| "We quantitatively validate the model against experiments and Lugiato-Lefever simulations" | Model Verification |
| "we leverage the Adler model's predictions to experimentally show chaotic DKS hopping […], resulting in chaotic group velocity hopping" | Chaotic group velocity hopping |

The self-aligned PDCS paper (Nature 2026) does the same: advances (i) and (ii) of the introduction become "Concept and experimental demonstration", and "the three core tasks of self-referenced OFCs" become "Self-aligned PDCS metrology".

Section openings that carry the thread (rule 3 above):

> Having shown that the second-order Adler equation accurately describes the soliton phase dynamics under KIS, we now apply this model to predict the regime in which chaotic behavior of the DKS is expected.
>
> — AC-KIS, PRL 2025

> The above empirical demonstration highlights the coherent trapping aspect of the multi-DKS state to the same reference field, yet does not fully elucidate the solitons' relative dynamical stability.
>
> — All-optical azimuthal trapping of Kerr multi-solitons, APL Photonics 2025

> Having established the self-balancing behavior in purely quadratic and in cubic integrated dispersion systems, we now extend our analysis to a resonator with an experimentally realistic and desirable quartic dispersion that supports two dispersive waves.
>
> — DKS self-balancing, PRA 2026

The introduction and the Discussion in the same words (rule 4 above):

> Here, we theoretically analyze and experimentally demonstrate the profound improvements that KIS enables on both the repetition rate noise and individual comb tooth noise in DKS microcombs.
>
> In conclusion, we have demonstrated both theoretically and experimentally that Kerr-induced synchronization (KIS) enables, in an all-optical fashion, quenching of internal noise sources in integrated optical frequency combs […]
>
> — All-optical noise quenching, Optica 2025

## Rules

### Structure

1. **One section per result.** If the format has section titles, the title states the result: "KIS damps the thermorefractive noise", not "Noise measurements".
2. **Say what is expected before showing the measurement.** Give the model, equation or simulation first, so the reader knows what to look for in the figure.
3. **Start every measurement with why it is done.** The reader must know what question the measurement answers before reading how it is made.
4. **End every measurement with the number, compared to what was expected, and what it confirms.** A measurement without a number and a comparison proves nothing.

### Content

5. **Describe the device and its operating conditions once, in one place.** The details go to Methods or the Supplementary when the format has them. In an abstract, keep them as short as possible.
6. **State every limit or mismatch with where it happens and why.** Give the range (Fourier frequency, power, detuning) and the cause. Never write "at higher frequencies, this is not true anymore".
7. **Compare two things only under the same conditions, and say what those conditions are.**

### Notation

8. **Give each object one name and use it everywhere.** Never alternate "repetition rate", "rep rate" and "FSR". Define an acronym only if you use it again, and once it is defined, write only the acronym.
9. **Give each quantity one symbol and use it everywhere.**
10. **Define every symbol where it first appears.**
11. **Once a symbol is defined, write the symbol instead of the words.** Write "we lock $\nu_\mathrm{rep}^\mathrm{pdcs}$ to the same \qty{10}{\MHz} reference", not "we lock the repetition rate of the PDCS to the same 10 MHz reference".
12. **Use ν for signal frequencies, optical or microwave, and f only for the Fourier frequency.**
13. **Introduce every equation with why it is needed, and follow it with what it means.**

### References

14. **Always use `\cref`.** Never "Eq. (2)", "equation (\ref{})" or "figure \ref{}".
15. **Every claim cites the figure panel that shows it**, at the end of the sentence: `(\cref{fig:2}b)`.

Notation and units follow [08 — Notation and units](08-NotationAndUnits.md).

## In published papers

Why the measurement is made, then how (rule 3):

> To confirm that the self-aligned PDCS acts as a true clockwork, we perform a second experiment a day later in which we locked a fiber comb's CEO and one comb tooth to the clock laser, achieving identical Allan deviation performance except at \qty{\tau<1}{\s}, where the PDCS repetition rate noise is dominated by the EOcomb downconverter.
>
> — Self-aligned PDCS, Nature 2026

The sentence also ends with the mismatch, where it happens (τ < 1 s) and why (rule 6).

The device described once, inside the sentence that says why it is used (rules 3 and 5):

> To demonstrate such performance improvement through KIS, we use an integrated microring resonator made of \qty{H=670}{\nm} thick \ce{Si3N4} embedded in \ce{SiO2}, with a ring radius of \qty{R=23}{\um} and a ring width of \qty{RW=850}{\nm}.
>
> — All-optical noise quenching, Optica 2025

Defined symbols instead of words, and the panel at the end of the sentence (rules 11 and 15):

> The repetition rate therefore depends linearly on the pump detunings $\delta\nu_\pm$, with opposite signs for positive- and negative-pump actuation and slope magnitude $1/N=1/(n_+-n_-)=1/n_-$ corresponding to the optical frequency division (OFD) factor (\cref{fig:2}d).
>
> — Self-aligned PDCS, Nature 2026

## Worked example

[Example 2: Results sentences, bad and published](../Examples/02-ResultsSentences.md) shows sentences written badly on purpose next to their published version.

## Before submission

Read each Results paragraph and check:

- Does it start with why the measurement is made?
- Does it end with a number, compared to the expectation, and the panel that shows it?
- Is every symbol defined, and used instead of words afterwards?
- Does any object have two names, or any quantity two symbols?

```bash
grep -nE 'Eq\. ?\(|[Ff]ig(ure|\.)? ?\\ref|equation ?\(?\\ref' paper.tex   # references without \cref
grep -nE 'rep(etition)? rate|beat (tone|note)|FSR' paper.tex           # synonyms for one quantity
```
