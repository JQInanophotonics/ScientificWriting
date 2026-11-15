# 06 — The conclusion closes the loop and opens

The conclusion is the mirror of the introduction. The introduction set up a problem: what the field accepts, what it cannot do, and why that matters. The conclusion answers that problem, point by point and in the same words, then turns outward and says what the answer now makes possible.

Many readers read the abstract, the introduction and the conclusion, and nothing else. For them the conclusion is where the argument ends. If it does not answer the question the introduction asked, the paper reads as a list of measurements rather than a result.

A conclusion therefore does two things, in this order. It **closes the loop**: the problem is answered, the limitations are gone, the stakes are met. Then it **opens**: the work becomes the starting point of what comes next.

## Two formats

The structure depends on the format, not on the content.

### Letters, short papers and conference abstracts

The conclusion is one paragraph, sometimes two, that starts with "In conclusion". It runs through the full sequence:

1. the answer to the problem of the introduction (rule 1);
2. one sentence per result, in the order of the Results, each with its number (rule 3), which also takes back the limitations (rule 2);
3. the limitation that remains, if there is one (rule 5);
4. what the work opens, ending on the stakes of the first paragraph (rules 6 and 4).

In a conference abstract there is no room for the recap. The conclusion is one or two sentences: the answer to the problem, then what it opens.

### Long articles (Nature, Nature Photonics, Communications Physics)

The conclusion is a Discussion section. It does **not** recap the Results; the reader has just read them. Instead it argues:

1. how the work differs from the conventional approach described in the introduction, which is the answer to its problem (rules 1 and 2);
2. the limitation a reviewer would raise, and why it is not fundamental (rule 5);
3. what the work opens, step by step (rule 6);
4. the stakes of the first paragraph, now within reach (rule 4).

The Discussion is longer than a letter's conclusion because each of these points is argued, with citations, rather than stated.

## Rules

### Close the loop

1. **Answer the problem of the introduction, in its words.**
   The introduction ended on something that is missing, unverified, or impossible: a model that only agrees qualitatively, a question nobody has answered, a signal too weak to use. The first sentence of the conclusion states that this is now done.
   - Reuse the nouns and verbs of the introduction. If the introduction wrote that a model "remains experimentally unverified", the conclusion writes that the work "quantitatively verifies" it. The reader must recognize the question without going back.
   - If the introduction asked a question, the conclusion answers that question, not a nearby one.
   - Restate the claim of the last paragraph of the introduction as demonstrated. The Results opened with this claim; the conclusion closes with it (see [05 — The Results section](05-Results.md#from-the-introduction-to-the-results)).

2. **Take back each limitation the introduction listed, and show it removed.**
   The introduction justified the work by listing what the conventional approach cannot do. Each item on that list must come back in the conclusion, now resolved.
   - If the introduction gave three drawbacks, the conclusion answers all three, ideally in the same order. A drawback raised and never answered is a promise the paper did not keep.
   - Give the number and the comparison point the introduction used. If the introduction said an existing method improves the noise by an order of magnitude, the conclusion says by how much this work improves it against that same method.
   - If one limitation is only partly removed, say so here; it becomes the limitation of rule 5.

3. **Recap each result once, in the order of the Results, with its number and its cause.** (Letters only.)
   - One sentence per Results section, in the same order and with the same words as its title or first sentence.
   - Each sentence carries the key number, against its reference: "suppressed by four orders of magnitude compared to the single-pump soliton", not "strongly suppressed".
   - Give the cause in a few words when it is the point of the paper: "because the soliton is phase-locked to the reference".
   - No setup, no new detail, no figure reference. The reader who wants the detail goes back to the Results.

4. **Return to the stakes of the first paragraph of the introduction.**
   The introduction opened with why the field matters: the applications, the community's goal, sometimes an analogy. The conclusion ends there, showing the result has moved the field toward it.
   - Name the same applications, in the same words. If the paper opened with optical clocks and navigation, it closes with optical clocks and navigation, not with a new list.
   - If the introduction used an analogy, the conclusion uses it again to state the result.
   - Say concretely how the work brings the application closer: lower power, a simpler architecture, a chip instead of a table.

### Open

5. **State the limitation that remains, and say why it is not fundamental or how it will be removed.**
   Every result has a weakness a reviewer will point to: a measurement that still needs bulky equipment, a noise floor set by the setup, a parameter not yet optimized. The conclusion names it first.
   - State it plainly, then give the reason it does not undermine the claim: it is technical rather than fundamental, it is a deliberate design choice, or a known technique removes it.
   - When it can be removed, say how, with a citation: better coupling design, locking the lasers, a known integration process.
   - Never hide it. A limitation the reader finds alone weakens the whole paper; one the authors state and answer strengthens it.

6. **Say what the work now makes possible.**
   This is the opening, and it is required: a conclusion that only summarizes has not said why the work matters beyond itself.
   - Go from the nearest step to the farthest: what can be done next with the same device, then what becomes possible in the field, then what other fields may gain.
   - Each step names the mechanism that makes it possible: "because the pumps remain available, they can be frequency-doubled on chip for CEO detection". The mechanism is what makes the opening credible rather than wishful.
   - Cite the work that the next step builds on, so the reader sees the path exists.
   - "Opens new avenues" is fine, followed by which avenues and why this work opens them.

7. **No new result.**
   Everything the conclusion states was shown in the Results or the Methods. A new measurement, simulation or claim in the conclusion has no figure behind it and no place for the reader to check it. If it matters, it belongs in the Results; if it is a perspective, write it as one (rule 6).

## Worked example

[Example 3: The conclusion mirrors the introduction](../Examples/03-ConclusionMirrorsIntroduction.md) shows each rule with sentences from published papers, introduction next to conclusion.

## Before submission

Put the introduction and the conclusion side by side and check:

- Does the first sentence of the conclusion answer the problem the introduction ended on, in the same words?
- Does each limitation listed in the introduction come back, removed, with a number against the same comparison point?
- In a letter: is there one sentence per Results section, in order, each with its number?
- Does the conclusion return to the applications of the first paragraph, in the same words?
- Is the remaining limitation stated, with why it is not fundamental?
- Does it say what the work now makes possible, with the mechanism for each step?
- Is every statement shown in the Results?
