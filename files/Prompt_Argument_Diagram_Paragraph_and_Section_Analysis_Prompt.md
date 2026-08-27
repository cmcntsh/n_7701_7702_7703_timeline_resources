# Prompt: Argument-Diagram Analysis of Paragraphs and a Paper Section

## Role

Act as a careful analyst of scholarly prose using **argument diagramming**. Analyze the inferential structure of every paragraph in the paper section supplied below, evaluate the strength and clarity of each paragraph in light of its actual role, and suggest targeted improvements. Then construct and evaluate an argument diagram for the paper section as a whole.

Your analysis must be **reconstruction-first**: determine as faithfully as possible what the existing text says and how its propositions appear to relate before evaluating or revising it. Separate reconstruction, evaluation, and revision into distinct stages.

Do not assume that every paragraph contains a complete argument. Classify paragraphs as:

- **Argumentative** — advances or defends a conclusion;
- **Argument-supporting** — supplies background, definitions, evidence, methods, results, or qualifications used by an argument elsewhere;
- **Mixed** — combines argumentative and nonargumentative work; or
- **Nonargumentative/functional** — primarily describes, reports, defines, sequences, or transitions without making an inferential move.

Judge each paragraph according to its actual role. Do not penalize a methods, results, or descriptive paragraph merely because it lacks a local conclusion.

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

## Argument-Diagram Conventions

### 1. Units and identifiers

1. Number paragraphs consecutively as `¶1`, `¶2`, `¶3`, and so forth.
2. Within each paragraph, number sentences as `S1`, `S2`, and so forth.
3. Extract distinct propositions and assign stable identifiers:

   ```text
   ¶1-[P1]   Explicit premise
   ¶1-[IC1]  Intermediate conclusion
   ¶1-[MC]   Main paragraph conclusion
   ¶1-[O1]   Objection or counterconsideration
   ¶1-[R1]   Response or rebuttal
   ¶1-[Q1]   Qualification or limitation
   ¶1-[IP1]  Reconstructed implicit premise
   ```

4. Preserve the wording and order of the original sentences before paraphrasing propositions.
5. Split compound sentences when they contain propositions that play different inferential roles. Do not split embedded material that does not make a separable claim.

### 2. Directed relations

Use these plain-text conventions:

```text
[reason] --supports--------> [conclusion]
[objection] --attacks------> [claim or inference]
[response] --rebuts--------> [objection]
[consideration] --undercuts--> [supporting inference]
[statement] --qualifies----> [claim]
```

The arrow must point from the proposition performing the inferential function to the proposition or inference it acts upon.

### 3. Linked and convergent support

Distinguish carefully between:

```text
LINKED SUPPORT
{[P1], [P2]} --jointly-supports--> [C]
```

and:

```text
CONVERGENT SUPPORT
[P1] --supports--> [C]
[P2] --supports--> [C]
```

Use linked support when the premises are intended to work together as a single reason and neither supplies the intended inference independently. Use convergent support when each premise contributes a distinct reason.

### 4. Implicit material

Reconstruct an implicit premise or intermediate conclusion only when it is needed to make the apparent inference intelligible. Mark it clearly as reconstructed rather than textual:

```text
¶2-[IP1] — [implicit bridging principle]
Status: Reconstructed; not explicitly stated
Basis: [why the inference appears to require it]
```

Do not silently strengthen the author's claims, add missing evidence, or replace a weak argument with a better one during reconstruction.

### 5. Attacks and responses

Distinguish:

- an attack on a **claim**;
- an attack on the **relevance, acceptability, or sufficiency of a premise**;
- an attack on the **inference** from premises to conclusion;
- a rebuttal of an objection;
- a qualification that narrows a claim without rejecting it.

If plain-text arrows cannot target an inference clearly, name the inference:

```text
I1: {[P1], [P2]} --jointly-supports--> [C1]
[O1] --undercuts--> I1
```

### 6. Graphs rather than forced trees

An argument may be a directed graph rather than a tree. A proposition may support more than one conclusion, and a response may both rebut an objection and support the main conclusion. Represent cross-connections explicitly rather than duplicating or concealing them.

---

## Analytical Procedure

Perform the following stages in order.

### Stage 1: Establish the section's apparent argumentative context

Before analyzing individual paragraphs:

1. State the section's apparent purpose in the paper.
2. Identify its apparent principal question, issue, thesis, conclusion, or informational outcome.
3. State whether the section appears primarily argumentative, explanatory, descriptive, methodological, evidentiary, interpretive, or mixed.
4. Identify important contextual uncertainty caused by the absence of other parts of the paper.

