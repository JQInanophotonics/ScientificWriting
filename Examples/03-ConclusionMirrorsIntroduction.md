# Example 3: The conclusion mirrors the introduction

This example applies [06 — The conclusion closes the loop and opens](../Writing/06-Conclusion.md) from the [main guide](../README.md). Each block names the rule, then puts a sentence of the introduction next to the sentence of the conclusion that answers it. All sentences are as published.

## Papers

- Self-aligned PDCS: Grégory Moille *et al.*, [*Self-aligned optical microcomb emerging between octave separated lasers*](https://doi.org/10.1038/s41586-026-11086-2), Nature **658**, 350–357 (2026).
- PDCS: Grégory Moille *et al.*, *Parametrically driven pure-Kerr temporal solitons in a chip-integrated microcavity*, Nature Photonics (2024).
- KIS: Grégory Moille *et al.*, *Kerr-induced synchronization of a cavity soliton to an optical reference*, Nature (2023).
- AC-KIS: *Toward chaotic group velocity hopping of an on-chip dissipative Kerr soliton*, Physical Review Letters (2025).
- TRN: *All-optical noise quenching of an integrated frequency comb*, Optica (2025).
- Self-balancing: *DKS self-balancing from Kerr-induced synchronization*, Physical Review A (2026).

### Answer the problem, in its words ([Rule 1](../Writing/06-Conclusion.md#rules))

| Introduction | Conclusion |
|---|---|
| `However, while DKS combs have proven their effectiveness in numerous applications, their outward cascading from a low-power seed pump laser leads to fundamental metrology limitations: Octave-spaced signals at the comb edges are typically very weak and noisy (due to thermo-refractive fluctuations), which critically hinders the detection and stabilization of the CEO.` (Self-aligned PDCS) | `Our self-aligned PDCS microcomb operates significantly differently from standard DKS microcombs that rely on outward cascading from a centred single pump laser, which results in weak and noisy signals at the comb edges, thus complicating the CEO detection and locking required for precision metrology.` |
| `A natural question that arises is: is it possible to generate PDCSs in foundry-ready, pure-Kerr resonators with bichromatic driving?` (PDCS) | `We have shown theoretically, numerically, and experimentally that dispersive resonators with a purely Kerr-type $\chi^{(3)}$ nonlinearity can support parametrically driven cavity solitons under conditions of bichromatic driving.` |
| `However, thus far this model has only demonstrated qualitative agreement in the KIS DC regime, and its second-order temporal derivative---crucial for chaotic DKS---remains experimentally unverified.` (AC-KIS) | `In conclusion, our combined experimental and theoretical work quantitatively verifies that the second-order Adler model accurately describes KIS DKS dynamics.` |
| `We show that by simply changing how the input lasers are locked, the same self-aligned PDCS can perform the three core tasks of self-referenced OFCs [...]` (Self-aligned PDCS) | `We demonstrate the benefit of this versatility by performing three key tasks for integrated OFC systems [...]` |

### Take back each limitation, removed ([Rule 2](../Writing/06-Conclusion.md#rules))

| Introduction | Conclusion |
|---|---|
| `noise on the external CW laser can degrade the coherence of nearby comb lines` (PDCS) | `[...] could result in fundamental advantages to noise characteristics.` |
| `removal of the CW background may require careful spectral filtering` (PDCS) | `Moreover, the lack of a dominating CW component at the PDCS carrier frequency alleviates the need for careful spectral shaping [...]` |
| `applications that require coexistence of distinguishable binary elements are fundamentally beyond reach.` (PDCS) | `Finally, the fact that PDCSs come in two forms with opposite phase opens the doors to a new range of applications that require a binary degree of freedom, including all-optical random number generation and realisations of coherent optical Ising machines.` |
| `these integrated microcombs fall short in their repetition rate noise performance - primarily due to their poor ability to manage the cavity thermorefractive noise (TRN), which increases inversely with the resonator size.` (TRN) | `Our work demonstrates that despite the low modal volume of integrated microcombs, which makes them predisposed to large TRN that can greatly hinder their performance, KIS can enable ultra-low-noise performance [...]` |

### Recap each result, in order, with its number ([Rule 3](../Writing/06-Conclusion.md#rules))

| Results section | Conclusion |
|---|---|
| `Self-balancing in purely quadratic dispersion resonators` (Self-balancing) | `In the simplest quadratic-dispersion system, this manifests as a spectral recoil on the opposite side of the optical spectrum to the reference pump.` |
| `Self-balancing effect in presence of a dispersive wave` (Self-balancing) | `Extending our analysis to systems that include higher-order dispersion, we showed that this same self-balancing mechanism transfers energy into a DW on the opposite side of the spectrum, leading to measurable power enhancement without changing the repetition rate.` |
| `Dispersive wave enhancement with quartic dispersion` (Self-balancing) | `For a quartic-dispersion resonator supporting two DWs, we showed that synchronizing the soliton at the low-frequency DW results in significant self-balancing-induced enhancement of the high-frequency DW power.` |
| No section titles (TRN) | `The repetition rate noise is suppressed by more than four orders of magnitude compared to free-running single pumped-DKS, and is about an order of magnitude lower than the minimum TRN that the singly-pumped DKS could exhibit in our system.` |

### Return to the stakes of the first paragraph ([Rule 4](../Writing/06-Conclusion.md#rules))

| Introduction | Conclusion |
|---|---|
| `the power budget and limited bandwidth associated with such active stabilization represents a barrier to full integration of an optical clock` (KIS) | `Our work is an important step toward compact optical clocks for fieldable applications in positioning, navigation, and timing, both through decreased power budget and a simplified architecture [...]` |
| `The analogy between optical and mechanical clocks in which the OFC is likened to gears is often drawn [...]` (KIS) | `Analogous to mechanical clockworks, passive synchronization is enabled by direct coupling to the reference.` |
| `Rather than an obstacle, optical chaos enables high-speed random number generation, secure communication, and reservoir computing.` (AC-KIS) | `Our work presents a new tool for generating optical chaos on a low-power, on-chip platform, harnessing a single low-noise DKS with the secure randomness of chaotic systems.` |

### State the limitation that remains ([Rule 5](../Writing/06-Conclusion.md#rules))

| Limitation | Why it is not fundamental |
|---|---|
| `Although detecting our large repetition rate currently requires a phase modulator apparatus for downconversion,` (Self-aligned PDCS) | `this high repetition rate is an integral part of the architecture. For a self-referenced platform, a large repetition rate prevents pump power from being diluted into densely packed comb teeth spread across the entirety of the spectrum, most of which serve no metrological purpose.` |

### Say what the work makes possible ([Rule 6](../Writing/06-Conclusion.md#rules))

| Introduction | Conclusion |
|---|---|
| `Crucially, because the octave-separated pumps are both comb lines (when operating in the self-alignment regime), the CEO of the subsequently generated PDCS is \textit{a priori} determined before the chip from the harmonic offset between the pumps, enabling flexible interfacing with microwave and optical frequency references.` (Self-aligned PDCS) | `Moving forward, our self-aligned PDCS enables several integration capabilities, many arising from the stabilized, octave-separated pumps that remain available for further use. For example, the system is highly suitable for integrated SHG of the negative pump for high signal-to-noise ratio CEO detection.` |
| `Importantly, this second-order equation describes a physical coupling mechanism through phase modulation that enables a path to chaos.` (AC-KIS) | `While our demonstration uses a phase-modulated injected reference, the Adler model remains agnostic to which oscillator is modulated, suggesting these observations would apply to breather states.` |
