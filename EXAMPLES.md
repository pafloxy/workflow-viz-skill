# Static specimens

All specimens are illustrative, not reports of implemented changes or independent proof verification. They show the same grammar in different domains.

| File | What to inspect |
| --- | --- |
| `examples/code-peers.txt` | Two expanded peers; blank rows below labels; a continuous @tree wire through both aligned ports. |
| `examples/ascii.txt` | Smaller pure-ASCII view with the same module/object semantics. |
| `examples/math.txt` | A theorem with scoped hypotheses, an off-screen lemma, and a joint induction route. |
| `examples/narrative.txt` | A reader contract with how and qualification relationships distinct from reading order. |
| `examples/paired.txt` | Direct mathematical support separated from transitive proof ancestry. |

The mathematical toy uses the familiar identity for powers of commuting square matrices. It illustrates communication structure; it is not a source-backed audit of a particular manuscript. Lswap abbreviates the lemma that AB=BA implies B^k A=A B^k. Expanding Step should show where that lemma is used and keep the induction hypothesis scoped to that step. Simply drawing an arrow is not a proof.

The reviewed fixture suite covers these exact specimens. It does not replace a separate geometry checker or claim that every possible ASCII or Unicode layout is supported.
