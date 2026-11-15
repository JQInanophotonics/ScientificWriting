# Notation and units

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

4. **Approximately equal is `\simeq` or `\approx`, never `\sim`.** `\sim` means "of the order of" or "scales as". Use one of the first two throughout a paper.

5. **Never use e-notation.** With `parse-numbers=false`, `\num{3e3}` prints "3e3" in the PDF. Write `$3\times10^{3}$` or `\num{3\times10^{3}}`.

6. **Frequency first, wavelength in parentheses.**

   ```latex
   pumped at \qty{\approx 283}{\THz} (\qty{1060}{\nm})
   ```

7. **Round value in the text, exact value in parentheses on first use.**

   ```latex
   a microcomb of $\nu_\mathrm{rep}$ \qty{\approx 109}{\GHz} (\qty{109.516441235}{\GHz})
   ```

8. **Keep the same precision for the same quantity.** Do not write `\qty{316.20}{\mW}` in one place and `\qty{316.2}{\mW}` in another.

9. **Descriptive subscripts are upright, variables are italic.** Write `\nu_\mathrm{rep}`, `f_\mathrm{ceo}`, `Q_\mathrm{c}`, but `\nu_n` or `P_\pm` when the index is a variable. Use `\mathrm`, not `\textrm` or `\text`. Write a given subscript the same way everywhere: not `Q_\mathrm{c}` in one sentence and `Q_c` in the next, nor `f_{ceo}` beside `f_\mathrm{ceo}`.

10. **Use `\times` for products and `\nicefrac` for inline ratios.**

    ```latex
    an OFD factor of 801 ($89 \times 9$)
    $\nicefrac{K}{M}$
    ```

## Before submission

Search the `.tex` for the slips these rules forbid:

```bash
grep -nE '[0-9] ?(nm|GHz|THz|MHz|kHz|mW|dB)\b' paper.tex   # units typed as text
grep -nE '\\qty\{[^}]*\}\{[a-zA-Z]' paper.tex             # unit without a macro
grep -nE '\\sim[^e]|\\num\{[0-9.]+e' paper.tex            # \sim, e-notation
grep -nE '_\{[a-z]{2,}\}' paper.tex                        # italic descriptive subscript
```

Then read the PDF text for "e3", "e-", and stray `\%`.
