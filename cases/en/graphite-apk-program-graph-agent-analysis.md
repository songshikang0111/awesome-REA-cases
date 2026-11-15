# Graphite: query APK call chains and dataflow as program graphs for agents, without source code

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-15
Stage: Related project

At 20:03:03 Beijing time on November 15, 2026, Johnson Li (@jingsenli) replies that an agent with only an APK can query call chains and dataflow across the app to trace value origins and connections. A supplementary earlier parent reply at 00:19:46 that day identifies johnsonlee/graphite, not the already cataloged Apkscope, and calls Graphite a force multiplier for REA. That parent predates this window and is used for identification, not as another candidate.

Supplementary reading inspected the README at d4dd8ee618b0345bb91de3f90c7c238b3f4425f9, committed November 14, 2026 at 13:53:37 UTC, before the window. Graphite builds program graphs from inputs including JVM bytecode, exposing calls, types and dataflow as focused context for LLM Cypher queries over MCP, with CLI and Explorer access. APK analysis needs Java and Android platform jars. The source-free JVM path does not imply arbitrary binary-only Swift/Objective-C analysis: the Apple frontend depends on compiler indexes and declarations.

The documentation explicitly limits static-graph coverage to supplied classes, dependencies and supported patterns; reflection and dynamic loading can leave relationships unresolved. README scale, latency, CodeGraph comparison and openCypher compatibility figures were not rerun here and do not prove complete recovery of every APK or correctness of every query. This records a specific agent-assisted reversing support project and APK investigation use, without a tested target APK. REA collaboration is an author suggestion, not an audited joint execution trace.

Sealed candidate: 0 likes, 10 views, 0 reposts, 0 replies; no installation or measurement of APK analysis completeness.

## Sources

- [Johnson Li on agent call-chain/dataflow investigation with only an APK, November 15, 2026 at 20:03:03 Beijing time](https://x.com/i/status/2121937017642881334)
- [Pre-window parent: Graphite name, repository and REA collaboration suggestion, November 15, 2026 at 00:19:46 Beijing time](https://x.com/i/status/2121639234293616957)
- [Pre-window pinned README: program graphs, MCP, APK requirements and static limits, commit November 14, 2026 at 13:53:37 UTC](https://github.com/johnsonlee/graphite/blob/d4dd8ee618b0345bb91de3f90c7c238b3f4425f9/README.md)

[中文](../graphite-apk-program-graph-agent-analysis.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
