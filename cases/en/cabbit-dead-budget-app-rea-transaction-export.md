# Rescuing a discontinued budgeting app: cabbit reports REA/Claude export of 11 years and a timezone-date fix

Category: Applications and clients · REA
Record date: 2026-11-02
Stage: Needs verification

At 03:45:25 Beijing time on November 2, 2026, cabbit (@cabbitar) says an unnamed budgeting app shut down its sync server in 2023. It still opens locally but has no export/API, a 404 support page and 11 years of history in a 640MB file. They report giving Claude Code a copy with a rule never to alter the original. Reader agents use REA to locate the transaction loader, identify SQLite encrypted amount blobs with a key derived from their own app password, and write a 24-field specification tracing each field to its writer.

The first 500 exports reportedly contain 37 wrong dates, attributed to local-time storage and a 2019 move between countries, fixed in one line. The full export reportedly yields 18,406 CSV transactions and 1,212 receipt photos with categories and notes retained. Checkers compare 300 random transactions in the original app with no mismatches. Split transactions and scanned PDFs remain raw and marked for manual checking; the original allegedly changed by zero bytes.

Original-post lookup confirmed attribution and full text but supplied no app name/version, code, detailed format, key mechanism, tool output or spot-check logs. Every step uses a [00:00] placeholder, not evidence of actual duration or measured timing. Retained as a concrete data-migration report, not complete recovery, password cracking or an audited read-only guarantee. A 300-item spot check does not establish correctness of everything else. No private finances were read, exporter run or credentials accessed.

Candidate snapshot: 8 likes, 75 views, 0 reposts. Eleven years, 640MB, 24 fields, 18,406 transactions and 300 zero-mismatch checks are author claims.
The app is unnamed. [00:00] is a placeholder, not timing; split transactions and PDFs still need manual review.

## Sources

- [cabbit's discontinued-budget-app migration and date-debugging report, November 2, 2026](https://x.com/i/status/2116979948280070166)

[中文](../cabbit-dead-budget-app-rea-transaction-export.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/apps.md)
