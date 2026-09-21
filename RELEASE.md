# Release preparation

## Status

This repository is the release candidate for [pafloxy/modular-view-skill](https://github.com/pafloxy/modular-view-skill). Its product name is Modular View Skill, and its shipped Agent Skill is module-map-visuals.

## Permanent product boundary

**This repository has no live components and will not add them.** It has no worker, viewer, window, pane, hook, event stream, animation, server, browser integration, background process, or runtime dependency. SKILL.md is text instructions for an agent.

## Evidence

The reviewed fixture suite passed 46 tests. Behavioral evidence is partial: C02, C08, C13, and C14 passed current-session smoke trials recorded in evals/CURRENT_SESSION_SMOKE.md. The remaining cases are NOT_RUN, so the record does not establish fresh-session or cross-agent reliability.

## License

Copyright © 2026 Rajarsi Pal. This repository is MIT licensed; see LICENSE.

## Publication sequence

1. Review README.md.
2. Verify the checked public payload and evaluation records.
3. Commit this repository and push the main branch to pafloxy/modular-view-skill.
4. Create the first versioned GitHub release when the behavioral evidence supports the intended claim.
