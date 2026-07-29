<div align="center">

```
    ┌─────────────────────────────────────────────────────────────────┐
    │  $ ./puneeth --introduce --mode=agentic                          │
    │  [boot] loading persona...                              [  OK  ] │
    │  [boot] warming up LangGraph runtime...                 [  OK  ] │
    │  [boot] connecting to SAP BTP...                        [  OK  ] │
    │  [boot] 3 agents online · 1 humanoid on standby         [ LIVE ] │
    └─────────────────────────────────────────────────────────────────┘
```

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=700&size=24&duration=2600&pause=700&color=6CC644&center=true&vCenter=true&multiline=true&width=900&height=110&lines=%3E+I+don't+build+chatbots.;%3E+I+build+agents+that+move+robots%2C+query+SAP%2C+and+refuse+to+hallucinate.;%3E+Sometimes+they+show+up+at+SAPPHIRE.)](https://git.io/typing-svg)

<img src="https://readme-jokes.vercel.app/api?theme=material-palenight&hideBorder=true" alt="joke of the day"/>

</div>

---

## ▲ ` cat ~/.identity `

```jsonc
{
  "name": "T Puneeth Reddy",
  "role": "AI Application Engineer · Forward Deployed Engineer",
  "org":  "Infosys · Bangalore",
  "obsession": "agents that DO things, not just chat",
  "stack": ["LangGraph", "LangChain", "MCP", "Joule Studio", "SAP BTP", "FastAPI"],
  "shipped_to_production": true,
  "featured_at": "SAP SAPPHIRE 2026",
  "published_by_SAP_itself": 3,   // agents on SAP Business Accelerator Hub
  "currently_teaching": ["a humanoid robot", "how to pick, place, and inspect"],
  "hallucination_policy": "refuse if not grounded"
}
```

---

## ⌘ ` puneeth.run("who are you?") `

<pre>
<b><span style="color:#6CC644">▸ Thought</span></b>   The user wants a two-line pitch. Skip the resume. Lead with the flex.
<b><span style="color:#f0883e">▸ Action</span></b>   introduce(mode="agentic", brag_level="moderate")
<b><span style="color:#58a6ff">▸ Observation</span></b>

   I'm Puneeth — I build multi-agent systems for enterprise SAP workloads
   at Infosys. Three of my agents were published to SAP's Accelerator Hub
   by SAP themselves. One of them showed up at SAPPHIRE 2026 driving a
   fleet of 120 autonomous robots on stage. My favourite hobby is arguing
   with LLMs until they stop hallucinating.

<b><span style="color:#6CC644">▸ Thought</span></b>   Good. Now stop before it turns into a bio.
<b><span style="color:#f0883e">▸ Action</span></b>   FINISH
</pre>

---

## ⚡ ` /tools ` — what I reach for

```bash
$ puneeth --list-tools --category=agentic
```

| tool                     | what I use it for                                                              |
|--------------------------|--------------------------------------------------------------------------------|
| `LangGraph`              | Multi-agent state graphs · fan-out/fan-in · shared typed state                 |
| `LangChain`              | ReAct loops · tool wiring · prompt composition                                 |
| `MCP` (Model Context Protocol) | Standardized tool exposure — LLM ↔ any data source without glue code     |
| `Hybrid RAG (BM25 + Cosine + RRF)` | Retrieval that survives real technical vocabulary (t-codes, tables)  |
| `OKF` (Open Knowledge Format)      | YAML-typed runbooks · precise structured lookups (not fuzzy vectors) |
| `Joule Studio`           | Enterprise-native agents deployed on SAP BTP                                   |
| `SAP CAP + OData V4`     | Live schema-aware data agents · read-only guardrails at the service layer      |
| `FastAPI + SSE`          | Streaming agent tokens straight into a Fiori UI                                |
| `Faithfulness guardrail` | Deterministic grounding check — no citation, no answer                         |

---

## 🛰️ ` /agents ` — currently in production

<table>
<tr>
<td width="55%" valign="top">

<b>⚙️ MAO Warehouse Fulfillment Agent</b>
<sub><code>🔴 LIVE · Joule · SAP BTP · SAPPHIRE 2026</code></sub>

The brain behind a fleet of <b>120 autonomous mobile robots</b>. When a robot
hits an empty-bin exception, my agents diagnose it, find the next valid
bin from EWM, reroute or trigger putaway from reserve storage, and write
the fix back to HANA — <i>no human ever logs into SAP</i>.

Supervisor → Inventory → Logistics. Ran live on stage at SAPPHIRE.

</td>
<td width="45%" valign="top">

<b>🦾 DRA · Daksha Humanoid Agent</b>
<sub><code>🟡 IN DEV · Joule · Humanoid Robotics</code></sub>

Successor to SAPPHIRE. Same agentic backbone, now driving a <b>humanoid</b>
through pick-and-place, navigation, and bin inspection — every action
kicked off by a plain-english prompt.

Because if your agent can't manipulate atoms, it's just a chatbot with
better PR.

</td>
</tr>
<tr>
<td width="55%" valign="top">

<b>🔐 SAP Security Audit Agent</b>
<sub><code>🟢 SHIPPED · Joule · SAP Accelerator Hub</code></sub>

