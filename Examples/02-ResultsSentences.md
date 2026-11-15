# Example 2: Results sentences, bad and published

## Paper

Grégory Moille *et al.*, [*Self-aligned optical microcomb emerging between
octave separated lasers*](https://arxiv.org/abs/2602.05151), arXiv:2602.05151
(2026). [PDF](https://arxiv.org/pdf/2602.05151) |
[DOI](https://doi.org/10.48550/arXiv.2602.05151)

This example applies [05 — The Results section](../Writing/05-Results.md) from the
[main guide](../README.md).

## Bad and published sentences

Each block names the rule, then shows a sentence written badly on purpose next to the sentence as published.

### Every symbol defined, `\qty` and `\approx` ([Rule 10](../Writing/05-Results.md#rules), [Notation](../Writing/07-NotationAndUnits.md))

| Bad | Good (published) |
|---|---|
| The pump frequencies ν₋ ∼ 193 THz and ν₊ ∼ 387 THz are almost separated by an octave, which is where the dispersion is good. | The dispersion conditions are satisfied at ν₋ ≈ 193 THz (n₋ = 263, C-band) and ν₊ ≈ 387 THz (n₊ = 2n₋ = 526, visible) (Fig. 2a). |

LaTeX of the good sentence: `\qty{\nu_- \approx 193}{\THz} ($n_-=263$, C-band)`.

### Describe the device once; details go to Methods ([Rule 5](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| The fabrication of the microrings was done by a commercial foundry and consists of several deposition, lithography, etching and cladding steps, and the bus waveguide was designed by changing its width and gap so that it couples light over more than an octave. | We demonstrate the above concept experimentally using silicon nitride microring resonators obtained via commercial four-inch wafer foundry fabrication, with a bus waveguide designed to couple across more than an octave (Fig. 1b; see Methods). |

### Start every measurement with why it is done ([Rule 3](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| The output of the chip is then sent to an OSA and to a photodiode to look at the beat between the PDCS and the pump comb. | We demonstrate self-alignment by directly measuring Δν_ceo between the PDCS and ν₊ pump comb (see Methods). |

### Write the symbol, here the relation, instead of words ([Rule 11](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| When the pumps are appropriately set, the PDCS can enter in the self-aligned regime, where it becomes aligned to the pumps, allowing for metrology applications. | In a self-aligned PDCS, both pumps are comb teeth that pin ν_rep = (ν₊ − ν₋)/(n₊ − n₋). |

### Always `\cref`, and define every symbol ([Rules 14 and 10](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| Optical frequency division is demonstrated on figure \ref{fig:2}(d), where the slope is 1/N. | The repetition rate therefore depends linearly on the pump detunings δν±, with […] slope magnitude 1/N = 1/(n₊ − n₋) = 1/n₋ corresponding to the optical frequency division (OFD) factor (Fig. 2d). |

LaTeX: `(\cref{fig:2}d)`, never `figure \ref{fig:2}(d)`.

### End with the number, compared to the reference ([Rule 4](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| The rep rate linewidth is much narrower once the soliton is self-aligned. | Due to self-alignment, the repetition rate noise depends only on the pump frequency noises, reducing its 3 dB linewidth from 70 kHz for the free-running case […] to 1.8 kHz (Fig. 2e). |

### State every limit with where it happens and why ([Rule 6](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| The division is confirmed experimentally at low frequency. At higher frequencies, this is not true anymore. | […] the lasers' long-term frequency drift prevents extended averaging. As a result, the noise floor exceeds the OFD of the laser noise above 10 kHz, which future work will improve. |

### Say why, and compare under the same conditions ([Rules 3 and 7](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| Both Allan deviations (PDCS/fiber comb) being identical, this shows that the PDCS works as a clockwork. | To confirm that the self-aligned PDCS acts as a true clockwork, we perform a second experiment […] in which we locked a fiber comb's CEO and one comb tooth to the clock laser, achieving identical Allan deviation performance except at τ < 1 s, where the PDCS repetition rate noise is dominated by the EOcomb downconverter. |

### One name per object, one symbol per quantity ([Rules 8 and 9](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| rep rate, repetition rate, FSR, comb spacing; PDCS, soliton, comb | ν_rep once defined; "PDCS" everywhere. |
