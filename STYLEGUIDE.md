# Writing conventions

These conventions are meant to make notes easy to read and verify, not to impose a rigid style on each course.

## Mathematical writing

1. State every theorem with its hypotheses and quantifiers. Do not silently strengthen a theorem.
2. Define symbols before first use, especially the domain, codomain, index sets, and measure spaces.
3. Keep the notation of the course or reference where practical. Mention any departures.
4. Distinguish an original argument, a standard fact, and a result quoted from a source.
5. For an exercise, preserve the problem statement exactly when transcribing it.
6. Do not skip a logically necessary step merely to shorten a proof.
7. Mark gaps as **Open step**, **To verify**, or **Incomplete proof**.

## Recommended structure

- **Definition / Theorem / Proposition / Lemma / Corollary**
- **Proof**
- **Remark / Example / Counterexample**
- **References**

Within a course, retain its theorem numbering when citing the textbook, e.g. “Theorem 3.2 of [1]”, and do not invent an established name for a result.

## Markdown mathematics

Inline: `$f \in L^p(\Omega)$`.

Display:

```text
$$
\|f\|_{L^p(\Omega)}
= \left(\int_\Omega |f|^p\,dx\right)^{1/p}.
$$
```

Prefer a single math display for a connected calculation. Explain any nontrivial inequality or change of variables.

## Sources and attribution

Add a **References** section when a note relies on a book, article, or lecture. Record author, title, and theorem/page/section when known. Avoid uploading copyrighted source material or unpublished collaborative work without permission.

## Privacy

This repository is public. Keep unpublished drafts, private advisor correspondence, and potentially publishable arguments in a private repository until cleared for public release.
