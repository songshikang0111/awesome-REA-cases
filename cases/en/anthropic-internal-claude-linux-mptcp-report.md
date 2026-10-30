# Linux MPTCP: internal Claude kernel-race research, now cross-checked against CVE and Go advisories

Category: Applications and clients · Other AI-assisted work
Record date: 2026-10-30
Stage: Analysis test

At 09:33:04 Beijing time on October 29, 2026, Ummon's five-target report relays Anthropic's Linux networking investigation. The demonstrated target is a kernel path exposed through a multipath-TCP listener. The account outlines a race-induced use-after-free, kernel-address disclosure and callback control-flow influence, claiming root command execution without credentials or user interaction. Only the research shape is recorded, without triggering packets, exploit code or instructions.

Earlier supplementary reading of the October 27 official article confirms a project-reported demonstration of about 48 minutes to obtain an address and five more to reach command execution, with a lost race failing the handshake rather than crashing the system. It labels the issue CVE-2026-98432 and says upstream and maintained stable branches were patched. These are not universal timings or evidence that all Linux systems are reachable. The internal model is unnamed and begins with human prompting; coordinated disclosure and no reported in-the-wild exploitation do not prove an absence of attackers.

In the new candidate at 11:31:02 on October 30, SANS.edu Internet Storm Center (@sans_isc) reports Claude's Linux-kernel MPTCP RCE under the same CVE. This supplements the same target rather than inventing a new flaw from a podcast title. The CVE Program record was checked: first published October 15, with the current record updated at 02:08:12Z on October 30. These are earlier disclosure and same-day documentary supplementation, not a first discovery in this window. The Linux CNA title concerns freeing inet_opt/ireq_opt after an RCU grace period and records a use-after-free in IPv4 TCP option lifetimes with patch references. The underlying bug is not MPTCP-only.

The oss-security forward at 08:21:41 Beijing time on October 30 reproduces a Go Security Team message originally sent at 07:34:28 that day, both before this candidate. It cites Anthropic's demonstration, explicitly distinguishing a demonstrated RCE requiring an MPTCP listener from possible similar attacks without one. Linux listening sockets enable MPTCP by default from Go 1.24, with per-socket settings able to override defaults. The team says upgrading to a patched kernel is the best fix; per-program MPTCP disabling is a fragile mitigation, not a complete repair. No attack method or exposure judgment about a reader's machine is supplied here.

This update checks the existence and scope of the CVE/advisory, correcting the earlier unchecked-advisory limitation. It does not validate every stable-branch build, rerun the exploit or count actually affected hosts. Documentary confirmation is not independent reproduction. Analysis-test status remains and REA is unspecified. This collection only read public text and sent no packets to targets.

Earlier shared candidate snapshot: 0 likes, 157 views, 0 reposts. The 48-minute/five-minute timings are project demonstration figures.
CVE and Go advisories were statically checked, not each branch's build, exploit or real exposure independently validated.
SANS candidate snapshot: 1 like, 446 views, 1 repost. The CVE documentation and original message predate the candidate and add no candidates.

## Sources

- [The Linux MPTCP investigation in Ummon's full report, October 29, 2026](https://x.com/i/status/2115617884533907835)
- [Supplementary original research: Anthropic's October 27 Linux section](https://www.anthropic.com/research/discovering-vulnerabilities-with-claude#5-zero-click-remote-code-execution-in-linux)
- [SANS Stormcast reports Claude/Linux research under the same CVE, October 30, 2026](https://x.com/i/status/2116009959230234650)
- [Supplementary CVE Program record: IPv4 TCP flaw and patch references, first published October 15](https://cveawg.mitre.org/api/cve/CVE-2026-98432)
- [Earlier supplementary evidence: oss-security forward of the Go Security Team's MPTCP scope and upgrade advice](https://www.openwall.com/lists/oss-security/2026/10/30/1)

[中文](../anthropic-internal-claude-linux-mptcp-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
