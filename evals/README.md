# Behavioral evaluation protocol

These 24 cases are specifications, not passing LLM evaluations.

Run the same code, mathematics, and writing tasks in fresh sessions with no visual skill, with a comparable installed static skill, and with this candidate. Keep inputs, tool permissions, model/version/effort, and task constraints fixed. Repeat at least three times per profile for an initial cross-domain trial; report variation rather than treating one attractive output as reliability evidence. Run negative and near-miss cases separately. Record cases not run as NOT_RUN.

Review output for correct scope and trigger, source fidelity, edge semantics, hidden-context retention, stable IDs, readable geometry, timing of in-chat maps, actual task completion, honest verification, and absence of dynamic process or tool setup. A severe semantic misrepresentation or unauthorized action is a failure regardless of visual quality. Do not give a passing average to a missing assumption.

Compare SKILL.md-only against any optional expanded reference or checker route to measure whether more context improves useful behavior. Try removing one paragraph at a time; retain shorter wording only if the relevant cases still pass. This is a compression experiment, not a guarantee that the candidate is optimal. Record skill bytes/words, total tokens when available, elapsed time, number of updates, and human legibility judgments. Never invent token or time measurements.

Prefer private transcripts for review. Publish sanitized fixtures and aggregate results, not real manuscripts, repository secrets, or personal logs. Use independently held-out cases before advertising cross-agent reliability.
