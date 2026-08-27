# Prompt: RST-Based Paragraph and Section Analysis

## Role

Act as a careful analyst of scholarly prose using **Rhetorical Structure Theory (RST)**. Analyze the internal rhetorical structure of every paragraph in the paper section supplied below, evaluate how effectively each paragraph performs its apparent function, and suggest targeted improvements. Then analyze how the paragraphs work together as a section.

Your analysis must be **reconstruction-first**: determine as faithfully as possible what the existing text is doing before evaluating or revising it. Do not assume that every paragraph should follow a claim–evidence pattern. Background, literature-review, methodological, procedural, descriptive, results, and transitional paragraphs should be judged according to their actual purposes.

## Inputs

The following may be supplied with the section:

- **Paper title:** optional
- **Paper genre or discipline:** optional
- **Paper-level research question or thesis:** optional
- **Preceding/following section context:** optional
- **Section heading:** preserve exactly
- **Section text:** required

If optional context is absent, infer cautiously from the supplied section and mark important uncertainty. Do not invent content from the rest of the paper.

---

## Core RST Conventions

1. Number paragraphs consecutively as `¶1`, `¶2`, `¶3`, and so forth.
2. Within each paragraph, number sentences as `S1`, `S2`, and so forth.
3. Segment sentences into **elementary discourse units (EDUs)** when an independent or dependent clause makes a distinct rhetorical contribution. Number them `[1]`, `[2]`, and so forth within each paragraph.
4. Do not over-segment complement clauses, restrictive relative clauses, or other embedded material that does not perform a separable rhetorical function.
5. Use:
   - `N` for **nucleus**: the more central span in a nucleus–satellite relation.
   - `S` for **satellite**: a span that performs a rhetorical function relative to a nucleus.
   - `SPAN [x–y]` for a recursively grouped sequence of EDUs.
6. For directed relation ledgers, use the convention:

   ```text
   Satellite --RELATION--> Nucleus
   ```

7. Mark relations such as `JOINT`, `LIST`, `SEQUENCE`, and `CONTRAST` as **multinuclear** when neither span is subordinate.
8. Choose relation names according to the apparent intended effect of one span upon another. Common relations include:

   - `EVIDENCE`
   - `BACKGROUND`
   - `ELABORATION`
   - `INTERPRETATION`
   - `EVALUATION`
   - `CAUSE` or `RESULT`
   - `CONDITION`
   - `PURPOSE`
   - `MOTIVATION`
   - `ENABLEMENT`
   - `SOLUTIONHOOD`
   - `CONCESSION`
   - `ANTITHESIS`
   - `JUSTIFY`
   - `PREPARATION`
   - `SUMMARY`
   - `RESTATEMENT`
   - `JOINT`, `LIST`, `SEQUENCE`, or `CONTRAST` for multinuclear structures

9. If another relation is necessary, define it before using it.
10. When two or more analyses are reasonably plausible, present the leading analysis and briefly identify the strongest alternative. Do not conceal genuine ambiguity.

---

## Analytical Procedure

Perform the following stages in order.

### Stage 1: Establish the section context

Before analyzing individual paragraphs:

1. State the section's apparent purpose in the paper.
2. State the section-level point, outcome, or understanding that the reader is apparently meant to reach.
3. Identify the genre of work the section appears to perform, such as background, literature synthesis, problem definition, theoretical argument, methods, results, interpretation, or recommendation.
4. Identify any contextual uncertainty that limits the analysis.

Do not score the section yet.

### Stage 2: Analyze every paragraph internally

For each paragraph, use all of the following components.

#### A. Paragraph contribution

Provide:

```text
¶# — [concise propositional gloss of the paragraph's principal contribution]
Apparent function: [what the paragraph is doing in the section]
```

The gloss must state the paragraph's contribution, not merely its topic.

#### B. Sentence and EDU segmentation

Reproduce the paragraph divided into sentences and EDUs:

```text
S1
[1] ...
[2] ...

S2
[3] ...
```

Preserve the original wording. Do not silently rewrite it during segmentation.

Then provide a brief propositional gloss for each EDU:

```text
[1] — ...
[2] — ...
```

#### C. Plain-text RST tree

Represent the paragraph's leading analysis recursively. For example:

```text
PARAGRAPH SPAN [1–6]
Relation: EVIDENCE
│
├── N: [1] — [central proposition]
└── S: SPAN [2–6] — [function relative to nucleus]
    │
    └── Relation: CONCESSION
        ├── S: [2] — ...
        └── N: SPAN [3–6] — ...
```

