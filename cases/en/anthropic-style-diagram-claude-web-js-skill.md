# Anthropic-style diagrams: Erduo studies Claude's drawing-time JavaScript to rebuild a reusable Skill

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-05
Stage: In progress

At 14:47:36 Beijing time on November 5, 2026, Erduo (@RookieRicardoR) recalls studying web-based Claude design: request a diagram, observe additional JavaScript loaded for SVG drawing, then ask Claude what it loads to locate rules, components and size constraints. The result is the anthropic-style-diagram Skill. The goal is reusable local technical diagrams in Claude's visual language, not training a model or breaking into an account.

Supplementary review reads README and SKILL.md at public erduo-skills commit 1fb6ec5df76c01dc43fb71631b8ae6121b9251df, dated July 26 at 00:44:44 Beijing time, before this window and used only as artifact documentation. Agents author geometry and semantic classes; render.mjs injects palette, theme and typography, checks text overflow, node overlap and connectors crossing unrelated nodes, crops output, and exports PNG and standalone SVG with light/dark themes. The docs require Playwright and insist on reviewing arrows, feedback loops, labels and categorical colors after geometric checks. Passing layout checks explicitly does not establish semantic correctness.

This confirms public workflow documentation, not identity with an official internal Skill, leaked verbatim prompts or accurate diagrams in every case. Original JavaScript-observation logs, official comparisons and runtime tests are absent. README claims MIT; no complete license audit was performed. Dependencies and rendering were not installed or executed here. REA is not mentioned.

Sealed candidate: 6 likes, 480 views, 0 reposts. Retrieval confirms authorship without substituting higher live counts.

## Sources

- [Candidate and authorship lookup: Erduo recalls Claude web JS/SVG research, November 5, 2026 at 14:47:36](https://x.com/i/status/2118233755966218710)
- [Supplementary project README pinned to a July 26 commit, not this window's result date](https://github.com/rookie-ricardo/erduo-skills/blob/1fb6ec5df76c01dc43fb71631b8ae6121b9251df/README.md)
- [Supplementary Skill at the same commit: drawing contract, geometry audit and semantic review](https://github.com/rookie-ricardo/erduo-skills/blob/1fb6ec5df76c01dc43fb71631b8ae6121b9251df/skills/anthropic-style-diagram/SKILL.md)

[中文](../anthropic-style-diagram-claude-web-js-skill.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