Auditors ask <i>"which roles allow creating a sales order?"</i>. The agent
generates <b>ABAP Open SQL</b> against <code>AGR_USERS</code> /
<code>AGR_1251</code> / <code>USR02</code>, executes read-only via OData on
BTP, streams a clean table into the chat. Hours → seconds.

</td>
<td width="45%" valign="top">

<b>🧬 SAP Enterprise Copilot</b>
<sub><code>🟢 SHIPPED · LangGraph · Python</code></sub>

Five agents. Hybrid retrieval. Deterministic grounding guardrail.
<b>Zero</b> ungrounded answers get out the door — every sentence must cite
its source or it doesn't ship.

My favourite thing I've built.

</td>
</tr>
<tr>
<td width="55%" valign="top">

<b>🔎 SAP Search + Troubleshooter Agents</b>
<sub><code>🟢 SHIPPED · Joule + Python/ReAct twin · SAP Accelerator Hub</code></sub>

Query-expand → scrape SAP Help / Notes / Community live → synthesize a
structured answer with references. Python version runs a ReAct loop
with 3 specialized Tavily tools + GPT-4.1 via SAP AI Core.

</td>
<td width="45%" valign="top">

<b>📦 Northwind MCP Data Agent</b>
<sub><code>🟢 POC · MCP · LangChain</code></sub>

Natural-language → MCP tool call → OData → formatted answer.
Built specifically to <i>deeply</i> understand MCP internals before betting
production on it.

</td>
</tr>
</table>

---

## 🧪 ` /demo ` — a real prompt from Enterprise Copilot

<pre>
<b><span style="color:#58a6ff">user</span></b>   "Why is bin A-12-03 showing empty when PO-5003 says stock arrived?"

<b><span style="color:#6CC644">supervisor</span></b>    classify → exception · route → [exception_agent, data_agent]
<b><span style="color:#f0883e">data_agent</span></b>    OData $metadata read → generated OData V4 query → 3 rows
<b><span style="color:#f0883e">exception</span></b>     OKF.lookup("BIN_MISMATCH") → runbook (5 ordered steps)
<b><span style="color:#f0883e">exception</span></b>     calls data_agent again → cross-checks goods receipt in MM
<b><span style="color:#a371f7">synthesis</span></b>     compose answer with inline [S1] [S2] [DATA] citations
<b><span style="color:#ff6b6b">guardrail</span></b>     faithfulness = 0.94 · ≥ threshold · ✅ deliver

<b><span style="color:#c9d1d9">answer</span></b>        "PO-5003 arrived at dock D-02 but the Goods Receipt was
              never posted [DATA]. Per BIN_MISMATCH runbook [S1], the
              bin will show empty until GR is posted. Post GR via MIGO
              or trigger the automated action below…"
</pre>

That's the whole point: **an answer, grounded and auditable — not a search result.**

---

## 🏆 ` /wall-of-wins `

```
[2026] 🎤 SAPPHIRE 2026 · agent I contributed to demoed live on stage
[2026] 📦 3× Joule Agents published to SAP Business Accelerator Hub — by SAP
[2025] 🎓 B.Tech CS · VIT-AP · CGPA 8.06
[2024] 🚀 Joined Infosys straight after grad → shipped to prod in year one
[2024] 🥈 1st Runner-up · SheCodes by WTM Reva (Llava-8B + R3F adaptive learning)
[2024] 🥈 1st Runner-up · HackQuest · VIT-AP (YOLO + OCR traffic AI)
[2024] 🥈 1st Runner-up · FrameX Web Hackathon · CSI VIT-AP
[2023] 🥇 Winner · Proglint CV 2K23 National Hackathon · Alliance University
[----] 📜 Claude Certified Architect — Foundations
```

---

## 📈 ` /telemetry `

<div align="center">

<img height="165em" src="https://github-readme-stats.vercel.app/api?username=puneethx&theme=material-palenight&hide_border=true&include_all_commits=false&count_private=false" />
<img height="165em" src="https://github-readme-streak-stats.herokuapp.com/?user=puneethx&theme=material-palenight&hide_border=true" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=puneethx&theme=material-palenight&hide_border=true&include_all_commits=false&count_private=false&layout=compact" />

<img src="https://github-profile-trophy.vercel.app/?username=puneethx&theme=radical&no-frame=true&no-bg=true&margin-w=4&column=7" />

<img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" alt="snake eating my contributions"/>

</div>

---

## 📡 ` /open-a-channel `

<div align="center">

```python
# I'm always up for talking agents, retrieval, grounding,
# or "how do we actually put this in front of real users"
```

[![Portfolio](https://img.shields.io/badge/▲_puneeth--reddy.vercel.app-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://puneeth-reddy.vercel.app/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/puneeth-reddy-75069824b/)
[![Gmail](https://img.shields.io/badge/puneethreddyt2004@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:puneethreddyt2004@gmail.com)
[![Instagram](https://img.shields.io/badge/@puneethx-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/puneethx)
[![Views](https://komarev.com/ghpvc/?username=puneethx&style=for-the-badge&color=6CC644&label=humans+observed)](https://github.com/puneethx)

<br/>

<sub><code>$ end of transcript · agent still running · next prompt?</code></sub>

</div>