Indentation must represent rhetorical dependency, not merely sentence order.

#### D. Relation ledger

For every material relation, identify the spans and intended effect:

```text
R1  [satellite] --RELATION--> [nucleus]
    Intended effect: [what recognizing the satellite is apparently
    intended to do for the reader in relation to the nucleus]
```

For multinuclear relations, write:

```text
R2  [span] ==CONTRAST== [span]
    Combined function: ...
```

#### E. Structural diagnosis

Identify what works and what may impede the paragraph's rhetorical effectiveness. Base every diagnosis on the reconstructed structure. Consider, when relevant:

- clarity and placement of the nucleus;
- whether each EDU has a recoverable function;
- missing or weakly signaled relations;
- misleading discourse markers or transitions;
- unsupported or insufficiently developed nuclei;
- evidence without interpretation;
- concessions without adequate responses;
- ambiguous attachment of clauses or sentences;
- excessive nesting or processing burden;
- competing nuclei or multiple paragraph purposes;
- repetition that functions as useful restatement versus unnecessary redundancy;
- whether the paragraph should be divided or combined with another paragraph.

Do not label complexity as a defect merely because the tree is deep. Explain the concrete reader difficulty produced by the structure.

#### F. Paragraph strength rating

Rate the paragraph on five dimensions from 1 to 5:

| Dimension | Diagnostic question |
|---|---|
| **Nuclear clarity** | Is the paragraph's central contribution identifiable and appropriately placed? |
| **Relational coherence** | Can each material EDU be connected to the paragraph through a plausible rhetorical relation? |
| **Relation signaling** | Are important relations sufficiently clear from wording, syntax, and discourse markers? |
| **Development and support** | Are central propositions adequately elaborated, supported, interpreted, or qualified for the paragraph's function? |
| **Focus and economy** | Does the paragraph perform its function without avoidable competition, digression, or redundancy? |

Use this scale consistently:

```text
5 — Strong: clear and effective; no material structural revision needed
4 — Effective: coherent, with one or two minor opportunities for improvement
3 — Adequate but uneven: understandable, with at least one substantive structural weakness
2 — Weak: significant difficulty recovering the intended contribution or relations
1 — Seriously impaired: no stable organizing nucleus or coherent structure is recoverable
```

Report:

```text
Nuclear clarity:         #/5
Relational coherence:    #/5
Relation signaling:      #/5
Development and support: #/5
Focus and economy:       #/5
Total:                  ##/25

Overall classification:
22–25 Strong
18–21 Effective
14–17 Adequate but uneven
10–13 Weak
 5–9  Seriously impaired
```

Give a concise justification for every score below 5. Scores must follow from identified textual evidence rather than general impressions.

#### G. Targeted improvement options

Suggest the smallest changes likely to resolve the diagnosed problems. Distinguish among options such as:

- clarify or reposition the nucleus;
- add an explicit relational bridge;
- replace a misleading transition;
- add interpretation after evidence;
- qualify a claim;
- respond to an acknowledged limitation;
- remove, relocate, or integrate an unattached EDU;
- reorder spans;
- divide an overloaded paragraph;
- combine an underdeveloped paragraph with an adjacent one.

For every recommendation, state:

```text
Problem addressed:
Recommended operation:
Expected structural effect:
```

You may offer short example wording for a missing bridge or transition, but do **not** rewrite the entire paragraph unless explicitly requested. Preserve the author's substantive position and disciplinary terminology.

### Stage 3: Analyze relations among paragraphs

After completing every paragraph-level analysis, return to the section as a whole.

#### A. Paragraph ledger

List the paragraphs in original order:

```text
¶1 — [principal contribution]
¶2 — [principal contribution]
¶3 — [principal contribution]
```

#### B. Section-level RST tree

Treat paragraphs or paragraph spans as the units and construct a plain-text RST tree:

```text
SECTION SPAN ¶1–¶8
Relation: [top-level relation]
│
├── N: SPAN ¶1–¶5 — ...
└── S: SPAN ¶6–¶8 — ...
```

Preserve paragraph order while representing rhetorical hierarchy. If a paragraph performs important functions for more than one non-nested span and the structure cannot be represented faithfully as a single tree, identify the cross-connection separately rather than duplicating or concealing it.

#### C. Section relation ledger

Record the principal paragraph- and span-level relations:

```text
¶2 --EVIDENCE--> ¶1
SPAN ¶3–¶5 --ELABORATION--> ¶2
¶7 --CONCESSION--> SPAN ¶1–¶6
```

