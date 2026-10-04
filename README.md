# James Nguyen

**I build the systems finance and operations run on.**

I'm a finance and operations analyst and the in-house developer at Day & Night Solar, a commercial solar and energy storage contractor in the St. Louis area. I spent 10+ years in accounting and reconciliation, and ran my own small business for 13 years before that. These days I write the Python, SQL and agent workflows that replace work I used to do by hand.

## What I build

- **Data pipelines.** Messy exports from banks, accounting software and documents go into one local warehouse, and the reports rebuild from there. Every number can be traced back to its source.
- **Finance automation.** QuickBooks imports that fail closed: if a file doesn't pass validation, nothing gets imported. Bank reconciliation that scores each match by confidence and sends unclear ones to a review queue.
- **AI workflows.** Claude Code agents and MCP tools, each scoped to one job, that can draft and check work but can't import, send or publish anything without my approval. I also run models locally (llama.cpp, Ollama, ComfyUI/SDXL LoRA training).

My work systems are private, so this page covers how they work and leaves out the details. The projects below are personal and public.

## Featured projects

| Project | What it is | Stack | Links |
|---|---|---|---|
| **Cinemetrics** | App for finding movies, TV and games: what's trending, what's on each streaming service, what's playing near a ZIP code, and entertainment news. Built without a framework. Started as my SavvyCoders capstone and I still maintain it (100+ commits). | Vanilla JS SPA, Express, MongoDB, TMDB | [Live](https://capstonesavvycoders.netlify.app/) · [Code](https://github.com/jamesmnguyen704/CapstoneSavvyCoders) |
| **No-Whey** | Checks ingredient lists for dairy. Returns **SAFE**, **UNSAFE** or **REVIEW REQUIRED** and says why. The rules live in YAML, so they can be read and reviewed. | FastAPI, vanilla JS PWA | [Live](https://no-whey.onrender.com) |
| **Bait & Switch** | Fishing map for the Midwest: 200+ curated waters, a live Illinois DNR depth overlay and OpenStreetMap boat ramps. | React, Vite, Leaflet | [Live](https://bait-and-switch-ruddy.vercel.app) |
| **TripleTen Data Science** | 16 projects covering EDA, hypothesis testing and ML. Includes churn prediction with CatBoost (AUC-ROC 0.844) and a CNN that estimates age from photos (~7-year MAE). | Python, pandas, scikit-learn, CatBoost, Keras | [Code](https://github.com/jamesmnguyen704/TripleTenProgram) |

<details>
<summary><b>Private projects (explained without the code)</b></summary>
<br>

- **Atlas:** a personal data lakehouse that runs locally. Raw exports move through staging into canonical tables, and the views get generated from those. Search runs on SQLite FTS5, and local LLMs answer questions against it. Nothing leaves the machine.
- **Garden OS:** structured garden records. CSV files are the source of truth, Python scripts work on them, and a static HTML hub plus a local web form handle input.

</details>

## How I work

- **Unknown is a valid answer.** If data is unmatched, stale or missing, it gets shown as that. It doesn't get filled in with a convenient guess.
- **A person approves.** Imports, emails and anything else that leaves the system gets staged for a human to sign off.
- **Check the output.** A passing run doesn't prove much. Check what the run actually produced.

## Writing

I write short lessons on finance automation, data work and building with AI agents: **[jamesnguyen.netlify.app/blog](https://jamesnguyen.netlify.app/blog)**

## Toolbox

- **Data:** Python · SQL · SQLite · pandas · scikit-learn · pytest · Jupyter
- **Web:** FastAPI · JavaScript · Node/Express · MongoDB · React · Astro
- **AI:** Claude Code · MCP · llama.cpp · Ollama · ComfyUI
- **Finance:** QuickBooks Enterprise · SAP · Oracle · Sage · Excel

BA in Accounting · Data Science, TripleTen (2024) · Full Stack Web Development, SavvyCoders (2025)

## Contact

[Portfolio](https://jamesnguyen.netlify.app) · [LinkedIn](https://www.linkedin.com/in/jamesmnguyen704/) · [GitLab](https://gitlab.com/jamesmnguyen704) · [Facebook](https://www.facebook.com/jamesmnguyen704/) · [Email](mailto:jamesmnguyen704@outlook.com)