Do not evaluate or score the section yet.

### Stage 2: Analyze every paragraph

For each paragraph, provide all of the following components.

#### A. Paragraph contribution and classification

```text
¶# — [concise propositional gloss of the paragraph's contribution]
Classification: [Argumentative / Argument-supporting / Mixed /
                 Nonargumentative-functional]
Apparent role in section: [specific function]
```

The gloss must state what the paragraph contributes, not merely its topic.

#### B. Sentence segmentation

Reproduce the paragraph sentence by sentence:

```text
S1 — [original sentence]
S2 — [original sentence]
```

Preserve the original wording. Do not silently revise it during analysis.

#### C. Proposition ledger

Extract and classify the paragraph's propositions:

| ID | Proposition | Explicit or reconstructed? | Inferential role |
|---|---|---|---|
| `¶1-[P1]` | ... | Explicit | Premise |
| `¶1-[IC1]` | ... | Reconstructed | Intermediate conclusion |
| `¶1-[MC]` | ... | Explicit | Main paragraph conclusion |

Use concise propositional paraphrases while preserving the original level of certainty. Do not change “may” into “does,” an association into causation, or a limited finding into a universal claim.

If no local inference is present, state:

```text
No local argument is asserted. These propositions function as
[background / definition / method / reported result / transition / other].
```

Then identify whether and how those propositions appear to supply premises or context for an argument elsewhere in the section.

#### D. Plain-text argument diagram

Construct the paragraph's leading argument reconstruction. For example:

```text
[MC] [main paragraph conclusion]
│
├── LINKED SUPPORT
│   ├── [P1] ...
│   ├── [P2] ...
│   └── [IP1] ...
│
└── OBJECTION
    └── [O1] ...
        └── REBUTTAL
            └── [R1] ...
```

Indentation is a reading aid. The edge ledger below is authoritative when the structure contains cross-connections.

For a nonargumentative paragraph, provide a **propositional contribution map** instead:

```text
PARAGRAPH CONTRIBUTION
├── [P1] Supplies background for section claim [SC1]
├── [P2] Defines a term used in [SC1]
└── [P3] Reports a result later interpreted in ¶5
```

Do not manufacture a local conclusion merely to produce a diagram.

#### E. Edge and inference ledger

List every material inferential relation:

```text
I1  {[P1], [P2]} --jointly-supports--> [IC1]
    Intended inference: ...

I2  [IC1] --supports--> [MC]
    Intended inference: ...

A1  [O1] --attacks--> [MC]
    Target and force of attack: ...

R1  [R1] --rebuts--> [O1]
    Intended response: ...
```

Identify whether each inference is:

- explicit and signaled;
- explicit but weakly signaled;
- reconstructed with high confidence;
- reconstructed with moderate or low confidence.

When two analyses are genuinely plausible, present the leading reconstruction and briefly state the strongest alternative.

#### F. Structural and inferential diagnosis

Identify what works and what may impede the paragraph's effectiveness. Ground each diagnosis in specific proposition or inference identifiers. Consider, when applicable:

- an absent, buried, vague, or competing conclusion;
- premise–conclusion relationships that are difficult to recover;
- premises that are irrelevant to the apparent conclusion;
- premises that require an unstated bridge;
- weak, implausible, or overly broad implicit premises;
- evidence that supports a narrower claim than the text concludes;
- a jump from description or correlation to causation or recommendation;
- linked premises incorrectly presented as independent reasons;
- evidence presented without an intermediate interpretive conclusion;
- an objection without a response;
- a response that does not address the objection's actual target;
- qualifications that are omitted, misplaced, or inconsistent with the conclusion;
- one proposition doing too many jobs;
- multiple arguments compressed into one paragraph;
- redundancy, digression, or an unattached proposition;
- dependence on evidence or definitions supplied elsewhere but not clearly connected.

Do not call an inference “weak” without explaining whether the problem concerns relevance, acceptability, sufficiency, an implicit premise, or the scope of the conclusion.

#### G. Paragraph strength rating

Rate every paragraph from 1 to 5 on five role-sensitive dimensions:

| Dimension | Diagnostic question |
|---|---|
| **Contribution clarity** | Is the paragraph's conclusion or nonargumentative contribution identifiable and appropriately expressed? |
| **Propositional precision** | Are its material claims distinct, appropriately scoped, and internally consistent? |
| **Inferential organization** | Are support, attack, qualification, and dependency relations recoverable and well organized? For a nonargumentative paragraph, are its propositions clearly connected to the section's argument or informational purpose? |
| **Development and sufficiency** | Does it supply enough support, explanation, evidence, detail, or qualification for its actual role? |
| **Relevance and focus** | Do its propositions contribute without avoidable digression, competition, or redundancy? |

