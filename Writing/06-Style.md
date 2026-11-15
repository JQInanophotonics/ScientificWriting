# 06 — Style

## Follow Strunk and White

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

## A scientific exception to active voice

Strunk and White advise writers to use the active voice. This should not be an absolute rule in a scientific paper.

Begin with the setup, system, condition, or information already known to the reader. Move toward the new result. The authors should not automatically become the subject.

Write:

> The Kerr nonlinearity synchronizes the soliton to the reference field.

Do not automatically write:

> We show that the Kerr nonlinearity synchronizes the soliton to the reference field.

Use passive voice when it preserves this order or when the actor does not matter.

> **Begin with the setup. End with the result.**

## Rules from the group's papers

1. **Begin the sentence with the setup or condition, end with the result.**
2. **Make the logic explicit.** Link a sentence to the previous one with *because*, *since*, *therefore* or *thus*, so the reader sees why it follows.
3. **State what is new against what is known.** Use *unlike*, *although* or *in contrast* to place the result next to the conventional approach.
4. **Replace qualitative words with numbers.** Never "much narrower", "large", "good agreement" alone: give the values.
5. **Make the physics the subject.** In the group's published papers, only 6 to 17 % of sentences start with "We".

### In published papers

The condition first, the result last (rule 1):

> Using on-chip pump powers of \qty{P_-=145}{\mW} and \qty{P_+=70}{\mW} for the pumps at $\nu_-$ and $\nu_+$, respectively, we deterministically generate an octave-spanning PDCS (\cref{fig:2}b; see Methods).

Each sentence follows from the previous one (rule 2):

> Because both pumps become part of the PDCS comb, they satisfy $\nu_+ = 2n_-\nu_\mathrm{rep}^\mathrm{pdcs} + \nu_\mathrm{ceo}^\mathrm{pdcs}$ and $\nu_- = n_-\nu_\mathrm{rep}^\mathrm{pdcs} + \nu_\mathrm{ceo}^\mathrm{pdcs}$. The CEO can therefore be readily measured and stabilized before the chip from the strong beat between one of the pumps at $\nu_+$ and the other doubled pump at $2\nu_-$.

The new against the known (rule 3):

> Although this self-alignment is conceptually related to Kerr-induced synchronization (KIS), where a single DKS comb tooth is captured by a weak externally injected reference laser, the two phenomena differ fundamentally. In KIS, the reference weakly perturbs a DKS and plays no role in the soliton's energy balance. In contrast, in the self-alignment regime described here, the two pump fields simultaneously synchronize and generate the PDCS through a fully non-perturbative interaction […]

Numbers, not adjectives (rule 4):

> Due to self-alignment, the repetition rate noise depends only on the pump frequency noises, reducing its \qty{3}{\dB} linewidth from \qty{70}{\kHz} for the free-running case with three comb components to \qty{1.8}{\kHz} (\cref{fig:2}e).

All four quotes: *Self-aligned optical microcomb emerging between octave separated lasers*, Nature 2026.

## Be consistent

Use the same terminology, symbols, units, colors, fonts, and visual conventions throughout the paper. Do not replace a precise term with a synonym to avoid repetition. A color, line style, or symbol must retain the same meaning in every figure. The reader should evaluate the science, not decode its presentation.

The rules for numbers, units and symbols are in [07 — Notation and units](07-NotationAndUnits.md).
