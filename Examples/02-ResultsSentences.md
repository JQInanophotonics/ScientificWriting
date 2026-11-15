# Example 2: Results sentences, bad and published

## Paper

Grégory Moille *et al.*, [*Self-aligned optical microcomb emerging between
octave separated lasers*](https://arxiv.org/abs/2602.05151), arXiv:2602.05151
(2026). [PDF](https://arxiv.org/pdf/2602.05151) |
[DOI](https://doi.org/10.48550/arXiv.2602.05151)

This example applies [05 — The Results section](../Writing/05-Results.md) from the
[main guide](../README.md).

## Bad and published sentences

Each left cell names the rule it breaks, in bold, then a sentence written badly on purpose with a fault that is common in drafts. Each right cell is the sentence as published.

| Bad | Good (published) |
|---|---|
| **[Notation](../Writing/07-NotationAndUnits.md): `\qty` with `\approx`, never `\sim`. [Rule 10](../Writing/05-Results.md#rules): define every symbol ($n_\pm$).**<br>The pump frequencies $\nu_-\sim 193$ THz and $\nu_+\sim 387$ THz are almost separated by an octave, which is where the dispersion is good. | `The dispersion conditions are satisfied at \qty{\nu_- \approx 193}{\THz} ($n_-=263$, C-band) and \qty{\nu_+ \approx 387}{\THz} ($n_+=2n_-=526$, visible) (\cref{fig:2}a).` |
| **[Rule 5](../Writing/05-Results.md#rules): describe the device once; the details go to Methods.**<br>The fabrication of the microrings was done by a commercial foundry and consists of several deposition, lithography, etching and cladding steps, and the bus waveguide was designed by changing its width and gap so that it couples light over more than an octave. | `We demonstrate the above concept experimentally using silicon nitride (\ce{Si_3N_4}) microring resonators obtained via commercial four-inch wafer foundry fabrication, with a bus waveguide designed to couple across more than an octave (\cref{fig:1}b; see Methods).` |
| **[Rule 3](../Writing/05-Results.md#rules): start every measurement with why it is done.**<br>The output of the chip is then sent to an OSA and to a photodiode to look at the beat between the PDCS and the pump comb. | `We demonstrate self-alignment by directly measuring $\Delta\nu_\mathrm{ceo}$ between the PDCS and $\nu_+$ pump comb (see Methods and Supplementary Information S.5).` |
| **[Rule 11](../Writing/05-Results.md#rules): write the symbol, here the relation, instead of the words.**<br>When the pumps are appropriately set, the PDCS can enter in the self-aligned regime, where it becomes aligned to the pumps, allowing for metrology applications. | `In a self-aligned PDCS, both pumps are comb teeth that pin $\nu_\mathrm{rep}^\mathrm{pdcs}=(\nu_+-\nu_-)/(n_+-n_-)$.` |
| **[Rule 14](../Writing/05-Results.md#rules): always `\cref`. [Rule 10](../Writing/05-Results.md#rules): define every symbol ($N$).**<br>Optical frequency division is demonstrated on figure \ref{fig:2}(d), where the slope is $1/N$. | `The repetition rate therefore depends linearly on the pump detunings $\delta\nu_\pm$, with opposite signs for positive- and negative-pump actuation and slope magnitude $1/N=1/(n_+-n_-)=1/n_-$ corresponding to the optical frequency division (OFD) factor (\cref{fig:2}d).` |
| **[Rule 4](../Writing/05-Results.md#rules): end with the number, compared to the reference.**<br>The rep rate linewidth is much narrower once the soliton is self-aligned, as can be seen on figure \ref{fig:2}(e). | `Due to self-alignment, the repetition rate noise depends only on the pump frequency noises, reducing its \qty{3}{\dB} linewidth from \qty{70}{\kHz} for the free-running case with three comb components to \qty{1.8}{\kHz} (\cref{fig:2}e).` |
| **[Rule 6](../Writing/05-Results.md#rules): state every limit with where it happens and why.**<br>The division is confirmed experimentally at low frequency. At higher frequencies, this is not true anymore. | `[…] the lasers' long-term frequency drift prevents extended averaging. As a result, the noise floor exceeds the OFD of the laser noise above \qty{10}{\kHz}, which future work will improve.` |
| **[Rule 3](../Writing/05-Results.md#rules): start with why the measurement is done. [Rule 7](../Writing/05-Results.md#rules): compare under the same conditions, and say which.**<br>Both Allan deviations (PDCS/fiber comb) being identical, this shows that the PDCS works as a clockwork. | `To confirm that the self-aligned PDCS acts as a true clockwork, we perform a second experiment a day later in which we locked a fiber comb's CEO and one comb tooth to the clock laser, achieving identical Allan deviation performance except at \qty{\tau<1}{\s}, where the PDCS repetition rate noise is dominated by the EOcomb downconverter.` |
| **[Rules 8 and 9](../Writing/05-Results.md#rules): one name per object, one symbol per quantity.**<br>rep rate / repetition rate / FSR / comb spacing; PDCS / soliton / comb | `$\nu_\mathrm{rep}^\mathrm{pdcs}$` once defined, and "PDCS" everywhere. |
