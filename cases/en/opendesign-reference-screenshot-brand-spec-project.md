# OpenDesign: extracting brand rules from reference screenshots for coding-agent interface reconstruction

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-15
Stage: Related project

At 09:46:09 Beijing time on November 15, 2026, AIWare (@aiwaremax) introduces nexu-io's OpenDesign. The problem is inconsistent type, corner radii and colors when coding agents separately generate landing pages, dashboards, slides and videos. The specific feature relevant here studies visual rules from reference screenshots of existing brands and turns them into reusable specifications. It is not decompiling Claude Design or recovering its source.

Supplementary research read the public README pinned at 59e4f2ae85de7e7318a5e6bdcf3a34584c4b7582, committed November 13, 2026 at 09:15:18 UTC, before this window. It supports methodology only. The documented workflow accepts a screenshot or URL, has an agent codify a reusable DESIGN.md, combines the specification with plugins and templates to generate HTML/CSS artifacts, and hands them to Claude Code, Codex or Cursor for further development. A stdio MCP server can read current project files such as tokens CSS, JSX and HTML. This supports the project's brand-rule extraction and reconstruction purpose, not exact recovery of a design system, interactions or backend from any screenshot.

The candidate lists 151 brand systems, 277 official plugins, 183 reference examples and 26 agent CLIs. The read README also gives these catalog sizes, but explains that legacy design packages may contain only DESIGN.md, while newer packages can add a manifest, tokens.css, components, assets and provenance. Not every package can be described as a complete token implementation. Directories were not enumerated and all adapters were not tested. The claimed 107,102 GitHub stars are the candidate's promotional snapshot, not independently verified.

The README states Apache-2.0 licensing; third-party assets and brand rights require separate checks. Local-first does not mean offline or no outbound data: documentation explicitly sends cloud-model/OpenDesign Cloud requests to their respective services, keeps safety and reliability telemetry always on, and consent-gates product analytics and session replay. This collection installed no tools, connected no MCP server, uploaded no screenshots, ran no extraction and compared no output. Included as a concrete supporting project for AI-assisted visual-rule study. REA is unmentioned, and accuracy and usability remain unverified here.

Sealed candidate: 4 likes, 475 views, 0 reposts, 13 replies. 107,102 stars is the post's claimed snapshot.
151 systems, 277 plugins, 183 examples and 26 CLIs are project/commentator catalog figures, not accuracy, complete coverage or time savings measured by this collection.

## Sources

- [AIWare introduces OpenDesign screenshot-based brand extraction and coding-agent workflow, November 15, 2026 at 09:46:09 Beijing time](https://x.com/i/status/2121781771750854878)
- [Pre-window pinned README: screenshot/URL to DESIGN.md, package structure and outbound-data caveats, committed November 13, 2026 at 09:15:18 UTC](https://github.com/nexu-io/open-design/blob/59e4f2ae85de7e7318a5e6bdcf3a34584c4b7582/README.md)

[中文](../opendesign-reference-screenshot-brand-spec-project.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
