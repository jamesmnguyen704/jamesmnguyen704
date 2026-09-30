# James Nguyen

Finance and operations analyst in St. Louis. I spent ten years reconciling numbers by hand in SAP, Oracle and QuickBooks. Now I write the Python that does it.

At Day & Night Solar, a commercial solar installer with 170+ projects in 15 states, I run the accounting side (AP/AR, bank recs, payroll, multi-state sales tax, period close) and build the internal tools the team works from.

## What I've built at Day & Night

It's one private system, so the code isn't public. This is how it fits together:

<p align="center"><img src="assets/system-flow.svg" alt="Exports flow through parsers into a warehouse, then matching, staged imports and human approval" width="820"></p>

- **Bank reconciliation.** Fuzzy matching across five bank accounts with confidence tiers. Anything ambiguous goes to a review queue instead of being auto-matched, and my decisions carry over between runs.
- **QuickBooks imports.** Generates IIF files for customers, POs, invoices and deposits, checked against the full transaction history so nothing posts twice. I import them; the tool never does.
- **Reporting.** P&L, cash flow, billing and margin workbooks rebuild themselves from a local warehouse: 100+ tables, 150+ scheduled steps, 1,300+ tests.
- **Document intake.** OCR and classification for vendor documents and bank statements.
- **AI assistants.** A handful of Claude Code agents, each limited to one area (bank, books, tax, documents). None of them can import, send or publish anything until I approve it.

The rules the assistants work under:

- **Unknown is a state.** Unmatched, stale or missing data stays visible instead of turning into a convenient guess.
- **Humans approve.** Accounting imports, email, tax filings and publishing are staged and handed to a person.
- **Every number has a source.** Answers name the table or file they came from and how old it is.
- **Measure the automation.** Checks read the real output, not the intent. A green run is where the question starts.

<details>
<summary>How the assistants are split up</summary>
<br>
<p align="center"><img src="assets/agent-lanes.svg" alt="Separate assistant lanes for bank, books, projects, tax and documents, all passing through one human approval gate" width="820"></p>
</details>

## Before this

I ran my own service business for 13 years, books and payroll included, then moved into corporate accounting: AP at Walmart eCommerce, reconciliations at NTT and Robert Half, staff accountant at Curtiss-Wright, and an ERP migration (Sage CRE 300 to CMiC) at Keeley Companies.

<details>
<summary>Full work history</summary>
<br>

| Years | Company | Role |
|---|---|---|
| 2025 to now | Day & Night Solar | Finance & Operations Analyst |
| 2025 | Keeley Companies | Data Analyst (contract), ERP migration |
| 2022 to 2023 | Curtiss-Wright | Staff Accountant, SAP and Oracle |
| 2021 to 2022 | Robert Half | Consultant, reconciliation for Elgi, Essity, Mood Media |
| 2019 to 2021 | NTT | Reconciliation Analyst, Cisco and Dell accounts |
| 2019 | Wells Fargo | Trading Service Rep (SIE, Series 7/63 program) |
| 2018 to 2019 | Walmart eCommerce | Accounts Payable, 800+ vendors |
| 2005 to 2018 | Top Nails Tech | Owner, team of six |

</details>

## Other projects

- **Cinemetrics:** movie data app on Node, Express and MongoDB. My SavvyCoders capstone. [Live site](https://capstonesavvycoders.netlify.app/) · [Code](https://github.com/jamesmnguyen704/CapstoneSavvyCoders)
- **[TripleTen data science](https://github.com/jamesmnguyen704/TripleTenProgram):** 16 projects, from EDA and hypothesis testing to machine learning.

## Tools

Python, SQL, SQLite, FastAPI, pandas, pytest, GitHub Actions, Claude Code, JavaScript and Node. On the accounting side: QuickBooks Enterprise, SAP, Oracle, Sage, Excel.

BA in Accounting, Belmont Abbey College (2012). Data Science, TripleTen (2024). Full Stack Web Development, SavvyCoders (2025).

## Contact

[LinkedIn](https://linkedin.com/in/jamesmnguyen704) · [Portfolio](https://jamesnguyen.netlify.app/) · [Email](mailto:jamesmnguyen704@outlook.com)
