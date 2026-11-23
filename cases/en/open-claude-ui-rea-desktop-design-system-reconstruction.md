# Open Claude UI: investigate Claude Desktop's design system with REA, then build reusable components

Category: Applications and clients · REA
Record date: 2026-11-23
Stage: In progress

At 17:07 Beijing time on November 23, 2026, a candidate introduces Caho1/open-claude-ui, translating research on Claude Desktop's interface into TypeScript/React components and design tokens for independent desktop-agent hosts. The public README was read at repository commit beb521e940db340a5f36a8bf6f34d21528adc37a, dated 2026-11-20T09:59:22Z, as supplementary material predating the window. It credits REA static extraction and read-only Main Process Debugger/9229 Node inspector observation as two evidence paths. Its current baseline is @ant/desktop 5.11492.5 and Electron 45.2.1.

The project lists 30 baseline modules, five later modules and two theme/configuration files, totaling 37 code files, plus an early manual of over 4,600 lines. Recorded details include clay #d97757, four surface layers, four spring configurations, a 4 px movement dead zone and CJK input-composition guards. Versioned documentation says some old parameters were superseded; early values are not constants across all versions. The repository says it avoids distributing proprietary fonts and recordings, using system fonts and synthesized audio instead. That is project policy, not a copyright audit performed here. The full manuals, original app and rendered comparisons were not checked, and no dependencies were installed. Rebuilding UI does not supply Claude models or backend capabilities. The candidate's assertion of saving two designer-weeks lacks measurements and is not adopted; 1,784 stars are also only a post snapshot.

Candidate: 0 likes, 39 views, 0 reposts, 0 replies. The reported 1,784 stars and 327 forks are snapshots, not proof of quality or parity.

## Sources

- [Candidate introduction to Claude Desktop UI components, November 23, 2026 at 17:07 Beijing time](https://x.com/i/status/2124791815178215634)
- [Supplementary public README pinned to a 2026-11-20T09:59:22Z commit](https://github.com/Caho1/open-claude-ui/blob/beb521e940db340a5f36a8bf6f34d21528adc37a/README.md)

[中文](../open-claude-ui-rea-desktop-design-system-reconstruction.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
