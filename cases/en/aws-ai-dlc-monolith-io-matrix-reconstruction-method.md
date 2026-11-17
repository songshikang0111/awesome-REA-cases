# AWS AI-DLC: reconstruct specifications from monolith shared state and check data flow through fault injection

Category: Applications and clients · Other AI-assisted work
Record date: 2026-11-17
Stage: Related project

At 14:14:06 Beijing time on November 17, 2026, the Korean AWS user group (@awskrug) shares an AI-DLC Reverse Engineering article. Supplementary reading obtained the complete Korean AWS technical blog by Eunhye Jo, dated the same day without a publication time. This is the method source linked by the candidate, not an additional candidate. AI-DLC means AI-Driven Development Life Cycle. The article addresses legacy monoliths whose global variables and shared memory hide inputs and outputs from function signatures, avoiding lost discount rates or pre-coupon amounts passed into payment when migrating to stage-specific data transfer objects (DTOs).

The example is new_order, a fictional ten-stage shopping-order C program written for the article, not a customer's production system. A tree-sitter AST and macro preprocessing extract reads/writes into an I/O matrix with R/W/RW/WR and conditional markers. Reaching definitions trace producers to consumers; CI prebuilds a code graph that agents query through read-only, predefined MCP tools. An io-matrix plugin for AI-DLC 2.11.3 links this to requirements, service boundaries, API contracts and tests. Kiro and Claude Code are workflow-compatible tool examples, not evidence both took part in the same run. A deterministic generator, rather than an LLM, produces API contracts and some code. AI writes requirements, designs and service implementations; humans decide stage configuration, terminology, unresolved accesses, effective-value rules, boundaries and approvals.

The article reports that the normal To-Be implementation passes generated tests. Injecting a pre-coupon payment amount breaks flow-delivery, conditional-value and golden-master tests. Only one coupon order among eight golden-master inputs exposes the difference, with PAYMENT.h_amount at 23691 in the legacy program versus 24691 in To-Be. Removing the hidden customer discount-rate input then breaks field-completeness, required-input, database-side-effect and other tests; five of eight golden-master cases differ. The illustrated response amounts are 23691 versus 24990 and points 236 versus 0. These are fault injections and execution outputs shown by the article, not runs performed here, a general detection rate or a customer migration outcome.

The article explicitly warns that deriving contracts and tests from one graph risks shared omissions. Human-authored expected tables and SQL/external-call execution records separately check the analyzer, but those records do not cover every variable read/write. Arrays do not distinguish indices; execution order depends on configuration; dynamic keys, indirect pointers and unanalyzed external modules need human interpretation or expanded analysis. Structural tests cannot replace computational golden masters, which depend on human-selected inputs. The complete article and code excerpts were read, not a complete reproducible repository or raw execution logs. No parser, target, AI session or AWS resources were run here. REA is unmentioned; status remains related-project for a method demonstration.

Sealed candidate: 0 likes, 50 views, 0 reposts, 0 replies. The supplementary full article has an original date and byline; article reports are not independent reproduction.
Ten stages, AI-DLC 2.11.3, eight cases and the one/five differing cases come from the author's example, not a customer's scale, detection rate or measured effort.

## Sources

- [Korean AWS user group shares the method, November 17, 2026 at 14:14:06 Beijing time](https://x.com/i/status/2122573978200134027)
- [Supplementary full article: Eunhye Jo's AWS technical blog, November 17, 2026, fictional order program and fault injection](https://aws.amazon.com/ko/blogs/tech/aws-ai-dlc-reverse-engineering-io-matrix-for-spec-and-verification/)

[中文](../aws-ai-dlc-monolith-io-matrix-reconstruction-method.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
