# Modular View Skill

One visual language for explaining code, mathematical arguments, and writing.

The shipped Agent Skill is [module-map-visuals](SKILL.md). It gives an agent stable module IDs, recursive disclosure, typed objects, directed relations, and scoped hidden context. Maps appear in ordinary terminal or chat messages.

## Agent handoff

For a direct agentic handoff, point the agent to [AGENT_HANDOFF.md](AGENT_HANDOFF.md) first. It states the public scope, required reading order, task branches, and completion criteria.

## Use

Give an agent [SKILL.md](SKILL.md) together with a task, or invoke it explicitly with: `Use $module-map-visuals for this task.`

For default-on communication, merge [integrations/AGENTS.md.snippet](integrations/AGENTS.md.snippet) into the applicable agent instructions. The snippet controls presentation only; it does not grant file access or mutation permission.

## Everyday prompts

- Explain this code and show the relevant callers.
- Map this proof, including hidden assumptions.
- Plan this subsection and show which results support each narrative unit.
- Expand #Parser, show the context of #T1, or use ASCII only at 80 columns.

Configuration is declarative: specify `charset=ascii|unicode`, `width=80`, `expanded_layers=2`, or `detail=compact|normal` in the request. These are prompt conventions, not command-line flags.

See [EXAMPLES.md](EXAMPLES.md) for explanatory notes, [examples/](examples/) for static specimens, [DEMOS.md](DEMOS.md) for self-contained tasks, and [evals/](evals/) for behavioral evaluation records.

## Product boundary

This is a static text skill. It has no worker, viewer, window, pane, hook, event stream, animation, server, browser integration, background process, or runtime dependency.

## Installation and publication

Place the skill folder in a supported user- or project-scoped Agent Skills location after checking that an existing same-name skill will not be overwritten. A folder containing only [SKILL.md](SKILL.md) is sufficient.

After publication, an optional discovery route is:

```sh
npx skills add pafloxy/modular-view-skill --skill module-map-visuals --agent codex
```

This optional installer is not a runtime dependency. Copying the skill folder remains sufficient.

## Evidence and limits

The package fixture suite validates the skill’s structure and static specimens. Behavioral evidence is partial and recorded in [evals/CURRENT_SESSION_SMOKE.md](evals/CURRENT_SESSION_SMOKE.md); remaining cases retain their stated status in [evals/cases.json](evals/cases.json). A geometry check cannot establish that a depicted dependency is true.

## Sources

- [Agent Skills format](https://agentskills.io/specification)
- [Codex skills](https://developers.openai.com/codex/skills/)
- [Codex instructions](https://developers.openai.com/codex/guides/agents-md/)
- [Optional distribution CLI](https://github.com/vercel-labs/skills)

## License

MIT © 2026 Rajarsi Pal. See [LICENSE](LICENSE).