#### D. Section-level diagnosis

Evaluate:

- whether the section has a clear nucleus or communicative outcome;
- whether every paragraph contributes to that outcome;
- whether paragraph order supports comprehension;
- whether transitions accurately signal paragraph relations;
- whether important argumentative or explanatory bridges are missing;
- whether background, evidence, interpretation, qualification, and closure are appropriately balanced for this section's genre;
- whether paragraphs duplicate, compete with, or interrupt one another;
- whether the section prepares the reader for what follows.

Identify both strengths and weaknesses. Distinguish a genuine structural problem from a merely unconventional but intelligible organization.

#### E. Section strength rating

Rate the section from 1 to 5 on each dimension:

| Dimension | Diagnostic question |
|---|---|
| **Section nucleus** | Is the section's principal contribution clear? |
| **Paragraph integration** | Does each paragraph have a recoverable role in the section? |
| **Progression and ordering** | Does the sequence support the intended rhetorical development? |
| **Cross-paragraph signaling** | Are relations among paragraphs sufficiently signaled? |
| **Development and balance** | Are necessary functions adequately developed for the section's genre? |
| **Closure and forward connection** | Does the section consolidate its contribution and connect appropriately to what follows? |

Report the six scores and a total out of 30:

```text
26–30 Strong
21–25 Effective
16–20 Adequate but uneven
11–15 Weak
 6–10 Seriously impaired
```

Justify every score below 5.

#### F. Prioritized section improvement plan

Provide a numbered list ordered by likely impact. For each recommendation, identify:

1. the affected paragraph(s) or span;
2. the structural problem;
3. the recommended operation;
4. the expected improvement in the section-level RST structure.

Conclude with a proposed **revision outline**, not a rewritten section. Show the intended role and order of paragraphs after revision:

```text
PROPOSED REVISION OUTLINE

¶1 — Establishes ...
¶2 — Provides evidence for ¶1 ...
¶3 — Interprets that evidence ...
¶4 — Addresses the principal qualification ...
¶5 — Consolidates the section's contribution ...
```

Clearly mark whether each proposed paragraph is retained, moved, divided, combined, substantially revised, or newly needed.

---

## Evaluation Boundaries

Maintain these distinctions throughout:

1. **Rhetorical coherence is not factual correctness.** Do not infer that a claim is true because it occupies a clear structural position.
2. **Rhetorical support is not necessarily logical or empirical sufficiency.** You may flag an apparent support gap, but do not conduct methodological, statistical, or source-quality appraisal unless separately requested.
3. **Reader difficulty must be explained.** Do not call a structure “unclear,” “awkward,” or “weak” without identifying the exact span, relation, or attachment problem.
4. **Do not force every paragraph into an argumentative template.** Judge descriptive and methodological paragraphs by how effectively they describe, specify, sequence, delimit, or enable understanding.
5. **Do not invent authorial intentions.** Describe intentions as plausible interpretations supported by the text.
6. **Prefer minimal revision.** Recommend wholesale rewriting only when local structural corrections cannot reasonably solve the problem.
7. **Preserve substantive meaning.** Do not change the author's conclusion, evidentiary claims, level of certainty, or disciplinary terminology without explicitly identifying the proposed substantive change.
8. **Acknowledge analytical uncertainty.** If segmentation, nuclearity, or relation choice is ambiguous, state that ambiguity and explain its implications for evaluation.

---

## Required Output Order

Use exactly this overall sequence:

```text
1. SECTION CONTEXT AND APPARENT PURPOSE

2. PARAGRAPH-BY-PARAGRAPH ANALYSIS
   ¶1
   - Contribution and function
   - Sentence/EDU segmentation
   - EDU glosses
   - RST tree
   - Relation ledger
   - Structural diagnosis
   - Strength rating
   - Improvement options

   ¶2
   [repeat for every paragraph]

3. SECTION-LEVEL ANALYSIS
   - Paragraph ledger
   - Section RST tree
   - Section relation ledger
   - Strengths
   - Structural problems
   - Section strength rating

4. PRIORITIZED REVISION PLAN

5. PROPOSED REVISION OUTLINE

6. ANALYTICAL UNCERTAINTIES AND LIMITS
```

---

## Material to Analyze

```text
PAPER TITLE (optional):

PAPER GENRE OR DISCIPLINE (optional):

PAPER-LEVEL RESEARCH QUESTION OR THESIS (optional):

PRECEDING/FOLLOWING CONTEXT (optional):

SECTION HEADING:

SECTION TEXT:
[Paste the complete paper section here.]
```
