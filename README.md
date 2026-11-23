# IFRS Year-End Close Agent

[![IFRS Year-End Close Agent MCP server](https://mcprush.com/badge/ifrs-year-end-close-agent-mcp/card.svg)](https://mcprush.com/to/ifrs-year-end-close-agent-mcp?ref=badge)

Impairment (IAS 36), provisions (IAS 37), income taxes and Pillar Two (IAS 12) and events after the reporting period (IAS 10) in one agent.

> FOR DEMONSTRATION AND EDUCATIONAL PURPOSES ONLY. This output is not accounting, audit, tax or legal advice, and no liability whatsoever is assumed for its results or for any decision based on them. Paragraph references point to the IFRS Accounting Standards issued by the IASB; the standards' text is not reproduced. Results depend entirely on the facts entered and must be independently verified by a qualified professional against the current authoritative text before any use.

**Standards:** IAS 36 Impairment of Assets; IAS 37 Provisions, Contingent Liabilities and Contingent Assets; IAS 12 Income Taxes; IAS 10 Events after the Reporting Period
**Tools:** 30 calculators, checklists and lookups, plus `agent_about`
**For:** Financial controllers, group reporting and audit teams preparing year-end financial statements.

## What it does

- Test goodwill and CGUs for impairment, including corporate assets and pre-tax rates
- Recognise and measure provisions, onerous contracts, restructuring and decommissioning
- Compute current and deferred tax, DTA recoverability, the rate reconciliation and Pillar Two
- Classify adjusting and non-adjusting events and assess going concern
- Run all four disclosure checklists

Every result cites the IFRS paragraphs it relies on. The standards' text is paraphrased, never reproduced.

## Install

With the mcprush CLI (after buying the listing):

```bash
npx mcprush add <publisher>/ifrs-year-end-close-agent
```

Or point any MCP client at the bundled server (Node.js 22+, no dependencies, no network, no API keys):

```json
{ "mcpServers": { "ifrs-year-end-close-agent": { "command": "node", "args": ["<path>/ifrs-year-end-close-agent/dist/server.mjs"] } } }
```


## Try it

> Goodwill of 2m sits in a CGU with carrying amount 10m; cash flows are 1.5m a year for 5 years plus terminal value at 2% growth, post-tax rate 9%. Test for impairment and give the deferred tax effect.

## Tools

| Tool | What it does |
|---|---|
| `ias36_indicators` | Impairment indicators and annual test triggers (8-17) |
| `ias36_value_in_use` | Value in use, recoverable amount and impairment loss (18-57) |
| `ias36_cgu_allocation` | CGU impairment: goodwill first, pro rata with floors, NCI gross-up (104-108, C1-C9) |
| `ias36_reversal` | Reversal of an impairment loss with the depreciated-cost ceiling (109-125) |
| `ias36_disclosure_checklist` | Disclosure checklist (126-137) |
| `ias36_lookup` | Paragraph & topic lookup |
| `ias36_corporate_assets` | Corporate assets allocated to CGUs (100-103) |
| `ias36_pre_tax_rate` | Pre-tax discount rate from a post-tax rate (55, BCZ85) |
| `ias37_recognition` | Provision, contingent liability or contingent asset? (14-35) |
| `ias37_best_estimate` | Best estimate: expected value, most likely outcome, discounting and reimbursements (36-58) |
| `ias37_onerous_contract` | Onerous contracts: least net cost of exiting (66-69) |
| `ias37_restructuring` | Restructuring provisions: obligation and eligible costs (70-83) |
| `ias37_provision_rollforward` | Provision movement reconciliation and unwinding (59-61, 84) |
| `ias37_decommissioning_change` | Change in a decommissioning liability (IFRIC 1, cost model) |
| `ias37_disclosure_checklist` | Disclosure checklist (84-92) |
| `ias37_lookup` | Paragraph & topic lookup |
| `ias12_current_tax` | Current tax computation (12-14, 46) |
| `ias12_deferred_tax` | Deferred tax schedule (15-33, 47-68, 74) |
| `ias12_dta_recoverability` | Deferred tax asset recoverability (24-31, 34-37) |
| `ias12_outside_basis` | Investments in subsidiaries, branches, associates and joint arrangements (38-45) |
| `ias12_rate_reconciliation` | Tax expense reconciliation (81(c)) |
| `ias12_uncertain_tax` | Uncertain tax treatments (IFRIC 23) |
| `ias12_pillar_two` | Pillar Two top-up taxes (4A, 88A-88D) |
| `ias12_disclosure_checklist` | Disclosure checklist (79-88D) |
| `ias12_lookup` | Paragraph & topic lookup |
| `ias10_authorisation_date` | Date of authorisation for issue (4-7, 17-18) |
| `ias10_classify_events` | Adjusting and non-adjusting events (3, 8-13, 21-22) |
| `ias10_going_concern` | Going concern after the reporting period (14-16) |
| `ias10_disclosure_checklist` | Disclosure checklist (13, 17-22) |
| `ias10_lookup` | Paragraph & topic lookup |

## Sample output (`ias36_indicators`, built-in example)

Impairment test required (4 indicator(s), annual test: goodwill).

## Privacy and safety

- Runs locally over stdio. No network calls, no telemetry, no files written.
- Every tool is read-only, idempotent and closed-world (MCP annotations declared).
- No personal data is collected.

Demo and educational use only. No liability assumed for results. Not professional advice.
