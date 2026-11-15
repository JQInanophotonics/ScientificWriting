# 01 — The Results section

The Results section shows, one result at a time, the evidence the introduction promised. Every sentence either says why a measurement is made, what is expected, what is measured, or what it confirms. Anything else is repetition or belongs in Methods.

## Rules

### Structure

1. **One section per result, and its title states the result.** Write "KIS damps the thermorefractive noise", not "Noise measurements".
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
11. **Once a symbol is defined, write the symbol instead of the words.** Write "Since $\nu_\mathrm{rep} \approx 735$ GHz is too high to be detected", not "The 735 GHz repetition rate is too high".
12. **Use ν for signal frequencies, optical or microwave, and f only for the Fourier frequency.**
13. **Introduce every equation with why it is needed, and follow it with what it means.**

### References

14. **Always use `\cref`.** Never "Eq. (2)", "equation (\ref{})" or "figure \ref{}".
15. **Every claim cites the figure panel that shows it**, at the end of the sentence: `[\cref{fig:2}b]`.

Notation and units follow [00 — Notation and units](00-NotationAndUnits.md).

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

The number, compared to the prediction, with its panel (rules 4, 11 and 15):

> When the CEO is locked through actuation of the main pump frequency, $S_\mathrm{rep}^{kis}$ is further reduced thanks to the larger $OFD=M_\mathrm{ref}^2 = 193^2$~[\cref{fig:4}b(v)], and is in good agreement with the measured pump frequency noise divided by this larger OFD factor.
>
> — All-optical noise quenching, Optica 2025

## Worked example: fixing a conference abstract

The left column is a draft abstract on optical frequency division with a self-aligned PDCS and an electro-optic down-converter. The right column is how it should be written.

| Bad (current) | Good (fixed) |
|---|---|
| …features a FSR of about $f_{\mathrm{rep}}=735$ GHz. | `…generating a PDCS with \qty{\nu_\mathrm{rep} \approx 735}{\GHz}.` |
| The pump frequencies $\nu_-\sim 192$ THz and $\nu_+\sim 385$ THz are almost separated by an octave… | `Two pumps at \qty{\nu_- \approx 192}{\THz} and \qty{\nu_+ \approx 385}{\THz}, at modes $N_+ = 2N_-$, generate a PDCS centered at \qty{\nu_0 \approx 289}{\THz}.` |
| When the pumps are appropriately set on resonance, the PDCS can enter in the self-aligned regime, … allowing for metrology applications. | `Once self-aligned, the PDCS becomes a self-aligned parametrically driven cavity soliton (SParCS): the SParCS and both pumps share a single frequency grid, and $\nu_\mathrm{rep} = (\nu_+ - \nu_-)/N_-$ [\cref{fig:1}a].` |
| The self-aligned PDCS (SParCS) signal is then sent to a EO modulator to measure the soliton repetition rate. | `Since \qty{\nu_\mathrm{rep} \approx 735}{\GHz} is too high to be detected, we measure it by down-converting the SParCS with a TFLT phase modulator driven at \qty{\nu_\mathrm{eo} \approx 17.5}{\GHz}, such that $\nu_\mathrm{rep} = N_\mathrm{eo} \nu_\mathrm{eo} \pm \nu_\mathrm{beat}$ with $N_\mathrm{eo} = 42$ [\cref{fig:1}a].` |
| The EO modulator was designed in the TFLT platform (film thickness = 500 nm). This modulator consists of a dual-pass… | `…a dual-pass TFLT phase modulator~\cite{…}.` The rest goes to Methods or the Supplementary if the format has them. |
| Optical frequency division is demonstrated on figure \ref{fig:fig}(b). … where $N=N_-$ is OFD factor of the PDCS. ($S_\mathrm{b}$ and $f$ never defined) | `…where $f$ is the Fourier frequency, $N_-$ the SParCS division factor, and $S_\mathrm{b}$ [?].` |
| Rewriting equation (\ref{eq:PN}) for the beat note phase noise, we find a division a factor $1/N^2=1/261^2$… | `With free-running pumps, \cref{eq:PN} predicts that $\nu_\mathrm{rep}$ carries the pump noise divided by $N_-^2 = 261^2$.` |
| This trend is confirmed experimentally at low frequency… At higher frequencies, this is not true anymore… | `$S_\mathrm{beat}$ follows this prediction for \qty{f < [?]}{\kHz} [\cref{fig:1}b], above which the synthesizer noise dominates.` |
| Both phase noise (ppln/tflt) being identical, this shows that the TFLT doesn't introduce any additional noise… | `To verify that the TFLT chip adds no noise, we measure the same SParCS with a bulk PPLN modulator. Both $S_\mathrm{beat}$ overlap [\cref{fig:1}b].` |
| …the OFD factor on the frequencyRF frequency becomes $N\times N_{\mathrm{eo}}=10 962$, which is confirmed experimentally… | `With $\nu_\mathrm{beat}$ locked to a \qty{10}{\MHz} reference, [?] carries the pump noise divided by $(N_- N_\mathrm{eo})^2 = (261 \times 42)^2$ up to the \qty{[?]}{\kHz} servo bandwidth [\cref{fig:1}c].` |
| rep rate / repetition rate / FSR; beat / beat tone / beat note; PDCS / self-aligned PDCS / SParCS | `$\nu_\mathrm{rep}$` and `$\nu_\mathrm{beat}$` everywhere. "SParCS" everywhere after it is defined. |

`[?]` marks a value or definition the draft never gives. Find it before writing the sentence.

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
