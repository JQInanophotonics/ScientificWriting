# Example 5: Style, bad and published

This example applies [07 — Style](../Writing/07-Style.md) from the [main guide](../README.md). Each block names the rule, then shows a sentence written badly on purpose next to the sentence as published.

## Paper

Grégory Moille *et al.*, [*Self-aligned optical microcomb emerging between octave separated lasers*](https://doi.org/10.1038/s41586-026-11086-2), Nature **658**, 350–357 (2026).

### Begin with the setup or condition, end with the result ([Rule 1](../Writing/07-Style.md#rules-from-the-groups-papers))

| Bad | Good (published) |
|---|---|
| `We deterministically generate an octave-spanning PDCS (\cref{fig:2}b), which is done with on-chip pump powers of \qty{P_-=145}{\mW} and \qty{P_+=70}{\mW} for the pumps at $\nu_-$ and $\nu_+$.` | `Using on-chip pump powers of \qty{P_-=145}{\mW} and \qty{P_+=70}{\mW} for the pumps at $\nu_-$ and $\nu_+$, respectively, we deterministically generate an octave-spanning PDCS (\cref{fig:2}b; see Methods).` |

### Make the logic explicit ([Rule 2](../Writing/07-Style.md#rules-from-the-groups-papers))

| Bad | Good (published) |
|---|---|
| `Both pumps satisfy $\nu_+ = 2n_-\nu_\mathrm{rep}^\mathrm{pdcs} + \nu_\mathrm{ceo}^\mathrm{pdcs}$ and $\nu_- = n_-\nu_\mathrm{rep}^\mathrm{pdcs} + \nu_\mathrm{ceo}^\mathrm{pdcs}$. The CEO can be measured before the chip from the beat between the pump at $\nu_+$ and the doubled pump at $2\nu_-$.` | `Because both pumps become part of the PDCS comb, they satisfy $\nu_+ = 2n_-\nu_\mathrm{rep}^\mathrm{pdcs} + \nu_\mathrm{ceo}^\mathrm{pdcs}$ and $\nu_- = n_-\nu_\mathrm{rep}^\mathrm{pdcs} + \nu_\mathrm{ceo}^\mathrm{pdcs}$. The CEO can therefore be readily measured and stabilized before the chip from the strong beat between one of the pumps at $\nu_+$ and the other doubled pump at $2\nu_-$.` |

### State what is new against what is known ([Rule 3](../Writing/07-Style.md#rules-from-the-groups-papers))

| Bad | Good (published) |
|---|---|
| `This self-alignment is a novel and unique phenomenon, where the two pump fields synchronize and generate the PDCS.` | `Although this self-alignment is conceptually related to Kerr-induced synchronization (KIS), where a single DKS comb tooth is captured by a weak externally injected reference laser, the two phenomena differ fundamentally. In KIS, the reference weakly perturbs a DKS and plays no role in the soliton's energy balance. In contrast, in the self-alignment regime described here, the two pump fields simultaneously synchronize and generate the PDCS through a fully non-perturbative interaction [...]` |

### Replace qualitative words with numbers ([Rule 4](../Writing/07-Style.md#rules-from-the-groups-papers))

| Bad | Good (published) |
|---|---|
| `The repetition rate linewidth becomes much narrower once the soliton is self-aligned (\cref{fig:2}e).` | `Due to self-alignment, the repetition rate noise depends only on the pump frequency noises, reducing its \qty{3}{\dB} linewidth from \qty{70}{\kHz} for the free-running case with three comb components to \qty{1.8}{\kHz} (\cref{fig:2}e).` |

### Make the physics the subject ([Rule 5](../Writing/07-Style.md#rules-from-the-groups-papers))

| Bad | Good |
|---|---|
| `We show that the Kerr nonlinearity synchronizes the soliton to the reference field.` | `The Kerr nonlinearity synchronizes the soliton to the reference field.` |
