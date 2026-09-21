# Three self-contained trial prompts

Use a fresh session with SKILL.md explicitly available. Repeat in another session using only standing instructions to test implicit adoption. Review the transcript because a final map alone does not establish that intermediate maps appeared at the appropriate moments.

## Code: a bounded multi-module exercise

```text
Use $module-map-visuals. Work only in a new temporary directory; do not reuse or overwrite an existing demo. Use Python standard library and unittest. No network, dependency installation, or unrelated repository reads. Implement a CSV sales-summary tool with distinct parsing, validation, aggregation, and formatting responsibilities. Fields: product, quantity, unit_price. Parse prices with Decimal. Reject negative quantities/prices and malformed rows with line-specific errors. Zero values are valid. An empty input containing only the header gives an empty summary. Aggregate repeated products; order product names lexicographically. Return a typed result rather than arbitrary nested dictionaries. Add a skip-invalid mode which reports errors but retains valid rows. Strict mode must reject the batch; do not let partially accumulated results escape. Use static maps in your assistant messages before substantial work and on real boundary or decision changes. Keep the map focused, show at least the interacting boundaries, and distinguish proposed from implemented. Do not invent revisions. Test invalid rows, zero quantities, repeated products, empty input, and both modes. End with a FINAL MAP, actual test evidence, changed demo files, and limitations.
```

## Proof: preserving hypotheses during pruning

```text
Use $module-map-visuals, text only; do not touch files. Explain and prove: For square real matrices A,B with AB=BA, and integer n>=0, (AB)^n=A^n B^n. Give a compact dependency map, open the induction step, and account for any off-screen lemmas using given/imports/needs correctly. Keep the induction hypothesis local and distinguish joint premises from alternative proofs. Supply the actual argument, not just boxes. Then test whether the commutation hypothesis can be dropped, using A=[[1,1],[0,1]], B=[[1,0],[1,1]], n=2. If a calculation contradicts a broader claim, report that openly. End with a map whose evidence status matches what you actually checked. No claim of formal proof-tool verification.
```

## Writing and paired support: catch scope inflation

```text
Use $module-map-visuals. Do not edit files. Source fact supplied for this exercise: If A and B are commuting square matrices and n is a nonnegative integer, (AB)^n=A^n B^n. No result about arbitrary matrices or algorithms is supplied. Draft a short teaching explanation for a reader who knows matrix multiplication but not why reordering is dangerous. First show reader-entry/exit modules and how/why/qualification edges; show the theorem-to-narrative support separately. Keep reading order distinct from proof dependence. Explain why the draft sentence "Matrix multiplication can always be reordered, so this identity is universal" is not supported. Supply corrected prose without changing the theorem. End with a compact paired FINAL MAP and source/claim limitations.
```
