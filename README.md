<div align="center">

# Ayush Pandey

AI Engineer @ Yellow.ai · building [versionCV](https://www.versioncv.com) (independent) · MCP & agentic systems

[![Portfolio](https://img.shields.io/badge/ayushpandey.me-0D1117?style=flat-square&logo=googlechrome&logoColor=00D9FF)](https://ayushpandey.me)
[![versionCV](https://img.shields.io/badge/versioncv.com-0D1117?style=flat-square&logo=vercel&logoColor=white)](https://www.versioncv.com)
[![MCP](https://img.shields.io/badge/mcp.versioncv.com-0D1117?style=flat-square&logo=cloudflare&logoColor=F38020)](https://www.versioncv.com/#mcp)
[![LinkedIn](https://img.shields.io/badge/in/linkedap-0D1117?style=flat-square&logo=linkedin&logoColor=0A66C2)](https://linkedin.com/in/linkedap)
[![Email](https://img.shields.io/badge/ayushpandey.cs@gmail.com-0D1117?style=flat-square&logo=gmail&logoColor=EA4335)](mailto:ayushpandey.cs@gmail.com)

</div>

```yaml
whoami:
  role:      AI Engineer @ Yellow.ai
  building:  versioncv.com                      # independent project: AI resume platform + remote MCP server
  focus:     [agentic systems, MCP, guardrails, serverless infra]
  stack:     [TypeScript, Python, Cloudflare Workers, GCP, AWS]
  motto:     "Execution is the currency that converts ideas into value."
```

---

### ▸ Highlights

| Signal | Detail |
|---|---|
| **versionCV** | Independent project · solo founder · full SDLC · MSME registered (Govt of India) · `~$0` idle infra cost |
| **Production MCP server** | 35 tools · OAuth 2.1 · Cloudflare Workers + Durable Objects · live at `mcp.versioncv.com` |
| **MCP Harness** | Open-source agent loop · any model × any MCP server · keys stay server-side |
| **Hackathon** | 2nd place out of 800 teams · Google DSC, IIT Kanpur |

---

### ▸ versionCV — AI resume platform with guardrails

[`versioncv.com`](https://www.versioncv.com) · independent project · May 2025 – present

Not an LLM wrapper: **rules find the problems → the AI fixes only those → the user approves every change**, so every line stays provable in an interview.

```text
  Browser ─────────▶ Next.js (Vercel)
                          │
  Claude / Cursor ──▶ MCP server ── OAuth 2.1 · Durable Object sessions
  VS Code                 │
                          ▼
                Cloudflare Workers ─── D1 · KV · R2 · Queues · Durable Objects
                          │
                          ▼
                Cloud Run ─── ATS engine · JD matcher · Meilisearch
                          ▲
  Greenhouse · Lever · Ashby · Workable · SmartRecruiters · Recruitee  (nightly cron)
```

| Layer | What it does |
|---|---|
| **Scoring** | Rule-based ATS checks (50+) · JD matching via skill regex normalization · graph-based skill inference |
| **LLM** | Deterministic pipeline with XML context binding · multi-model fallback (Gemini → GPT → Claude → Mistral) |
| **MCP** | 35 tools: scan, optimize, JD match, edit, save, vault, jobs, referrals · same credits & limits as the web app |
| **Jobs** | 6 ATS sources → D1 → Meilisearch · expired jobs removed nightly · JD extractor validated on 117 live JDs |
| **Workspace** | Zero-dep WYSIWYG editor · role-based versions · proof vault · resume analytics · shareable links |
| **Security** | Firebase JWT · RPC-only internal services · 4-layer rate limiting · strict CSP · Cloudflare DDoS |

<details>
<summary><b>Performance</b></summary>

| Metric | Value |
|---|---|
| Latency | `<100ms` avg |
| Capacity | `4K+ req/s` |
| Auth | `1ms` JWT verification |
| Idle cost | `~$0` (was `$250/month`) |

</details>

---

### ▸ MCP Harness — any model × any MCP server

[`ap-dev-github/mcp-harness`](https://github.com/ap-dev-github/mcp-harness) · open source (MIT)

```text
  reason ──▶ call tool ──▶ observe ──▶ repeat
     │                                    │
     └──── OpenAI · Claude · Gemini ──────┘      keys + MCP tokens stay server-side
```

- Custom agent loop in React, zero dependencies beyond React
- Model-agnostic: OpenAI-, Claude- and Gemini-style APIs (incl. OpenRouter)
- Per-user Google sign-in · rate limiting · retries · runs on Cloudflare Workers
- Tested end to end against the production versionCV MCP server

---

### ▸ Open source

**[AdenHQ / Hive](https://github.com/adenhq/hive)** · YC-backed agent framework · [PR #641](https://github.com/adenhq/hive/pull/641)

```diff
+ fixed Windows UnicodeEncodeError (cp1252) → explicit UTF-8, cross-platform stability restored
+ debugged CI/CD failures after the DX overhaul → filed issue, submitted fix PR
```

---

### ▸ More projects

| Project | Stack | Notes |
|---|---|---|
| [SwiftVault](https://github.com/ap-dev-github/swiftvault-smart-storage) | Go · GraphQL · PostgreSQL · Redis → Cloudflare Workers, KV, R2 | `$204/yr → $0` (year 1), 47% permanent |
| [Atithidev DB API](https://kzjttnxnf3.execute-api.ap-south-1.amazonaws.com/dev/) | AWS Lambda · DynamoDB | Serverless REST API |
| [Sentiment Analyzer](https://github.com/ap-dev-github/sentiment-analyzer-api) | Python · AWS Lambda · NLTK | NLP microservice |

---

### ▸ Stack

![TypeScript](https://img.shields.io/badge/TypeScript-0D1117?style=flat-square&logo=typescript&logoColor=3178C6)
![Python](https://img.shields.io/badge/Python-0D1117?style=flat-square&logo=python&logoColor=3776AB)
![Go](https://img.shields.io/badge/Go-0D1117?style=flat-square&logo=go&logoColor=00ADD8)
![Java](https://img.shields.io/badge/Java-0D1117?style=flat-square&logo=openjdk&logoColor=ED8B00)
![C++](https://img.shields.io/badge/C++-0D1117?style=flat-square&logo=cplusplus&logoColor=00599C)
![Next.js](https://img.shields.io/badge/Next.js-0D1117?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-0D1117?style=flat-square&logo=react&logoColor=61DAFB)
![Cloudflare](https://img.shields.io/badge/Cloudflare_Workers-0D1117?style=flat-square&logo=cloudflare&logoColor=F38020)
![GCP](https://img.shields.io/badge/Google_Cloud-0D1117?style=flat-square&logo=googlecloud&logoColor=4285F4)
![AWS](https://img.shields.io/badge/AWS-0D1117?style=flat-square&logo=amazonwebservices&logoColor=FF9900)
![Firebase](https://img.shields.io/badge/Firebase-0D1117?style=flat-square&logo=firebase&logoColor=FFCA28)
![Meilisearch](https://img.shields.io/badge/Meilisearch-0D1117?style=flat-square&logo=meilisearch&logoColor=FF5CAA)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-0D1117?style=flat-square&logo=postgresql&logoColor=4169E1)
![Redis](https://img.shields.io/badge/Redis-0D1117?style=flat-square&logo=redis&logoColor=DC382D)
![Docker](https://img.shields.io/badge/Docker-0D1117?style=flat-square&logo=docker&logoColor=2496ED)
![Kubernetes](https://img.shields.io/badge/Kubernetes-0D1117?style=flat-square&logo=kubernetes&logoColor=326CE5)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-0D1117?style=flat-square&logo=githubactions&logoColor=2088FF)

`MCP` `OAuth 2.1` `Agentic systems` `Guardrails` `RAG` `Embeddings` `Durable Objects` `D1` `KV` `R2`

---

<div align="center">

![GitHub Streak](https://streak-stats.demolab.com/?user=ap-dev-github&theme=github-dark-blue&hide_border=true&background=0D1117&ring=00D9FF&fire=FF6B6B&currStreakLabel=00D9FF)

**Open to:** SDE – AI Systems · AI Engineer · Serverless AI Infrastructure & Cost Optimization

[![Email](https://img.shields.io/badge/ayushpandey.cs@gmail.com-0D1117?style=flat-square&logo=gmail&logoColor=EA4335)](mailto:ayushpandey.cs@gmail.com)
[![LinkedIn](https://img.shields.io/badge/in/linkedap-0D1117?style=flat-square&logo=linkedin&logoColor=0A66C2)](https://linkedin.com/in/linkedap)

</div>
