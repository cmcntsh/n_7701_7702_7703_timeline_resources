## Task

Perform a **paragraph-level lightweight argument analysis** of the paper section provided below. Analyze **each paragraph separately** and represent its internal rhetorical/argumentative structure as a small text-based tree.

The purpose is **reverse outlining**, not rewriting or editing. Preserve the author's sentences exactly and identify the function each sentence performs within its paragraph.

## Notation

Use the following labels:

- **I — Issue:** Introduces the question, problem, tension, gap, or issue the paragraph addresses.
- **C — Claim:** Makes a supporting claim, reason, proposition, or assertion that advances the paragraph's reasoning.
- **E — Evidence:** Provides evidence, data, examples, citations, observations, facts, or other support for a claim.
- **A — Analysis:** Interprets evidence or reasoning; explains what it means, why it matters, or how it supports a claim or point.
- **P — Point:** States the paragraph's main takeaway, controlling proposition, conclusion, or argumentative payoff.
- **L — Link:** Connects the paragraph to the preceding/following argument or explicitly performs a transition.

Use numbered labels when a paragraph contains multiple elements of the same type:

`C1`, `C2`, `C3`; `E1`, `E2`; `A1`, `A2`, etc.

Numbers should help show relationships. For example, `E1` should normally be evidence supporting `C1`, and `A1` should normally be analysis associated with that evidence or claim.

## Important Principles

### 1. Analyze the paragraph as written

Do **not** impose an idealized `I → C → E → A → P` structure on every paragraph.

A paragraph may legitimately have a structure such as:

```text
P
├── C1
└── C2
    └── E2
```

or:

```text
I
├── C1
│   └── E1
├── C2
│   └── E2
└── P
```

or simply:

```text
I
└── P
```

Missing elements are analytically meaningful. Do not invent an Issue, Evidence, Analysis, Point, or other function merely to complete the framework.

### 2. Use the author's sentences

Place the **complete original sentence** after its label.

Do not paraphrase, summarize, rewrite, correct, or shorten the sentence.

### 3. Assign function based on what the sentence does

Classify sentences according to their **rhetorical or argumentative function in that particular paragraph**, not merely according to their grammatical form.

For example, a sentence containing a citation is not automatically Evidence. It may make a Claim supported by an external source.

Similarly, a sentence describing a fact may function as Evidence if that fact supports another proposition in the paragraph.

### 4. Represent relationships, not merely sequence

The tree should show **which sentences support, explain, or develop other sentences**.

For example:

```text
C1
├── E1
└── A1
```

means that E1 and A1 develop or support C1.

Do not simply place every sentence beneath the preceding sentence because it occurs next in the paragraph.

### 5. Allow the Point to occur anywhere

Do not assume that `P` must be the final sentence.

A deductively organized paragraph may state its main point first:

```text
P
├── C1
│   └── E1
└── C2
```

An inductively organized paragraph may build toward it:

```text
I
├── E1
├── E2
└── P
```

Determine the structure from the paragraph itself.

### 6. Distinguish Claim, Evidence, and Analysis carefully

Use these diagnostic questions:

**Claim (C):**  
What proposition is the author asking the reader to accept?

**Evidence (E):**  
What information gives the reader a reason to accept that proposition?

**Analysis (A):**  
What explains the significance, meaning, implication, or relevance of the evidence or reasoning?

A useful relationship is often:

```text
C
├── E
└── A
```

but do not require this pattern.

### 7. Distinguish Issue from Point

The **Issue** identifies what needs to be addressed.

The **Point** states what the paragraph ultimately wants the reader to understand or accept about that issue.

For example:

```text
I  Previous studies disagree about whether X causes Y.
│
├── E1  Study A found...
├── E2  Study B found...
└── P   The disagreement is best explained by differences in...
```

### 8. Use Link sparingly

Use `L` only when a sentence genuinely performs an important connective or transitional function between this paragraph and the surrounding argument.

Do not label ordinary introductory sentences as `L` merely because they occur at the beginning of a paragraph.

### 9. Handle sentences with multiple functions conservatively

Prefer assigning **one primary function per sentence**.

If a sentence genuinely performs two inseparable functions, a combined label such as `E1/A1` may be used, but only when assigning a single primary function would materially misrepresent the sentence.

Do not split a sentence into clauses unless necessary to understand the paragraph's structure.

## Output Format

Analyze every paragraph in order.

For each paragraph, provide:

**Paragraph [number]**

```text
[argument tree containing the complete original sentences]
```

Then provide a brief **Structural note** of approximately 1–3 sentences explaining any important feature or ambiguity in the mapping. Focus especially on unclear relationships, missing rhetorical functions, or sentences that could reasonably receive more than one label.

For example:

**Paragraph 1**

```text
P  [complete original sentence]

├── C1  [complete original sentence]
│   └── E1  [complete original sentence]
│
└── C2  [complete original sentence]
        └── E2  [complete original sentence]
```

**Structural note:** The first sentence functions as the paragraph point rather than merely as an introduction because it states the controlling proposition that the remaining sentences develop. The final sentence functions as evidence for C2 because it specifies the concrete activities supporting that claim.

## Cross-Paragraph Summary

After analyzing all paragraphs individually, provide a compact summary showing only the structural signatures:

```text
Paragraph 1: P → {C1, C2 → E2}
Paragraph 2: I → {C1 → E1, C2 → E2} → P
Paragraph 3: L → P → {C1 → E1}
...
```

Then identify any **structural patterns worth reviewing**, such as:

- paragraphs with no identifiable Point;
- paragraphs containing claims without support;
- evidence whose relationship to a claim is unclear;
- paragraphs dominated by Evidence but lacking Analysis;
- paragraphs with multiple competing Points;
- paragraphs whose Issue is implicit or unclear;
- paragraphs in which the Point does not appear to follow from the preceding material;
- unusually complex paragraphs that may contain more than one argumentative unit.

Treat these as **diagnostic observations, not automatic writing defects**. Do not recommend revisions unless explicitly asked.

## Paper Section to Analyze

[PASTE PAPER SECTION HERE]