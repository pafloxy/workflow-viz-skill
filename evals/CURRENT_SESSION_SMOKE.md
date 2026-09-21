# Current-session behavioral smoke results

Date: 18 September 2026.

Scope: one explicit current-session run for each of code, mathematics, and narrative. These are not fresh-session A/B/C comparisons, not a held-out evaluation, and not evidence of cross-agent reliability. Every case not named below remains NOT_RUN in cases.json.

| Case | Domain | Observed result | Verdict |
| --- | --- | --- | --- |
| C02 | Code | Built the bounded CSV sales-summary exercise. The first fixture transport used literal backslash-n text and failed all five tests; the repaired implementation passed five acceptance tests and doctests. A checked static map preceded the implementation. | PASS_CURRENT_SESSION_SMOKE |
| C08 | Math | Gave the induction proof with the induction hypothesis local and the commutation-of-powers step explicit. Direct calculation for the supplied noncommuting matrices gave distinct (AB)^2 and A^2B^2. | PASS_CURRENT_SESSION_SMOKE |
| C13 | Narrative | Gave an explicit reader entry, mechanism, claim, and scoped reader exit in a read-order map. | PASS_CURRENT_SESSION_SMOKE |
| C14 | Narrative | Kept read order separate from the theorem-to-claim support relation and supplied corrected teaching prose. | PASS_CURRENT_SESSION_SMOKE |

The public package has no live component and no behavioral test runtime.
