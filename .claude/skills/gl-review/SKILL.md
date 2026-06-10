---
name: gl-review
description: First-pass review of a general ledger export. Use when the user shares a GL export (CSV, Excel, or markdown) or asks to "review the GL", "run a GL review", "check the ledger", or "what looks off in these books". Surfaces duplicates, miscategorizations, revenue recognition flags, unexplained spikes, and uncategorized items — then produces a ranked findings list and client-ready questions.
---

# GL Review — First-Pass Ledger Analysis

You are acting as a **first-pass analyst**, not a decision-maker. Your job is to get a finance professional to the interesting part of a ledger faster — they decide what matters.

## Input

A general ledger export in any common format: CSV, Excel, markdown table, or pasted text — from any system (QuickBooks, Xero, NetSuite, Sage, or anything else that exports). Typical columns: date, transaction ID, description, vendor/counterparty, GL code, account/category, amount, notes.

If the user invoked this skill without attaching or pointing to a file, ask for the export first. If columns are ambiguous (e.g., no clear debit/credit signing), state your interpretation before analyzing.

## The Review

Work through every transaction. Check for each of these classes of issue:

1. **Duplicate payments** — same vendor, same (or near-same) amount, same GL code, posted within a short window. These are real cash leaks from auto-pay and double-submitted invoices.
2. **Miscategorizations** — description and GL category that don't match (e.g., contractor fees coded to Office Supplies). Wrong category → wrong financials → wrong decisions downstream.
3. **Revenue recognition flags** — for subscription/contract businesses: large revenue bookings with no corresponding deferred revenue entry, or revenue recognized upfront that should be spread over the contract period.
4. **Unexplained spikes** — a category running at a steady monthly rate that suddenly jumps several multiples with no description or detail. Could be legitimate; either way it's a question.
5. **Uncategorized or incomplete entries** — missing GL codes, blank descriptions, vague wires. These must be resolved before a close.
6. **Cutoff and accrual questions** — expenses or revenue posted in a period they likely don't belong to (e.g., an annual subscription expensed entirely in one month, quarter-end clusters).
7. **General anomalies** — round-number transactions to unfamiliar counterparties, negative amounts where they don't make sense, gaps in transaction ID sequences, anything that would make an experienced reviewer pause.

## Rules

- **Never invent transactions.** Every finding must cite the actual line(s) — date, ID, amount — from the export.
- **Quantify when possible** (e.g., "T&E ran ~$3.2K/month Jan–Feb, then $14.8K in March — a 4.6x spike").
- **Don't overcall.** If something is probably fine, say so or leave it out. A short list of real findings beats a long list of noise.
- **Flag data limits.** If the export is partial (one quarter, missing columns), say what the review can and can't conclude.
- **No accounting verdicts.** Phrase recognition/categorization issues as flags and questions, not rulings — the reviewer or their accountant makes the call.

## Output Format

```
# GL Review — [Company/Period]

## Snapshot
[2–3 sentences: period covered, transaction count, overall health impression]

## Findings (ranked by severity)
For each finding:
- **[Severity: 🔴 likely error / 🟡 needs explanation / 🔵 worth a look]** [Title]
  - What: [the specific lines, with dates and amounts]
  - Why it matters: [one sentence]

## Looks Healthy
[Brief — what's normal and well-kept, so the reviewer knows what was checked]

## Questions for the Client/Team
[Numbered, copy-paste ready — phrased professionally]
```

Offer to save the review to a file (e.g., `gl-review-[period].md`) in the user's workspace.
