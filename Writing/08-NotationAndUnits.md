# 08 — Notation and units

Every value in a paper is written the same way. The reader should never notice how a number was typeset.
These rules come from the self-aligned PDCS paper (Nature 2026) and the KIS interlocking draft.

## The siunitx setup

The group's class (`MoillePaper.cls`) loads `siunitx` with these options. Use them as given, and do not reset them in the paper.

```latex
\usepackage[per-mode=power,
            exponent-product = \times,
            inter-unit-product = \ensuremath{{\cdot}},
            tight-spacing = true,
            number-unit-product=~,
            parse-numbers=false,]{siunitx}
\AtBeginDocument{\RenewCommandCopy\qty\SI}
\ExplSyntaxOn
\msg_redirect_name:nnn { siunitx } { physics-pkg } { none }
\ExplSyntaxOff
```

| Option | Effect |
|--------|--------|
| `per-mode=power` | `\qty{-140}{dBc\per\Hz}` prints dBc·Hz⁻¹, not dBc/Hz |
| `exponent-product = \times` | Scientific notation uses ×, not · |
| `inter-unit-product = \ensuremath{{\cdot}}` | A centered dot between units |
| `number-unit-product=~` | A non-breaking space between the value and its unit |
| `parse-numbers=false` | The number argument is printed as written, so it can hold symbols and relations |
| `\RenewCommandCopy\qty\SI` | Keeps `\qty` from `siunitx` when the `physics` package is loaded |

A journal template without the class needs the same block in its preamble. Declare missing units once in the preamble, for example
`\DeclareSIUnit[qualifier-mode = combine]{\dBm}{\deci\bel\of{m}}`.

## Rules

1. **Every value with a unit goes through `\qty{}{}`.** Never type `283 THz` or `283~THz`.

2. **Write the whole relation inside `\qty`.** The symbol, the relation and the value go in the first argument, and the unit lands after them with the right spacing.

   ```latex
   \qty{\nu_0 \approx 283}{\THz}
   \qty{R = 22.98}{\um}
   \qty{\tau < 1}{\s}
   \qty{> 2}{\GHz}
   ```

   Do not split it as `$\approx$~\qty{26}{\kHz}`. Write `\qty{\approx 26}{\kHz}`.

3. **Use unit macros, never text.** Write `\qty{800}{\nm}`, not `\qty{800}{nm}`. Pick one form per paper: `\mW` everywhere, not `\mW` in one place and `\milli\watt` in another. Write percentages as `\qty{5}{\percent}`, not `5\%`.

4. **Use SI units only.** Never inches, mils or feet. Write `\qty{100}{\mm} wafer`, not "four-inch wafer".

5. **dBm is not an SI unit.** In a figure, label the axis in dB and state the reference in the caption: "Power normalized to \qty{1}{\mW} (\qty{}{\dBm})."

6. **Approximately equal is `\simeq` or `\approx`, never `\sim`.** `\sim` means "of the order of" or "scales as". Use one of the first two throughout a paper.

7. **Never use e-notation.** With `parse-numbers=false`, `\num{3e3}` prints "3e3" in the PDF. Write `$3\times10^{3}$` or `\num{3\times10^{3}}`.

8. **Frequency first, wavelength in parentheses.**

   ```latex
   pumped at \qty{\approx 283}{\THz} (\qty{1060}{\nm})
   ```

9. **Round value in the text, exact value in parentheses on first use.**

   ```latex
   a microcomb of $\nu_\mathrm{rep}$ \qty{\approx 109}{\GHz} (\qty{109.516441235}{\GHz})
   ```

10. **Keep the same precision for the same quantity.** Do not write `\qty{316.20}{\mW}` in one place and `\qty{316.2}{\mW}` in another.

11. **Math mode: sub- and superscripts on a symbol use `_` and `^`.** A descriptive label is upright with `\mathrm`, a variable index is italic.

   ```latex
   $\nu_\mathrm{rep}$, $\nu_\mathrm{ceo}$, $Q_\mathrm{c}$    % labels: upright
   $\nu_n$, $P_\pm$, $\chi^{(3)}$                     % variables: italic
   ```

   Use `\mathrm`, not `\textrm` or `\text`. Write a given subscript the same way everywhere: not `Q_\mathrm{c}` in one sentence and `Q_c` in the next, nor `\nu_{ceo}` beside `\nu_\mathrm{ceo}`.

12. **Text mode: sub- and superscripts on a word use `\textsubscript` and `\textsuperscript`.** This covers ordinals, mode labels and state names.

    ```latex
    the $m$\textsuperscript{th} sideband
    the k\textsuperscript{th} comb tooth
    the TE\textsubscript{0} mode
    the 5S\textsubscript{1/2} state
    ```

    Never write `TE$_0$` or `5S$_{1/2}$`: math mode switches the font and the spacing in the middle of a word.

13. **Use `\times` for products and `\nicefrac` for inline ratios.**

    ```latex
    an OFD factor of 801 ($89 \times 9$)
    $\nicefrac{K}{M}$
    ```

14. **Chemical formulas and isotopes use `\ce{}` from `mhchem`.** Load `\usepackage[version=4]{mhchem}`. Digits become subscripts automatically, so write `\ce{Si3N4}`, not `\ce{Si_3N_4}` or `Si$_3$N$_4$`.

    ```latex
    \ce{Si3N4}, \ce{SiO2}, \ce{SiN}, \ce{LiNbO3}
    \ce{^{87}Rb}                                  % isotope
    ```

## Before submission

Search the `.tex` for the slips these rules forbid:

```bash
grep -nE '[0-9] ?(nm|GHz|THz|MHz|kHz|mW|dB)\b' paper.tex   # units typed as text
grep -nE '\\qty\{[^}]*\}\{[a-zA-Z]' paper.tex             # unit without a macro
grep -nE '\\sim[^e]|\\num\{[0-9.]+e' paper.tex            # \sim, e-notation
grep -nE '_\{[a-z]{2,}\}' paper.tex                        # italic descriptive subscript
grep -nE '[A-Za-z]\$[_^]' paper.tex                         # math sub/superscript glued to a word
grep -nE 'Si\$?_\{?3|SiO\$?_\{?2|(^|[^{])(Si3N4|SiO2)' paper.tex # formula outside \ce, or with _
grep -nE 'inch|[0-9]~?in\b|mil\b' paper.tex                  # non-SI lengths
```

Then read the PDF text for "e3", "e-", and stray `\%`.
