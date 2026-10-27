<h1 align="center">James Nguyen</h1>
<p align="center"><b>Finance and Operation Analyst · I build the systems finance and operations run on</b></p>

<p align="center">
  <img src="https://img.shields.io/badge/Data_Architecture-1f6feb?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Finance_Automation-2ea043?style=for-the-badge" />
  <img src="https://img.shields.io/badge/AI_Agent_Operations-8957e5?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Internal_Controls-d29922?style=for-the-badge" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/jamesmnguyen704/"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?logo=linkedin&logoColor=white" /></a>
  <a href="https://jamesnguyen.netlify.app/blog"><img src="https://img.shields.io/badge/Blog-000000?logo=netlify&logoColor=white" /></a>
</p>

Accountant turned builder. 10+ years in accounting and reconciliation and 13 years running my own business. Now I'm the in-house developer at a commercial solar and storage contractor, where I designed and run the company's finance and operations platform end to end.

---

## The platform I built (private, case study)

> An AI-assisted finance and operations platform for a commercial solar contractor. I designed it and direct the build. The code and data are private, so this shows how it works, not what's in it.

<table>
<tr>
<td align="center"><h2>170+</h2>warehouse tables</td>
<td align="center"><h2>~50</h2>automated loaders</td>
<td align="center"><h2>~150</h2>daily pipeline steps</td>
<td align="center"><h2>~20</h2>chartered AI agents</td>
<td align="center"><h2>1,000+</h2>issues tracked to closed</td>
<td align="center"><h2>~2,500</h2>automated tests</td>
</tr>
</table>

```mermaid
flowchart LR
  A[Bank feeds] --> L
  B[Accounting exports] --> L
  C[Project docs<br/>estimates · invoices] --> L
  L[ELT loaders<br/>load stamps · lineage] --> W[(Analytics warehouse<br/>170+ tables)]
  W --> Q{Quality gates<br/>health score · freshness<br/>unknown = hold}
  Q --> D[Dashboards<br/>company hub · per-project<br/>ownership · data quality]
  Q --> R[Reconciliation<br/>bank is truth<br/>append-only verdicts]
  R --> S[Staged ledger entries<br/>fail-closed safety gate]
  AG[AI agents<br/>scoped charters] -.draft & check.-> R
  AG -.draft.-> S
  S --> H((Human<br/>approves))
  H --> GL[General ledger]
```

**What it does**

| Area | What I built |
|---|---|
| 🗄️ **Data architecture** | One governed analytics warehouse that replaced scattered spreadsheets. Every table carries its source, load time, owner and a data-quality health score. |
| 🏦 **Reconciliation** | Bank-first matching of every bank transaction to the ledger. Verdicts are append-only, so the audit trail can't be overwritten. |
| 🧾 **Ledger automation** | Purchase orders, bills, invoices and payments generated as import files behind a fail-closed validation gate. A person approves every posting. |
| 📊 **Dashboards** | A company operations hub, a page for each active project (budget → POs → spend → milestones), and system-health boards, all rebuilt from the warehouse every day. |
| ⚙️ **Pipeline** | A scheduled daily run of ~150 steps that records every step's status, so a partial run never passes for a complete one. |
| 🤖 **AI operations** | ~20 Claude Code agents, each scoped to one job (books, bank, projects, tax, data quality, dashboards). Ownership registry, issue register and a decision log of 240+ rulings. Agents propose; a human approves money, tax and anything external. |
| 🛡️ **Controls** | Pre-commit gates for secrets and unsafe changes, rolled out report-only first, then enforced. |

**Principles:** Unknown is a valid answer · The bank is the source of truth · A person approves · Check the output, not the exit code

---

## Public projects

