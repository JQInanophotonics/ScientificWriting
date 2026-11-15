# Example 2: Results sentences, bad and published

## Paper

Grégory Moille *et al.*, [*Self-aligned optical microcomb emerging between
octave separated lasers*](https://doi.org/10.1038/s41586-026-11086-2),
Nature **658**, 350–357 (2026).

This example applies [05 — The Results section](../Writing/05-Results.md) from the
[main guide](../README.md).

## Bad and published sentences

Each block names the rule, then shows a sentence written badly on purpose next to the sentence as published.

### Every symbol defined, `\qty` and `\approx` ([Rule 10](../Writing/05-Results.md#rules), [Notation](../Writing/07-NotationAndUnits.md#rules))

| Bad | Good (published) |
|---|---|
| The pump frequencies $\nu_-\sim 193$ THz and $\nu_+\sim 387$ THz are almost separated by an octave, which is where the dispersion is good. | The dispersion conditions are satisfied at \qty{\nu_- \approx 193}{\THz} ($n_-=263$, C-band) and \qty{\nu_+ \approx 387}{\THz} ($n_+=2n_-=526$, visible) (\cref{fig:2}a). |

### Describe the device once; details go to Methods ([Rule 5](../Writing/05-Results.md#rules))

| Bad | Good (published, with SI units) |
|---|---|
| The fabrication of the microrings was done by a commercial foundry and consists of several deposition, lithography, etching and cladding steps, and the bus waveguide was designed by changing its width and gap so that it couples light over more than an octave. | We demonstrate the above concept experimentally using silicon nitride (\ce{Si3N4}) microring resonators obtained via commercial \qty{100}{\mm} wafer foundry fabrication, with a bus waveguide designed to couple across more than an octave (\cref{fig:1}b; see Methods). |

### Start every measurement with why it is done ([Rule 3](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| The output of the chip is then sent to an OSA and to a photodiode to look at the beat between the PDCS and the pump comb. | We demonstrate self-alignment by directly measuring $\Delta\nu_\mathrm{ceo}$ between the PDCS and $\nu_+$ pump comb (see Methods and Supplementary Information S.5). |

### Write the symbol, here the relation, instead of words ([Rule 11](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| When the pumps are appropriately set, the PDCS can enter in the self-aligned regime, where it becomes aligned to the pumps, allowing for metrology applications. | In a self-aligned PDCS, both pumps are comb teeth that pin $\nu_\mathrm{rep}^\mathrm{pdcs}=(\nu_+-\nu_-)/(n_+-n_-)$. |

### Always `\cref`, and define every symbol ([Rules 14 and 10](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| Optical frequency division is demonstrated on figure \ref{fig:2}(d), where the slope is $1/N$. | The repetition rate therefore depends linearly on the pump detunings $\delta\nu_\pm$, with opposite signs for positive- and negative-pump actuation and slope magnitude $1/N=1/(n_+-n_-)=1/n_-$ corresponding to the optical frequency division (OFD) factor (\cref{fig:2}d). |

### End with the number, compared to the reference ([Rule 4](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| The rep rate linewidth is much narrower once the soliton is self-aligned, as can be seen on figure \ref{fig:2}(e). | Due to self-alignment, the repetition rate noise depends only on the pump frequency noises, reducing its \qty{3}{\dB} linewidth from \qty{70}{\kHz} for the free-running case with three comb components to \qty{1.8}{\kHz} (\cref{fig:2}e). |

### State every limit with where it happens and why ([Rule 6](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| The division is confirmed experimentally at low frequency. At higher frequencies, this is not true anymore. | [...] the lasers' long-term frequency drift prevents extended averaging. As a result, the noise floor exceeds the OFD of the laser noise above \qty{10}{\kHz}, which future work will improve. |

### Say why, and compare under the same conditions ([Rules 3 and 7](../Writing/05-Results.md#rules))

| Bad | Good (published) |
|---|---|
| Both Allan deviations (PDCS/fiber comb) being identical, this shows that the PDCS works as a clockwork. | To confirm that the self-aligned PDCS acts as a true clockwork, we perform a second experiment a day later in which we locked a fiber comb's CEO and one comb tooth to the clock laser, achieving identical Allan deviation performance except at \qty{\tau<1}{\s}, where the PDCS repetition rate noise is dominated by the EOcomb downconverter. |

### One name per object, one symbol per quantity ([Rules 8 and 9](../Writing/05-Results.md#rules))

| Bad | Good |
|---|---|
| rep rate / repetition rate / FSR / comb spacing; PDCS / soliton / comb | $\nu_\mathrm{rep}^\mathrm{pdcs}$ once defined; PDCS everywhere |

### SI units only ([Notation rule 4](../Writing/07-NotationAndUnits.md#rules))

| Bad (published) | Good (corrected) |
|---|---|
| [...] microring resonators obtained via commercial four-inch wafer foundry fabrication [...] | [...] microring resonators obtained via commercial \qty{100}{\mm} wafer foundry fabrication [...] |

### dBm is not an SI unit ([Notation rule 5](../Writing/07-NotationAndUnits.md#rules))

| Bad | Good (published) |
|---|---|
| [...] with all comb teeth between the two octave-separated pump lasers above \qty{-60}{\dBm}. | [...] with all comb teeth between the two octave-separated pump lasers above \qty{1}{\nW} (i.e., \qty{-60}{\dBm}). |
