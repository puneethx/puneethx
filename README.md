
<div  align="center">

  

<img src="https://github.com/Anmol-Baranwal/Cool-GIFs-For-GitHub/assets/74038190/d48893bd-0757-481c-8d7e-ba3e163feae7" />

  

<br/><br/>

  

[![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=26&duration=2800&pause=800&color=6CC644&center=true&vCenter=true&multiline=true&width=900&height=140&lines=Hi%2C+I'm+Puneeth+Reddy+%F0%9F%91%8B;AI+Application+Engineer+%40+Infosys;I+build+multi-agent+systems+that+ship+to+production;LangGraph+%C2%B7+RAG+%C2%B7+SAP+Joule+%C2%B7+MCP+%C2%B7+FastAPI)](https://git.io/typing-svg)

  

[![Portfolio](https://img.shields.io/badge/Portfolio-puneeth--reddy.vercel.app-6CC644?style=for-the-badge&logo=vercel&logoColor=white)](https://puneeth-reddy.vercel.app/)

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Puneeth_Reddy-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/puneeth-reddy-75069824b/)

[![Gmail](https://img.shields.io/badge/Email-puneethreddyt2004-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:puneethreddyt2004@gmail.com)

[![Profile Views](https://komarev.com/ghpvc/?username=puneethx&style=for-the-badge&color=6CC644)](https://github.com/puneethx)

  

</div>

  

---

  

## 🧠 whoami

  

```yaml

name: T Puneeth Reddy

role: AI Application Engineer · Forward Deployed Engineer

company: Infosys · Bangalore, India

focus: Agentic AI · Multi-Agent Orchestration · Grounded RAG

shipping: Production Joule + LangGraph agents on SAP BTP

featured: SAP SAPPHIRE 2026 · SAP Business Accelerator Hub (3 agents published by SAP)

mission: Take agents from a notebook idea → to real users → to measurable outcomes

```

  

> 🤖 I build agents that **do things**, not just chat. Retrieval-grounded, tool-using, multi-step, audited — and running against real enterprise SAP workloads.

  

---

  

## 🕸️ The Agent Graph I Ship Every Day

  

Because a screenshot beats a bullet list. This is roughly what my day looks like:

  

```mermaid

%%{init: {'theme':'dark', 'themeVariables': { 'primaryColor':'#0d1117','primaryTextColor':'#6CC644','lineColor':'#6CC644','fontFamily':'JetBrains Mono'}}}%%

flowchart LR

U([👤 User<br/>plain english]) --> S{{🧭 Supervisor Agent<br/>classify + route}}

  

S -->|knowledge| K[📚 Knowledge Agent<br/>Hybrid RAG · BM25+Cosine+RRF]

S -->|data| D[📊 Data Agent<br/>OData V4 · live $metadata]

S -->|exception| E[⚠️ Exception Agent<br/>Runbook + evidence]

  

K --> SY[[🧬 Synthesis Agent<br/>compose + cite]]

D --> SY

E --> SY

  

SY --> G{{🛡️ Guardrail<br/>faithfulness ≥ threshold?}}

G -->|✅ grounded| A([💬 Answer + citations])

G -->|❌ ungrounded| R([🚫 Refuse])

  

classDef agent fill:#161b22,stroke:#6CC644,stroke-width:1.5px,color:#c9d1d9;

classDef gate fill:#0d1117,stroke:#f0883e,stroke-width:1.5px,color:#f0883e;

classDef io fill:#0d1117,stroke:#58a6ff,stroke-width:1.5px,color:#58a6ff;

class S,K,D,E,SY agent;

class G gate;

class U,A,R io;

```

  

That's **SAP Enterprise Copilot** — 5 agents on LangGraph, hybrid retrieval, deterministic grounding. No hallucinated answers get out the door.

  

---

  

## 🚀 Currently Shipping

  

<table>

<tr>

<td width="50%" valign="top">

  

### 🤖 SAP MAO Warehouse Agent

**Live at SAPPHIRE 2026 · Published on SAP Accelerator Hub**

  

A multi-agent Joule system that acts as **the brain behind a fleet of 120 autonomous robots**. When a robot hits an empty-bin exception, my agents:

  

- 🔎 Diagnose the exception in real time

- 📦 Locate the next valid bin via EWM

- 🚦 Reroute the robot or trigger putaway from reserve storage

- ✍️ Write the resolution back to HANA — no human logs into SAP

  

`Supervisor` → `Inventory` → `Logistics` agents · Joule Studio · SAP BTP

  

</td>

<td width="50%" valign="top">

  

### 🦾 DRA — Humanoid Robot Agent

**Under active development · Infosys R&D**

  

The follow-up to SAPPHIRE. Same agentic backbone, but now driving a **humanoid** through pick-and-place, navigation, and inspection tasks — all via plain-english prompts.

  

- 🧭 Supervisor classifies task → routes to specialist

- 👁️ Vision system feeds the inspection agent

- 🔁 Failure-recovery loop being built out now

  

Because manipulating physical space is the ultimate agentic benchmark.

  

</td>

</tr>

<tr>

<td width="50%" valign="top">

  

### 🔐 SAP Security Audit Agent

**Published on SAP Accelerator Hub**

  

Auditors ask in plain english — *"which roles allow creating a sales order?"* — the agent generates **ABAP Open SQL** against `AGR_USERS` / `AGR_1251` / `USR02`, executes read-only via OData on BTP, and streams a clean table into the chat. Hours → seconds.

  

</td>

<td width="50%" valign="top">

  

### 🔍 SAP Search + Troubleshooter Agents

**Published on SAP Accelerator Hub**

  

Two Joule agents (+ a Python/ReAct twin) that **query-expand**, scrape live SAP Help / Notes / Community, and synthesize structured answers with citations. The Python version runs a ReAct loop with three specialized Tavily tools + GPT-4.1 via SAP AI Core.

  

</td>

</tr>

</table>

  

---

  

## 🧰 Tech I Actually Use

  

<details open>

<summary><b>🤖 Agentic AI & GenAI</b> — where I spend most of my time</summary>

  

![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)

![LangGraph](https://img.shields.io/badge/LangGraph-FF6F61?style=flat&logo=langgraph&logoColor=white)

![Claude](https://img.shields.io/badge/Claude-D97757?style=flat&logo=anthropic&logoColor=white)

![OpenAI](https://img.shields.io/badge/GPT--4.1-412991?style=flat&logo=openai&logoColor=white)

![MCP](https://img.shields.io/badge/MCP-000000?style=flat&logo=anthropic&logoColor=white)

![RAG](https://img.shields.io/badge/Hybrid_RAG-6CC644?style=flat&logo=databricks&logoColor=white)

![ReAct](https://img.shields.io/badge/ReAct_Agents-FF9E0F?style=flat&logo=react&logoColor=white)

![Tavily](https://img.shields.io/badge/Tavily-1E90FF?style=flat&logoColor=white)

  

</details>

  

<details open>

<summary><b>⚙️ Backend, APIs & Runtime</b></summary>

  

![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)

![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=openjdk&logoColor=white)

![Node.js](https://img.shields.io/badge/Node.js-6DA55F?style=flat&logo=node.js&logoColor=white)

![Express](https://img.shields.io/badge/Express.js-404d59?style=flat&logo=express&logoColor=61DAFB)

![SSE](https://img.shields.io/badge/SSE_Streaming-FF4500?style=flat&logoColor=white)

![REST](https://img.shields.io/badge/REST_APIs-25A162?style=flat&logo=fastapi&logoColor=white)

  

</details>

  

<details open>

<summary><b>🏢 SAP Stack</b> — where the agents run</summary>

  

![SAP BTP](https://img.shields.io/badge/SAP_BTP-0FAAFF?style=flat&logo=sap&logoColor=white)

![Joule Studio](https://img.shields.io/badge/Joule_Studio-1D7CBF?style=flat&logo=sap&logoColor=white)

![SAP CAP](https://img.shields.io/badge/SAP_CAP_(CAPM)-0057A4?style=flat&logo=sap&logoColor=white)

![SAP AI Core](https://img.shields.io/badge/SAP_AI_Core-0FAAFF?style=flat&logo=sap&logoColor=white)

![SAPUI5](https://img.shields.io/badge/SAPUI5/Fiori-0FAAFF?style=flat&logo=sap&logoColor=white)

![S/4HANA](https://img.shields.io/badge/S%2F4HANA-0FAAFF?style=flat&logo=sap&logoColor=white)

![EWM](https://img.shields.io/badge/SAP_EWM-0057A4?style=flat&logo=sap&logoColor=white)

![OData V4](https://img.shields.io/badge/OData_V4-CE0000?style=flat&logoColor=white)

  

</details>

  

<details>

<summary><b>🧪 ML / Computer Vision</b> — where I started</summary>

  

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)

![Lightning](https://img.shields.io/badge/PyTorch_Lightning-792EE5?style=flat&logo=pytorchlightning&logoColor=white)

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat&logo=tensorflow&logoColor=white)

![YOLO](https://img.shields.io/badge/YOLOv8-00FFFF?style=flat&logo=yolo&logoColor=black)

![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat&logo=opencv&logoColor=white)

  

</details>

  

<details>

<summary><b>🎨 Frontend & Everything Else</b></summary>

  

![React](https://img.shields.io/badge/React-20232a?style=flat&logo=react&logoColor=61DAFB)

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat&logo=nextdotjs&logoColor=white)

![R3F](https://img.shields.io/badge/React_Three_Fiber-000000?style=flat&logo=three.js&logoColor=white)

![Streamlit](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)

![Tailwind](https://img.shields.io/badge/TailwindCSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white)

![MongoDB](https://img.shields.io/badge/MongoDB-4ea94b?style=flat&logo=mongodb&logoColor=white)

![Git](https://img.shields.io/badge/Git-fc6d26?style=flat&logo=git&logoColor=white)

![Figma](https://img.shields.io/badge/Figma-F24E1E?style=flat&logo=figma&logoColor=white)

  

</details>

  

---

  

## 🏆 Wall of Wins

  

- 🎤 **SAP SAPPHIRE 2026** — contributed to an agent showcased live at SAP's biggest global conference

- 📦 **3 Joule Agents published to SAP Business Accelerator Hub — by SAP themselves**

- 🥇 **Winner** · Proglint CV 2K23 National Hackathon (Alliance University, Bangalore)

- 🥈 **1st Runner-up** · SheCodes by WTM Reva — Llava-8B + R3F adaptive learning

- 🥈 **1st Runner-up** · HackQuest by I-Quest (VIT-AP) — YOLO + OCR traffic AI

- 🥈 **1st Runner-up** · FrameX Web Hackathon (CSI, VIT-AP)

- 📜 **Claude Certified Architect — Foundations**

  

---

  

## 📊 GitHub Stats

  

<div  align="center">

  

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=puneethx&theme=material-palenight&hide_border=true&include_all_commits=false&count_private=false" />

<img height="180em" src="https://github-readme-streak-stats.herokuapp.com/?user=puneethx&theme=material-palenight&hide_border=true" />

  

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=puneethx&theme=material-palenight&hide_border=true&include_all_commits=false&count_private=false&layout=compact" />

  

<img src="https://github-profile-trophy.vercel.app/?username=puneethx&theme=radical&no-frame=true&no-bg=true&margin-w=4&column=7" />

  

<img src="https://raw.githubusercontent.com/platane/snk/output/github-contribution-grid-snake-dark.svg" alt="snake" />

  

</div>

  

---

  

## 🌐 Let's Talk

  

<div  align="center">

  

If you're building agents, shipping GenAI to real users, or figuring out how to keep LLMs honest with retrieval and guardrails — I'd love to trade notes.

  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/puneeth-reddy-75069824b/)

[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/puneethx)

[![Gmail](https://img.shields.io/badge/Email_Me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:puneethreddyt2004@gmail.com)

[![Portfolio](https://img.shields.io/badge/Portfolio-6CC644?style=for-the-badge&logo=vercel&logoColor=white)](https://puneeth-reddy.vercel.app/)

  

<sub>*"The interesting part isn't that it chats — it's that it acts, grounded and auditable."*</sub>

  

</div>
