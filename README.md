# Month 13 — Agentic AI & Advanced GenAI Portfolio
**Deepanshu Garg | [@deepanshu0110](https://github.com/deepanshu0110)**

> The final month of a 13-month Data Science & AI self-study program.
> Covers LangGraph, MCP (Model Context Protocol), CrewAI, and LoRA/QLoRA fine-tuning —
> the agentic AI stack needed for freelance RAG/agent work and Netherlands MSc-level project depth.

**Full Month 13 result: 1600/1600 + 80★, 16/16 days perfect.**
This repo holds Days 200–212 (foundations + mini-projects). The Days 213–216 capstone —
a LangGraph agent with a fine-tuned classifier and a 208x latency fix — is a standalone,
starred repo: **[teleserve-agentic-router](https://github.com/deepanshu0110/teleserve-agentic-router)**.

---

## Contents (Days 200–212)

| Day | Topic | File |
|-----|-------|------|
| 200 | LangGraph Fundamentals | `Day200_LangGraph_Fundamentals.ipynb` |
| 201 | LangGraph — Multi-Turn & Checkpointing | `Day201_LangGraph_MultiTurn_Checkpointing.ipynb` |
| 202 | Streaming, Parallel Nodes & Retry | `Day202_Streaming_Parallel_Retry.ipynb` |
| 203 | TeleServe Mini-Project | `Day203_TeleServe_MiniProject.ipynb` |
| 204 | ResumeGapAI as an MCP Server | `Day204_ResumeGapAI_MCP_Server.ipynb` |
| 205 | MCP Client + LangGraph Agent | `Day205_MCP_Client_LangGraph_Agent.ipynb` |
| 206 | CrewAI Fundamentals | `Day206_CrewAI_Fundamentals.ipynb` |
| 207 | CrewAI + MCP Mini-Project | `Day207_CrewAI_MCP_Mini_Project.ipynb` |
| 208 | LoRA / QLoRA Fundamentals | `day208_LoRA_QLoRA_Fundamentals.ipynb` |
| 209 | QLoRA Training Run | `day209_QLoRA_Training_Run.ipynb` |
| 210 | Evaluation Report | `day210_Evaluation_Report.ipynb` |
| 211 | Inference Wrapper | `day211_Inference_Wrapper.ipynb` |
| 212 | Capstone Ideation & Scope | `Day212_Capstone_Ideation_Scope.ipynb` |

Supporting datasets: `teleserve_tickets_209.csv`, `hard_test_210.csv`, `test_templated_210.csv`, `day211_test_tickets.csv` (TeleServe India support-ticket data, priority levels P1/P2/P3). `resumegap_engine.py` is the matching engine reused from Month 12, exposed as an MCP tool in Day 204.

---

## What this covers

- **LangGraph (200–203):** `StateGraph` construction, conditional routing, multi-turn conversation with checkpointing, streaming/parallel execution with retry logic.
- **MCP (204–205):** Wrapping an existing app (ResumeGapAI) as an MCP server, then building an MCP client consumed by a LangGraph agent — the same protocol pattern used to connect Claude to external tools.
- **CrewAI (206–207):** Multi-agent orchestration with role-based agents, tool use, and hierarchical/sequential process management.
- **LoRA/QLoRA (208–211):** Fine-tuning DistilBERT with quantized low-rank adapters on a ticket-classification task, from training through evaluation to a production inference wrapper.
- **212:** Scoping the Days 213–216 capstone that ties all of the above into one deployed agent.

## Tech Stack
`langgraph==1.2.8` · `langchain-groq` · `fastmcp==3.4.4` · `crewai==1.15.2` · `litellm` · `peft` / `bitsandbytes` (LoRA/QLoRA) · `transformers` · Groq API (`openai/gpt-oss-20b`) · Google Colab (T4 GPU)

## Program Context
Month 13 of a 13-month data analytics → data science → agentic AI self-study program, following [Month12-Capstone-Portfolio](https://github.com/deepanshu0110/Month12-Capstone-Portfolio). The capstone this month scopes lives on in [teleserve-agentic-router](https://github.com/deepanshu0110/teleserve-agentic-router), live at [teleserve-agentic-router-tmwo3kyftn9ix8mdgaqk64.streamlit.app](https://teleserve-agentic-router-tmwo3kyftn9ix8mdgaqk64.streamlit.app).