<table>
<tr>
<td width="50%" valign="top">
<b>🎬 Cinemetrics</b><br/>
Find movies, TV and games: trending, where to stream, what's playing near a ZIP code. No framework. SavvyCoders capstone, still maintained (100+ commits).<br/>
<img src="https://img.shields.io/badge/-Vanilla_JS-F7DF1E?logo=javascript&logoColor=black" /> <img src="https://img.shields.io/badge/-Express-000?logo=express" /> <img src="https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white" /><br/>
<a href="https://capstonesavvycoders.netlify.app/">Live</a> · <a href="https://github.com/jamesmnguyen704/CapstoneSavvyCoders">Code</a>
</td>
<td width="50%" valign="top">
<b>🥛 No-Whey</b><br/>
Checks ingredient lists for dairy and returns SAFE, UNSAFE or REVIEW REQUIRED with the reason. Rules live in readable YAML.<br/>
<img src="https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white" /> <img src="https://img.shields.io/badge/-PWA-5A0FC8?logo=pwa&logoColor=white" /><br/>
<a href="https://no-whey.onrender.com">Live</a>
</td>
</tr>
<tr>
<td width="50%" valign="top">
<b>🎣 Bait &amp; Switch</b><br/>
A Midwest fishing map: 200+ curated waters, a live Illinois DNR depth overlay and OpenStreetMap boat ramps.<br/>
<img src="https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=black" /> <img src="https://img.shields.io/badge/-Vite-646CFF?logo=vite&logoColor=white" /> <img src="https://img.shields.io/badge/-Leaflet-199900?logo=leaflet&logoColor=white" /><br/>
<a href="https://bait-and-switch-ruddy.vercel.app">Live</a>
</td>
<td width="50%" valign="top">
<b>📈 TripleTen Data Science</b><br/>
16 projects: EDA, hypothesis testing and ML. Churn prediction with CatBoost (AUC-ROC 0.844) and a CNN that estimates age from photos (~7-year MAE).<br/>
<img src="https://img.shields.io/badge/-pandas-150458?logo=pandas" /> <img src="https://img.shields.io/badge/-scikit--learn-F7931E?logo=scikitlearn&logoColor=white" /> <img src="https://img.shields.io/badge/-Keras-D00000?logo=keras&logoColor=white" /><br/>
<a href="https://github.com/jamesmnguyen704/TripleTenProgram">Code</a> · <a href="https://jamesnguyen.netlify.app">Portfolio</a>
</td>
</tr>
</table>

---

## Toolbox

**Data** <img src="https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white" /> <img src="https://img.shields.io/badge/-SQL-4479A1?logo=postgresql&logoColor=white" /> <img src="https://img.shields.io/badge/-SQLite-003B57?logo=sqlite&logoColor=white" /> <img src="https://img.shields.io/badge/-pandas-150458?logo=pandas" /> <img src="https://img.shields.io/badge/-pytest-0A9EDC?logo=pytest&logoColor=white" /> <img src="https://img.shields.io/badge/-Jupyter-F37626?logo=jupyter&logoColor=white" />

**AI** <img src="https://img.shields.io/badge/-Claude_Code-D97757?logo=anthropic&logoColor=white" /> <img src="https://img.shields.io/badge/-MCP-000000" /> <img src="https://img.shields.io/badge/-Ollama-000000?logo=ollama" /> <img src="https://img.shields.io/badge/-llama.cpp-555" /> <img src="https://img.shields.io/badge/-ComfyUI-333" />

**Web** <img src="https://img.shields.io/badge/-FastAPI-009688?logo=fastapi&logoColor=white" /> <img src="https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black" /> <img src="https://img.shields.io/badge/-Node.js-339933?logo=nodedotjs&logoColor=white" /> <img src="https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=black" /> <img src="https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white" /> <img src="https://img.shields.io/badge/-Astro-BC52EE?logo=astro&logoColor=white" />

**Finance** <img src="https://img.shields.io/badge/-QuickBooks_Enterprise-2CA01C?logo=intuit&logoColor=white" /> <img src="https://img.shields.io/badge/-SAP-0FAAFF?logo=sap&logoColor=white" /> <img src="https://img.shields.io/badge/-Oracle-F80000?logo=oracle&logoColor=white" /> <img src="https://img.shields.io/badge/-Sage-00D639" /> <img src="https://img.shields.io/badge/-Excel-217346?logo=microsoftexcel&logoColor=white" />

**Credentials:** BA Accounting · Data Science, TripleTen (2024) · Full Stack Web Dev, SavvyCoders (2025) · Anthropic Academy: Claude Code, MCP, AI Fluency, Cowork

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=jamesmnguyen704&hide_rank=true&show_icons=true&hide_border=true" height="150"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=jamesmnguyen704&hide=jupyter%20notebook,html,css&layout=compact&hide_border=true" height="150"/>
</p>

<!--
PICTURES TO ADD (save into the profile repo as /img/*.png):
- cinemetrics.png, nowhey.png, baitswitch.png: a screenshot of each live site (Win+Shift+S).
- tripleten-chart.png: one chart from a TripleTen notebook (e.g. the ROC curve).
- dashboard-demo.png: NEVER a real work screenshot. Only a dashboard rebuilt with fake data, or skip it. The mermaid diagram above already renders as a picture on GitHub.
Then swap each "IMG: x.png" line for: <img src="img/x.png" width="100%"/>
-->
