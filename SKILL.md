---
name: module-map-visuals
description: "Explain code, proofs, and writing through static terminal module maps. Use for modular work, dependencies, focused changes, and decisions; not greetings, exact-output requests, or unrelated questions."
---

# Module Map Visuals

Use one recursive visual language as the primary explanation of substantive work. Print maps in ordinary assistant messages, not only tool stdout or files. This file is sufficient: no renderer, script, network, pane, animation, worker, or hook is required. Show public conclusions, evidence, decisions, and uncertainty, never private deliberation.

## Routine

1. Read the relevant sources; identify the question, scope, and missing evidence. Separate source statements from inferred relationships and proposed repairs. This skill changes communication, not permissions or the requested task.
2. Show the smallest useful map before substantial work, then revise only for material changes in scope, understanding, dependencies, contracts, or evidence. Keep IDs stable. Use `Map M0`, `Map M1`, and `FINAL MAP`; distinguish current, proposed, and actual states. Do not manufacture revisions or alternatives. An atomic task needs only a final micro-map.
3. Open the active branch with its parent context and boundary neighbors. Expand multiple peers when their interaction matters. Show responsibility, relevant inputs/outputs or hypotheses/conclusion or reader entry/exit, and the invariant being preserved. A conceptual module need not be a file, function, heading, or paragraph.
4. For a real structural change, show focused before/target/actual views and a concise decision with evidence. Finish with the current map, checks and limitations, and files changed when applicable. `FINAL` can be partial, blocked, or proposed; it never implies verified.

## Grammar

```text
#Unit(@object)                  expanded in this view
##Unit(@object)                 visible, unopened
###Unit(@object)                reference to a deeper hidden descendant
@result <- #Unit(@object)       named binding; Unicode arrow also allowed
@source : Text (.md)            type/format at an external or changing boundary
<description>                  kind, relation, method, or scoped context
[*] focus   [x] affected        [!] attention   [?] uncertainty
```

Hashes describe disclosure, not permanent depth, mathematical rank, or identity. Preserve source IDs and labels; do not globally rewrite existing `@` references. Use `@` for reusable objects; omit repetitive types inside the map. Repeat attention marks at most three times; never overload them as success/failure/proof status.

`/module-expand #ID` opens the unit; `/module-context #ID` shows hidden context. Treat these as conversational requests, not installed shell or native slash commands. Natural-language requests work too. Opening changes disclosure, not the underlying claim. Mark repeated occurrences of a shared unit without creating new identities.

## Layout

Default: Unicode square borders, at most 100 columns, roughly 5–9 visible units, and two expanded layers. These are adjustable budgets, not demands to invent units. Use spaces, fixed columns, solid rails, aligned corners/ports, destination arrowheads, and a blank interior row immediately below every nested label. Narrow or uncertain-width terminals use ASCII and shorter labels; never truncate away hypotheses or distinctions.

Prefer a continuous producer-to-consumer wire through aligned borders. Put labels beside an unbroken shaft. Avoid crossings; never imply a junction between unrelated edges. Use a named-value handoff with an explicit reason only when direct routing would be ambiguous or congested. A tree alone does not show dataflow or proof dependence. Preserve readable whitespace; omit decorative boxes before omitting meaningful edges.

Illustrative peer expansion (apply the same geometry to other domains):

```text
┌─ #Pipeline(@text) <code> ────────────────────────────────────────────────────────────────────┐
│                                                                                              │
│                                                                                              │
│  ┌─ #Parse(@text) ────────────────┐                  ┌─ #Check(@tree) [*] ───────────────┐   │
│  │                                │                  │                                   │   │
│  │  @tokens <- ##Lex(@text)       │                  │                                   │   │
│  │  @tree <- ##Tree(@tokens)      │                  │                                   │   │
│  │     │                          │   @tree          │                                   │   │
│  │     └──────────────────────────┼──────────────────┼─────▶ ##Validate(@tree)           │   │
│  │                                │                  │                                   │   │
│  │                                │                  │  @report : CheckResult            │   │
│  │                                │                  │                                   │   │
│  └────────────────────────────────┘                  └───────────────────────────────────┘   │
│                                                                                              │
│  <preserve: parser emits structure; checker owns validation>                                 │
│  <basis: illustrative proposed architecture; no test verdict>                                │
│                                                                                              │
└──────────────────────────────────────────────────────────────────────────────────────────────┘
```

## Meaning: one grammar, three domains

| Domain | A module represents | Default directed relationship |
|---|---|---|
| Code | Responsibility/computation | Producer to consumer; label calls or control separately |
| Math | Definition, assumption, theorem, lemma, or precise claim | Prerequisite to dependent statement, e.g. `<used in proof>` |
| Narrative | Contribution to reader understanding | Explanatory/supporting unit to its target: `<how>`, `<why>`, `<justifies>`, `<qualifies>` |

Containment, semantic dependencies, and reading order are separate. Declare the relation once in a single-relation view; label edges individually in mixed views. Math-to-narrative `<supports>` is neither dataflow nor proof by itself. Record direct support; do not promote hidden transitive paths into direct evidence.

In math, preserve domains, quantifiers, hypotheses, and proof status. Definitions may be leaves or expose constituent objects. Expand proofs into meaningful subclaims, not commands disguised as theorems. Distinguish jointly required premises from alternative proof routes. Keep discharged assumptions local. Objects are reusable, not consumed by theorem application. Put long formulas outside the fence with an exact reference/alias inside; never weaken mathematics to fit a box.

In narrative, show role and intended reader entry/exit, not an invented measurement of comprehension. Keep reading order explicit and separate from justification. Previews/reminders are occurrences, not reverse dependencies. A polished claim cannot become stronger than its supporting mathematics. Preserve the requested prose, code, or proof deliverable: the map explains it rather than replacing it.

## Hidden context and evidence

Use `<given: ...>` for scoped hypotheses, `<imports: ID; role; status>` for off-screen dependencies/support, and `<needs: ...>` for reader prerequisites. Cover every material incoming relation omitted by pruning. A named context is acceptable only with an inspectable complete list. `###` is not an external-import marker. Hidden does not mean proved, assumed, or understood.

Check semantic direction and source support separately from visual alignment. Distinguish observed, inferred, proposed, open, and stale claims as needed. Source inconsistencies get `[!]`, not silent correction. Tests, numerical experiments, informal arguments, and formal certificates support different claims. An unedited neighbor is not automatically unaffected. After a material change, recheck affected consumers; `[x]` means review needed, not false.

## Output discipline

Lead substantive explanations with the map; allow a short outcome/orientation sentence. Keep prose subordinate but include essential caveats and accessible relationship summaries. Honor explicit brevity, plain-prose, accessibility, or exact-output constraints. No diagrams for greetings. No separate windows, animations, live logs, HTML/Mermaid exports, or runtime setup.

Before sending, check borders, spacer rows, continuous wires, destinations, labels, assumptions, and evidence. An existing compatible checker can help when available and authorized; do not install one merely to speak. Passing geometry is not semantic verification. If complex layout fails, simplify the view without changing its meaning. Configurable presentation does not redefine edge semantics or evidence standards.