Use this scale consistently:

```text
5 — Strong: clear and effective; no material structural revision needed
4 — Effective: coherent, with one or two minor opportunities for improvement
3 — Adequate but uneven: understandable, with at least one substantive weakness
2 — Weak: significant difficulty recovering or accepting its intended contribution
1 — Seriously impaired: no stable contribution or coherent inferential role is recoverable
```

Report:

```text
Contribution clarity:      #/5
Propositional precision:   #/5
Inferential organization:  #/5
Development and sufficiency:#/5
Relevance and focus:       #/5
Total:                    ##/25

Overall classification:
22–25 Strong
18–21 Effective
14–17 Adequate but uneven
10–13 Weak
 5–9  Seriously impaired
```

For a paragraph with no local argument, also state:

```text
Local argument strength: Not applicable
```

Its total should measure the effectiveness of its contribution to the section, not the strength of a nonexistent local inference.

Give a concise justification for every score below 5. Scores must follow from identified propositions and relations rather than general impressions.

#### H. Targeted improvement options

Suggest the smallest changes likely to resolve the diagnosed problems. Possible operations include:

- state, narrow, or reposition the conclusion;
- separate two conclusions;
- add or make explicit a necessary bridging premise;
- add an intermediate conclusion connecting evidence to the main claim;
- supply support for a premise currently asserted without support;
- distinguish linked from convergent reasons;
- remove, relocate, or integrate an irrelevant proposition;
- align the scope and certainty of the conclusion with its premises;
- add a qualification;
- identify and answer an objection;
- revise a response so it addresses the objection's actual target;
- split an overloaded paragraph;
- combine an underdeveloped paragraph with an adjacent argument;
- improve an explicit inference marker such as “therefore,” “because,” “however,” or “although.”

For every recommendation, state:

```text
Problem addressed:
Affected node(s) or inference(s):
Recommended operation:
Expected effect on the argument diagram:
```

You may offer short example wording for a missing bridge, qualification, or transition, but do **not** rewrite the entire paragraph unless explicitly requested. Preserve the author's substantive position and disciplinary terminology.

### Stage 3: Construct and evaluate the section-level argument

After analyzing every paragraph, examine how the paragraphs work together.

#### A. Paragraph contribution ledger

List paragraphs in their original order:

```text
¶1 — Establishes ...
¶2 — Supplies evidence for ...
¶3 — Develops an alternative explanation ...
¶4 — Reports a result later used by ...
```

#### B. Section proposition ledger

Assign section-level identifiers:

```text
[SC]   Section's principal conclusion or outcome
[SIC1] Section-level intermediate conclusion
[SP1]  Section-level premise
[SO1]  Section-level objection
[SR1]  Section-level response
[SIP1] Reconstructed section-level implicit premise
```

For each section-level proposition, identify the paragraph(s) in which it is expressed or supported.

#### C. Whole-section argument diagram

Construct a plain-text directed graph. For example:

```text
[SC] [section conclusion]
│
├── ARGUMENT 1 — LINKED
│   ├── [SIC1] ...       ← developed in ¶1–¶3
│   ├── [SP2] ...        ← evidence in ¶4
│   └── [SIP1] ...       ← reconstructed bridge
│
├── ARGUMENT 2 — CONVERGENT
│   └── [SP3] ...        ← developed in ¶5
│
└── OBJECTION
    └── [SO1] ...        ← ¶6
        └── RESPONSE
            └── [SR1] ... ← ¶7
```

Then provide an authoritative edge list that records all cross-connections:

```text
{[SIC1], [SP2], [SIP1]} --jointly-supports--> [SC]
[SP3] --supports--> [SC]
[SO1] --attacks--> [SC]
[SR1] --rebuts--> [SO1]
[SP2] --also-supports--> [SIC2]
```

Preserve paragraph order in the contribution ledger, but organize the diagram by inferential dependency rather than chronology.

#### D. Section-level diagnosis

Evaluate:

- whether the section has a clear principal conclusion or informational outcome;
- whether each paragraph contributes to a proposition or inference in the section map;
- whether the order of paragraphs helps the reader reconstruct the argument;
- whether intermediate conclusions connect evidence to higher-level claims;
- whether linked and convergent reasons are appropriately organized;
- whether central premises have adequate support;
- whether important bridging assumptions remain implicit;
- whether the conclusion exceeds the scope or certainty of the premises;
- whether objections, alternative explanations, limitations, and responses are properly connected;
- whether background, methods, or results are supplied but never used inferentially;
- whether duplication, gaps, or cross-connections indicate that paragraphs should be moved, split, or combined.

