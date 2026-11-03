# pomace and a Mac VM escape: a secondary report of AI teams studying video-codec components

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-03
Stage: Needs verification

At 16:00:47 Beijing time on November 3, 2026, qwerty__cs relays research slides reportedly released that day: an AI-agent team studies Apple video-codec components from code inside a Mac virtual machine, chains vulnerabilities across guest/host isolation and ultimately opens Calculator on the host. The post says guest video-processing requests can reach host components, so placing untrusted software in a VM does not automatically remove this class of attack surface. This records a reported demonstration, not an exploit chain confirmed by this collection.

The poster describes pomace as supplying reverse-engineering tools, controllable VMs, crash records, snapshot recovery and shared notes. Agents split into groups to find bugs, write code and run experiments; humans supply tools, redirect work and review results. The post also says an H9 encoder bug appeared in Calif's earlier iOS 27 jailbreak chain. Original-post lookup confirms the poster and attached video, but complete slides, original researcher attribution, vulnerability identifiers, OS builds, patch status and reproducible logs were not obtained. The H9 link and iOS version remain unverified, and fully unattended AI work must not be inferred.

Included as a concrete but unverified secondary security-research report. No target code was executed, escape reproduced or affected-version range tested. REA is unspecified. Even an authentic Calculator demonstration would not establish applicability to every Mac, hypervisor or current release.

November 3 candidate snapshot: 9 likes, 985 views, 0 reposts. The research slides and exploit chain were not independently verified.

## Sources

- [qwerty__cs relays pomace/AI Mac VM-escape research, November 3, 2026](https://x.com/i/status/2117527393921650976)

[中文](../pomace-ai-mac-vm-escape-secondary-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
