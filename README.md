<div align="center">

# Ayush Pandey

### AI Full-Stack Engineer • SaaS Builder • Performance-Cost Optimizer

*Designing AI-powered efficient cloud solutions that scale massively while spending minimally*

[![Portfolio](https://img.shields.io/badge/🌐_Portfolio-ayushpandey.me-00D9FF?style=for-the-badge)](https://ayushpandey.me)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=for-the-badge&logo=linkedin)](https://linkedin.com/in/linkedap)
[![Email](https://img.shields.io/badge/Email-Collaborate-D14836?style=for-the-badge&logo=gmail)](mailto:ayushpandey.cs@gmail.com)

</div>

---

## 💡 Philosophy

> **Execution is the currency that converts ideas into value.**

<table>
<tr>
<td width="25%" align="center">
<img src="https://img.shields.io/badge/🏆_2nd_Place-Google_DSC_IIT_KANPUR_Hackathon-4285F4?style=flat-square" alt="Achievement"/>
<br/><sub>Led team to 2nd position out of 800 teams</sub>
</td>
<td width="25%" align="center">
<img src="https://img.shields.io/badge/🎯_Solo_Founder-versionCV-00D9FF?style=flat-square" alt="Founder"/>
<br/><sub>Full SDLC ownership: Idea → Production in 8 months</sub>
</td>
<td width="25%" align="center">
<img src="https://img.shields.io/badge/💰_Cost_Optimization-versionCV-4CAF50?style=flat-square" alt="Cost"/>
<br/><sub>$250/month → ~$0 idle • ~100% savings</sub>
</td>
<td width="25%" align="center">
<img src="https://img.shields.io/badge/⚡_Performance-4K+_req/sec-FF6B6B?style=flat-square" alt="Performance"/>
<br/><sub>High-performance, low latency api</sub>
</td>
</tr>
</table>

---

## 🌍 Open Source Impact

### 🐝 **Hive AI Agent Framework** 
<sup>Production framework by **AdenHQ** • ![Y Combinator](https://img.shields.io/badge/YC-Backed-FF6600?style=flat-square&logo=ycombinator)</sup>
```diff
+ Fixed critical Windows UnicodeEncodeError → Restored cross-platform stability
+ Debugged broken CI/CD pipeline → Unblocked core team deployment
+ Resolved merge conflicts → Improved codebase quality
```

**Impact:** Enhanced reliability for production AI agents  
**Collaboration:** Direct work with CTO & engineering team  
🔗 [View PR #641](https://github.com/adenhq/hive/pull/641)

---

## 🎯 Featured Projects

<div align="center">

### 🎯 **versionCV** – AI Resume Optimization Platform
**[Live Platform ↗](https://www.versioncv.com)** • *MSME Registered (Govt of India)* • **May 2025 – Present**

![Status](https://img.shields.io/badge/Status-Beta_Launched-00D9FF?style=for-the-badge)
![Users](https://img.shields.io/badge/Idle_Infrastructure_Cost-~$0-4CAF50?style=for-the-badge)

</div>

#### The Vision

Transforming professional resume management with AI-powered optimization, version control, and ATS intelligence.

#### Core Features Matrix

<table>
<tr>
<td width="50%">

**AI Resume Agent**
- Multi-model fallback (Gemini→GPT→Claude→Mistral)
- <30s full resume rewrites
- Hallucination control via xml prompting and deterministic context binding.
- Token optimization for cost efficiency
- Preserves links & original data accuracy

</td>
<td width="50%">

**ATS Analyzer**
- Real-time scoring & feedback
- Keyword optimization
- Format compatibility checking
- Layout complexity detection
- Missing section identification

</td>
</tr>
<tr>
<td width="50%">

**Custom WYSIWYG Editor**
- Zero-dependency WYSIWYG
- React-powered
- Integrated ATS scanner
- Real-time formatting

</td>
<td width="50%">

**Smart Management**
- Role-based versioning
- CDN-accessible links
- Clone & edit workflows
- Analytics tracking per resume/role/vault

</td>
</tr>
</table>

#### Infrastructure Architecture
```
┌──────────────────────────────────────────────────────────────────┐
│  EDGE LAYER (Cloudflare)                                         │
├──────────────────────────────────────────────────────────────────┤
│  Workers (Serverless Functions)                                  │
│  ├─ KV Cache ( real-time invalidation)                           │
│  ├─ D1 Database (SQLite with fallback protection)                │
│  ├─ R2 Storage (Versioned resumes, CDN delivery)                 │
│  ├─ Queue (Background processing)                                │
│  ├─ Durable Objects (Stateful coordination)                      │
│  └─ CDN (Global distribution)                                    │
├──────────────────────────────────────────────────────────────────┤
│  COMPUTE LAYER                                                   │
├──────────────────────────────────────────────────────────────────┤
│  Google Cloud Run (Containerized API)                            │
│  Vercel Edge (Next.js 14 Frontend)                               │
├──────────────────────────────────────────────────────────────────┤
│  SECURITY LAYER (Multi-layered)                                  │
├──────────────────────────────────────────────────────────────────┤
│  ✓ Firebase JWT (1ms claim verification on every request)        │
│  ✓ Email verification                                            │
│  ✓ Zero client trust model                                       │
│  ✓ Internal API isolation (no DNS, RPC-only access)              │
│  ✓ API interlocking via isolated secrets                         │
│  ✓ 4-layer rate limiting with fallback                           │
│  ✓ Strict CSP Headers                                            │
│  ✓ Multi-layer DDoS mitigation (Cloudflare + internal)           │
└──────────────────────────────────────────────────────────────────┘
```

#### 📈 Performance Metrics

<div align="center">

| Metric | Achievement |
|--------|-------------|
| **⚡ Latency** | `<100ms` average |
| **🚀 Capacity** | `4K+ req/sec` capable |
| **⏱️ Uptime** | `99.9%` |
| **🔒 Auth Speed** | `1ms` Full JWT verification |
| **💰Idle Infrastructure Cost** | `~$0` |

</div>

#### Security Architecture
```
Request Flow with Security Layers:

User Request
    ↓
┌─────────────────────────────────────┐
│ Layer 1: CSP Headers Check          │
└─────────────────────────────────────┘
   ↓
┌─────────────────────────────────────┐
│ Layer 2: Cloudflare DDoS Protection │
└─────────────────────────────────────┘
    ↓
┌─────────────────────────────────────┐
│ Layer 3: Bot Verification           │
└─────────────────────────────────────┘
    ↓
┌─────────────────────────────────────┐
│ Layer 4: Rate Limiter (4 fallbacks) │
│  ├─ User: 2 req/s                   │
│  └─ IP: 10 req/s                    │
└─────────────────────────────────────┘
    ↓
┌─────────────────────────────────────┐
│ Layer 5: Firebase JWT Validation    │
│  └─ 1ms full claim verification     │
└─────────────────────────────────────┘
    ↓
┌─────────────────────────────────────┐
│ Layer 6: API Interlocking           │
│  └─ Isolated secrets per service    │
└─────────────────────────────────────┘
    ↓
Internal Services (No DNS exposure)
```

<details>
<summary><b> Data Strategy Details</b></summary>

**Primary Database**: Cloudflare D1 (SQLite)
- Batch-based updates preventing race conditions
- Fallback protection for reliability

**Caching Layer**: KV Cache
- Real-time invalidation
- Cloudflare CDN integration

**Storage**: Cloudflare R2
- CDN-accessible resume links
- Version control built-in
- Instant global distribution

</details>

<div align="center">

### 🔒 **SwiftVault** – Enterprise File Vault
**[Live Demo ↗](https://swiftvault-ayushs-projects-0e2cdca4.vercel.app/)** • *8-day sprint: 6 days MVP → 2 days serverless transformation*

</div>

#### The Transformation
<div align="center">
<table border="1" cellpadding="8" cellspacing="0" width="100%">
  <tr>
    <th width="50%">Before: Monolithic</th>
    <th width="50%">After: Edge-Native Serverless</th>
  </tr>

  <tr>
    <td>Cost: $17/month</td>
    <td>Cost: $0/month (Year 1)</td>
  </tr>

  <tr>
    <td>Latency: Regional delays</td>
    <td>Latency: &lt;50ms globally</td>
  </tr>

  <tr>
    <td>Deployment: Single EC2 instance</td>
    <td>Deployment: Edge distribution</td>
  </tr>

  <tr>
    <td>Scaling: Manual intervention</td>
    <td>Scaling: Zero-cost automatic</td>
  </tr>

  <tr>
    <td>Idle costs: Always paying</td>
    <td>Idle costs: None</td>
  </tr>
</table>

</div>

#### Impact Metrics

<div align="center">

| Metric | Result | 
|--------|--------|
| **💰 Cost Reduction** | `$204/year → $0` **(100% Year 1)** → `$108/year` **(47% permanent)** |
| **⚡ Metadata Queries** | `<100ms` |
| **📤 Upload Speed** | `<500ms` with edge caching |
| **💾 Storage Savings** | `30-40%` via SHA-256 deduplication ||
| **🌐 Global Latency** | `<100ms` response times |

</div>

#### Architecture Evolution
```
┌─────────────────────────────────────────────────────────────┐
│  BEFORE: Monolithic Stack                                   │
├─────────────────────────────────────────────────────────────┤
│  AWS EC2 (t2.micro) → PostgreSQL → Redis → MinIO            │
│  Nginx → Go Backend → JWT Auth                              │
└─────────────────────────────────────────────────────────────┘

                         ⬇️ TRANSFORMATION ⬇️

┌─────────────────────────────────────────────────────────────┐
│  AFTER: Distributed Serverless                              │
├─────────────────────────────────────────────────────────────┤
│  Cloudflare Workers (Edge Functions)                        │
│  ├─ KV Cache (Redis replacement)                            │
│  ├─ R2 Storage (MinIO replacement)                          │
│  └─ Rate Limiting (2 req/s user, 10 req/s IP)               │
│                                                             │
│  Neon PostgreSQL (Serverless)                               │
│  Vercel Edge (Next.js 14 Frontend)                          │
└─────────────────────────────────────────────────────────────┘
```

#### Technical Highlights

- 🔐 **Security**: RS256 JWT • bcrypt hashing • MIME validation • Zero-trust architecture
- 🧠 **Smart Deduplication**: SHA-256 hash-based duplicate detection
- ⚡ **Real-time**: Async uploads with live progress tracking
- 🎯 **Advanced Search**: Multi-criteria filtering with tag support
- 🔗 **Flexible Sharing**: Private + public link sharing with analytics
- 📊 **Admin Dashboard**: Comprehensive system monitoring

<details>
<summary><b>🔧 Tech Stack Deep Dive</b></summary>

**Backend**: Go • GraphQL • PostgreSQL • Redis • MinIO  
**Frontend**: Next.js 14 • TypeScript • Tailwind CSS  
**Cloud**: AWS • Vercel • Cloudflare (Workers/KV/R2) • Neon  
**DevOps**: Docker • Nginx • SSL/TLS • GitHub Actions  

</details>

---

## Additional Projects

<table>
<tr>
<td width="50%">

### 🔌 **Atithidev DB API**
*Serverless REST API*

**Impact**: Scalable hospitality data layer  
**Stack**: AWS Lambda • DynamoDB  
🔗 [Live API](https://kzjttnxnf3.execute-api.ap-south-1.amazonaws.com/dev/)

</td>
<td width="50%">

### 🧠 **Sentiment Analyzer**
*NLP microservice*

**Impact**: Real-time sentiment analysis  
**Stack**: Python • AWS Lambda • NLTK  
🔗 [Live API](https://6z8qsa4i2i.execute-api.ap-south-1.amazonaws.com/dev/)

</td>
</tr>
</table>

---

## 🛠️ Tech Arsenal

<details open>
<summary><b>💻 Languages</b></summary>

![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=flat-square&logo=typescript&logoColor=white)
![Go](https://img.shields.io/badge/Go-00ADD8?style=flat-square&logo=go&logoColor=white)

</details>

<details>
<summary><b>🌐 Web & Frameworks</b></summary>

![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat-square&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![Fastify](https://img.shields.io/badge/Fastify-000000?style=flat-square&logo=fastify&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?style=flat-square&logo=graphql&logoColor=white)
![Tailwind](https://img.shields.io/badge/Tailwind-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)

</details>

<details>
<summary><b>☁️ Cloud Platforms</b></summary>

![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel&logoColor=white)

</details>

<details>
<summary><b>🧪 Testing & Quality</b></summary>

![Jest](https://img.shields.io/badge/Jest-C21325?style=flat-square&logo=jest&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-FF6C37?style=flat-square&logo=postman&logoColor=white)
![ESLint](https://img.shields.io/badge/ESLint-4B3263?style=flat-square&logo=eslint&logoColor=white)

</details>

<details>
<summary><b>🔧 DevOps & Tools</b></summary>

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)

</details>

<details>
<summary><b>💾 Databases & Storage</b></summary>

![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-003B57?style=flat-square&logo=sqlite&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72E49?style=flat-square&logo=minio&logoColor=white)

</details>

---

## 📊 GitHub Activity

<div align="center">

![GitHub Streak](https://nirzak-streak-stats.vercel.app/?user=ap-dev-github&theme=dark&hide_border=true&background=0D1117&ring=00D9FF&fire=FF6B6B&currStreakLabel=00D9FF)


</div>

---

## 🤝 Let's Build Together

I'm actively seeking collaboration on:

<table>
<tr>
<td width="50%" align="center">

### 🏗️ **Distributed Systems**
Complex architectures at scale

</td>
<td width="50%" align="center">

### 💰 **Cost Optimization**
Cloud automation & efficiency

</td>
</tr>
<tr>
<td width="50%" align="center">

### ⚡ **High-Performance APIs**
Sub-100ms response times

</td>
<td width="50%" align="center">

### 🔐 **Security-First Design**
Zero-trust architectures

</td>
</tr>
</table>

<div align="center">

### 📬 Get In Touch

[![Email](https://img.shields.io/badge/Email-ayushpandey.cs@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:ayushpandey.cs@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-in/linkedap-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/linkedap)


</div>