Identify both strengths and weaknesses. Distinguish an actual inferential problem from an unconventional but defensible organization.

#### E. Section strength rating

Rate the section from 1 to 5 on each dimension:

| Dimension | Diagnostic question |
|---|---|
| **Central conclusion or outcome** | Is the section's principal contribution clear and appropriately scoped? |
| **Paragraph integration** | Does every paragraph have a recoverable role in the section map? |
| **Inferential architecture** | Are premises, intermediate conclusions, objections, and responses organized coherently? |
| **Relevance and support** | Do the stated reasons bear on the conclusions they are meant to support? |
| **Sufficiency and bridges** | Is the path from evidence to conclusion adequately developed without untenable hidden steps? |
| **Qualification and dialectical balance** | Are limitations, alternatives, and objections handled in proportion to the claims? |

Report the six scores and a total out of 30:

```text
26–30 Strong
21–25 Effective
16–20 Adequate but uneven
11–15 Weak
 6–10 Seriously impaired
```

Justify every score below 5 with specific nodes or inferences.

#### F. Prioritized section improvement plan

Provide a numbered list ordered by likely impact. For each recommendation, identify:

1. the affected paragraph(s), node(s), or inference(s);
2. the structural or inferential problem;
3. the recommended operation;
4. the expected improvement in the section-level argument graph.

Conclude with both:

1. a proposed **revision outline**, and
2. a proposed **revised argument skeleton**.

Use formats such as:

```text
PROPOSED REVISION OUTLINE

¶1 — [Retain; clarify conclusion] Establishes ...
¶2 — [Move before current ¶1] Supplies ...
¶3a — [Divide current ¶3] Presents evidence for ...
¶3b — [Divide current ¶3] Interprets that evidence as ...
¶4 — [Substantially revise] Addresses ...
```

```text
PROPOSED REVISED ARGUMENT SKELETON

{[P1], [P2]} --jointly-supports--> [IC1]
[P3] --supports--> [IC1]
{[IC1], [IP1]} --jointly-supports--> [SC]
[O1] --attacks--> [SC]
[R1] --rebuts--> [O1]
```

Do not rewrite the full section unless explicitly requested.

---

## Evaluation Boundaries

Maintain these distinctions throughout:

1. **Reconstruction is not endorsement.** Map the author's apparent argument before judging it.
2. **Argument structure is not factual verification.** Do not assume a premise is true because it is clearly connected.
3. **Local inferential strength is not methodological validity.** Do not conduct statistical, methodological, or source-quality appraisal unless separately requested.
4. **Rhetorical connection is not inferential support.** Background or elaboration may help comprehension without increasing the probability or acceptability of a conclusion.
5. **Do not force every paragraph into an argument.** Accurately identify nonargumentative contributions and connect them to the section only when the text warrants that connection.
6. **Do not repair during reconstruction.** Mark implicit premises, missing links, and possible improvements separately.
7. **Preserve modality and scope.** Do not convert possibility into certainty, association into causation, or a local result into a universal conclusion.
8. **Explain each weakness precisely.** Identify whether it concerns clarity, relevance, premise acceptability, sufficiency, inference strength, qualification, or organization.
9. **Prefer minimal revision.** Recommend wholesale rewriting only when local changes cannot reasonably repair the argument.
10. **Acknowledge uncertainty.** If proposition boundaries, inference direction, linked/convergent status, or objection targets are ambiguous, explain the alternatives.

---

## Required Output Order

Use exactly this overall sequence:

```text
1. SECTION CONTEXT AND APPARENT ARGUMENTATIVE PURPOSE

2. PARAGRAPH-BY-PARAGRAPH ANALYSIS
   ¶1
   - Contribution, classification, and role
   - Original sentence segmentation
   - Proposition ledger
   - Argument diagram or contribution map
   - Edge and inference ledger
   - Structural and inferential diagnosis
   - Paragraph strength rating
   - Targeted improvement options

   ¶2
   [repeat for every paragraph]

3. SECTION-LEVEL ARGUMENT ANALYSIS
   - Paragraph contribution ledger
   - Section proposition ledger
   - Whole-section argument diagram
   - Authoritative edge list
   - Strengths
   - Structural and inferential problems
   - Section strength rating

4. PRIORITIZED REVISION PLAN

5. PROPOSED REVISION OUTLINE

6. PROPOSED REVISED ARGUMENT SKELETON

7. ANALYTICAL UNCERTAINTIES AND LIMITS
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
