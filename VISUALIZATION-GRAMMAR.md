## Visual grammar across domains

| Symbol | Stable meaning | Programming | Mathematics | Narrative |
|---|---|---|---|---|
| `#Unit(@input)` | A module expanded in the current view. | A function, component, service, or responsibility whose internals are visible. Example: `#Parse(@text)`. | A definition, theorem, lemma, construction, or proof step whose structure is visible. Example: `#Theorem(@assumptions)`. | A section, claim, argument, or reader-facing unit whose role is visible. Example: `#Claim(@evidence)`. |
| `##Unit(@input)` | A relevant child whose internals remain hidden. | A called routine or dependency that has not been opened. | A supporting lemma, definition, or proof step referenced without expansion. | A supporting idea, subsection, example, or qualification referenced without expansion. |
| `###Unit(@input)` | A deeper descendant referenced without opening the intervening levels. | A low-level implementation detail. | A deeper proof dependency or imported result. | A deeper supporting point or source behind the visible argument. |
| `@name` | A stable identity for a reusable object. | Data, configuration, state, input, or result. Example: `@tree`. | A mathematical object, assumption, quantity, or conclusion. Example: `@Hamiltonian`. | A claim, evidence set, reader state, theme, or draft object. Example: `@main-claim`. |
| `@result ← #Unit(@input)` | The value on the right is produced and named on the left. This is assignment, not a spatial arrow. | A function produces a stored result. | A construction or definition produces a named object. | A reasoning or drafting unit produces a named claim, section, or explanation. |
| `A ──▶ B` | A directed relationship from source to destination. | Data flows from producer to consumer. Calls or control flow should be labeled separately. | A definition, assumption, or lemma supports a dependent statement. Label the edge, for example `<used in proof>`. | An idea explains, supports, justifies, or qualifies another unit. Label the rhetorical relation. |
| `┌─ #Composite ─┐` | A boundary containing related units under one local contract. | A subsystem, pipeline, package, or composite operation. | A theorem package, proof region, or scope containing local assumptions. | A section, argument block, or reader journey containing related ideas. |
| `<description>` | A short natural-language description of a role, relation, condition, or status. | `<validates input>` or `<preserve API>`. | `<given: AB=BA>` or `<used in proof>`. | `<why>`, `<qualifies>`, or `<reader exit>`. |
| `: Type` or `(.ext)` | The representation or type of an object, shown when it clarifies a boundary or conversion. | `@report : CheckResult`. | `@H : Hermitian operator`. | `@draft : Markdown (.md)`. |
| `[*]` | Current focus. | The component being inspected or changed. | The result or proof step under discussion. | The claim or section currently being developed. |
| `[x]` | Affected or selected for change; not automatically incorrect. | A module inside the impact cone. | A statement that must be rechecked after a changed assumption. | A passage affected by a structural or rhetorical change. |
| `[!]` | Warning or review required. | An unresolved contract, failure, or risk. | A questionable assumption, unsupported step, or conflicting source. | A claim that may overstate its evidence or confuse the reader. |
| `[?]` | Unknown or unresolved. | Missing implementation evidence or uncertain behavior. | An open hypothesis, unavailable proof, or unknown status. | Missing support, uncertain reader prerequisite, or unresolved framing. |

> `#`, `##`, and `###` describe how much is revealed **in the current view**. They are not permanent hierarchy levels. Likewise, containment, data flow, proof dependence, rhetorical support, and reading order are different relationships and should not share an unlabeled arrow.




## Reading the map

| Symbol | Programming | Mathematics | Narrative |
|---|---|---|---|
| `#Unit(@x)` | Function or component. | Theorem or proof step. | Section or claim. |
| `##Unit` | Hidden child function. | Hidden supporting lemma. | Hidden supporting idea. |
| `@name` | Data or result. | Object or assumption. | Claim or evidence. |
| `A ──▶ B` | Data flows to a consumer. | A result supports another result. | An idea supports or explains another idea. |

> `#` means visible; `##` means present but unopened; `@` names what flows between modules.