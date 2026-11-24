# Promon's AI reversing experiments: containerized malware research, repeated protection benchmarks and red/blue hardening

Category: Algorithms and feature recovery · Other AI-assisted work
Record date: 2026-11-24
Stage: Analysis test

At 18:25:30 Beijing time on November 24, 2026, JikGuard (@JikGuardTech) cites Promon's November 23 Q4 2026 App Threat Report on hardening and AI attack costs. Its 18:25:32 source reply and the full public report by head of security research Benjamin Adolphi were read as supplementary evidence. This is a vendor's own research project, not independent security certification.

The team puts Claude Code or Codex, IDA Pro/Ghidra/gdb/Frida and the target inside a disposable isolated container, using fixed tools, skills and MCP services for mobile-security analysis, with controlled devices and emulators available. The comparison with REA explains architecture, not use of the REA engine. One public example is Coretax Android malware: packing, obfuscated resource names and a large Go binary hide network logic, and the agent helps locate command-and-control behavior and document mechanical analysis. The team says agents did over 80% of the work in many tasks while humans validated and guided. No auditable work-quantity definition, per-task logs or independent reproduction is supplied, so 80% is not accuracy or precisely measured time savings.

The same project's repeated benchmark controls tools and permissions for static, emulation, dynamic and unrestricted methods. External scripts grade results; judging code, protection revision and project identity are hidden from the agent. In a small binary containing a protected secret, five runs per version with the same target, model, prompt and unrestricted methodology reportedly show roughly an order-of-magnitude cost increase and more than an order-of-magnitude time increase after hardening, with success changing from every run to some runs. Model identity, target binaries and raw trial records are undisclosed. This does not mean a shipped app can be broken in three minutes or that protection is unbreakable. Parallel resource contention, tools, task scope, public training material and agent strategy all affect outcomes.

A red/blue loop has red agents investigate weaknesses, blue agents edit protector source, and the target protected again. Three attacker-knowledge levels cover no prior information, prior reports, and reports plus source. After a handful of rounds, some red-agent runs reportedly spend three to five hours and hundreds of dollars without succeeding, but AI often blocks just one trick or changes the target rather than the protector. This remains a prototype, not an unreviewed production-release pipeline. The author also explicitly acknowledges that a secret decrypted into device memory cannot be made absolutely inaccessible by client-side hardening.

The candidate, supplementary thread and November 23 public report were read here. No harness, sample, benchmark or patch was obtained or executed; no device was attacked or credentials read. All costs, durations and effectiveness claims are project reports. Analysis-test status, sample-size limits and required human review remain.

Sealed candidate: 0 likes, 2 views, 0 reposts, 1 reply. The report was published November 23, not newly published within this candidate window.

## Sources

- [Candidate: JikGuard cites AI attack-cost research, November 24, 2026 at 18:25:30 Beijing time](https://x.com/i/status/2125173961780830323)
- [Supplementary source reply naming Promon's Q4 report, 18:25:32](https://x.com/i/status/2125173967254442084)
- [Supplementary first-party report: Benjamin Adolphi, November 23, 2026, on the harness, benchmark and hardening experiments](https://promon.io/security-news/app-threat-report-q4-2026-using-ai-to-break-and-harden-app-protection-at-speed)

[中文](../promon-q42026-ai-mobile-protection-harness-benchmark.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/algorithms.md)
