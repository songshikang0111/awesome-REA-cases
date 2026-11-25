# GLM-5.4 inside Drost: the original author's private-lab black-box trust-chain account

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-25
Stage: Needs verification

At 10:50:13 Beijing time on November 25, 2026, 柠檬头.sol (@colinchen4), in AI Radar, separately describes developer Migel Tissera testing GLM-5.4 inside Drost on a multi-stage black-box chain in his own private laboratory. The application is unnamed. The concrete behavioral/trust boundaries involve an authenticated upload entry, subtitle storage, PostgreSQL, background jobs and a rendering environment. The post says injection, job poisoning and a database-to-shell trust flaw ultimately yielded non-root remote execution inside a gVisor-isolated renderer. After the author requested further escalation, the model reportedly found a path to take over arbitrary users.

These initially came from the roundup. Supplementary reading of Migel Tissera's (@migtissera) original post, dated November 24 at 00:51:26 Beijing time, confirms the same private laboratory, intended chain, non-root execution and follow-on account-takeover claim. He specifically says he had not deliberately planted another path; that is not independent validation of the absence of other prepared conditions. The original predates this window and supplies first-party attribution for the candidate, not another candidate. Drost revision, pinned model, laboratory setup, samples, complete sessions and remediation validation were not obtained; attached screenshots were not inspected. The post date is not an experiment date. Execution inside gVisor establishes neither a gVisor escape nor host root, and an arbitrary-user path does not establish control of production users. Tools and a prepared attack surface support this laboratory experiment; no general success rate against public systems follows.

Cairn/MONAI Label in the same roundup is a different target and environment, retained separately without transferring timings or success metrics. REA is unmentioned; status is unverified. Drost was not installed, no target was connected and no attack was run here. No reusable exploit payload is provided. The entry retains reported black-box behavior research and its limits.

Shared roundup snapshot with the MONAI entry: 1 like, 374 views, 0 reposts, 1 reply. Not a second independent reproduction, and no elapsed-time metric is supplied.

## Sources

- [AI Radar relays Migel Tissera's GLM-5.4/Drost private-lab test, November 25, 2026 at 10:50:13 Beijing time](https://x.com/i/status/2125421770249535608)
- [Supplement: original experiment account by Migel Tissera, November 24, 2026 at 00:51:26 Beijing time; pre-window context](https://x.com/i/status/2124908697218699315)

[中文](../glm54-drost-private-lab-blackbox-chain-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
