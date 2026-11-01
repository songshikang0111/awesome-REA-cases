# SRE-Bench: from alliance announcement to execution scoring — generating a correct candidate is not selecting it

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-02
Stage: Related project

At 04:33:42 Beijing time on October 27, 2026, Artificial Analysis (@ArtificialAnlys) announces Pasta Lab joining the Cyber Index Alliance, describing members from Columbia, Tufts and UCLA and SRE-Bench for evaluating AI reversing. The official post's attribution was previously checked. Collaboration alongside CollinearAI, IBM, NVIDIA and Vercel establishes neither independent reproduction by those organizations nor inclusion as a scored Cyber Index component.

A new candidate at 03:28:06 Beijing time on November 2 explains SRE-Bench's distinction between generating and selecting a correct solution. This review additionally read the abstract, evaluation configuration and relevant C.1 passages of arXiv:2608.11469v2. The first submission is August 11 and the read version October 1, both before the candidate: supplementary primary evidence, not a new result from this window. The paper describes experts creating 19 private programs from scratch averaging 16.9K lines, with compilation variations and 44 in-house anti-analysis mechanisms producing 262 binaries, six tasks each and 1,572 tasks overall, not 262 independent software projects. Agents receive binaries, domain material and tools, submitting programs/actions to an unseen deterministic execution grader rather than being scored for plausible prose.

The candidate and paper report provider-internal Codex runs of GPT-6-Astra Max with public cyber safeguards disabled and no evaluation budget cap: four attempts on each of the same 262 instances, with all six tasks solved in 922/1,048 attempts, about 88.0% pass@1, and at least one full solve on 260/262 instances, about 99.2% pass@4. All four attempts succeed on 191 instances; 69 mix success/failure; two always fail. These are different units from the same trials, not before/after training gains or attack success rates. High pass@4 relies on the private grader identifying a correct answer afterward; this evaluation does not test choosing an answer without that grader. A simulated malware-cleanup task also requires retaining ordinary user data and removing restart mechanisms; deleting everything cannot earn credit.

The separate public configuration uses mini-SWE-agent with 500 steps and six hours, excluding runs ungradable because of refusal or context overflow from the corresponding statistics. It cannot be compared directly with uncapped internal scores as an improvement. New evidence fills the original announcement's missing sample/scoring details, but private binaries, reference answers and the grader were not run here, nor was the original repository read or the benchmark independently reproduced. Scale/contamination control are paper design claims, not demonstrated coverage of large real products. The original ID and related-project status remain. REA is not mentioned.

Original announcement snapshot: 37 likes, 7,356 views, 2 reposts. New candidate: 2 likes, 32 views, 0 reposts, not newly executed model scores.
Arithmetic checked here: 922/1,048 is about 87.98%; 260/262 about 99.24%, rounded in the paper to 88.0% and 99.2%. No evaluation was run here.
Paper v2 is dated October 1, 2026, before the November 2 candidate. Only relevant public passages were additionally read; the private benchmark was not independently reproduced.

## Sources

- [Artificial Analysis official Pasta Lab/SRE-Bench alliance announcement, October 27, 2026 Beijing time](https://x.com/i/status/2114817771188175007)
- [New candidate: four-attempt SRE-Bench results and the untested solution-selector limitation, November 2, 2026](https://x.com/i/status/2116975588741423314)
- [Supplementary primary paper v2: design, internal configuration and selection limits, October 1, 2026](https://arxiv.org/html/2608.11469v2)

[中文](../pasta-lab-sre-bench-cyber-index-alliance.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
