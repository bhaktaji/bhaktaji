<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&color=7dd3fc&height=220&section=header&text=Aakash%20Bhakta&fontSize=42&fontColor=0b0f19&animation=twinkling&fontAlignY=38&desc=Senior%20Java%20Developer%20%7C%20Java%20Consultant%20%7C%20Backend%20Engineering%20Lead&descAlignY=58&descSize=18)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&duration=3000&pause=1000&color=7DD3FC&center=true&vCenter=true&width=640&lines=Java+%7C+Spring+Boot+%7C+REST+APIs;Leading+the+Engage+Backend+Team+%40+VMO2;IoT+%2B+Telecom+%2B+Insurance+%2B+Identity+Governance;Building+privacy-first+fintech+and+WhatsApp+SaaS+tools;Exploring+Generative+AI+%26+Automation)](https://git.io/typing-svg)

![Open to Work](https://img.shields.io/badge/Open%20to%20Work-7DD3FC?style=for-the-badge&logo=git&logoColor=0b0f19&labelColor=0b0f19)

![Profile Views](https://komarev.com/ghpvc/?username=bhaktaji&color=7dd3fc&style=flat-square&label=Profile+Views)
![Followers](https://img.shields.io/github/followers/bhaktaji?color=7dd3fc&style=flat-square&label=Followers)

</div>

## 🧭 Who I Am

I'm a backend engineer who ships production Java for a living and builds product ideas on the side. By day I lead the backend team on the **Engage** platform at **Virgin Media O2** (via TCS). After hours I turn real-world problems into working systems: a Java mall management and POS platform, a privacy-first debt diagnostic, a WhatsApp order-capture suite for distributors, a steganography tool, and more.

|                    |                                                                          |
|--------------------|--------------------------------------------------------------------------|
| 🎯 **Title**        | Senior Java Developer / Java Consultant / Backend Engineering Lead       |
| 📍 **Location**     | Kolkata, India                                                           |
| 💼 **Current Role** | Java Backend Lead @ Engage, Virgin Media O2 (via TCS)                    |
| ⏳ **Experience**   | 5+ years                                                                 |
| ⚡ **Status**       | Leading a team of 5 backend developers, shipping production Java systems |
| 🔍 **Open To**      | Java Consultant · Senior Java Developer · Java Backend Lead              |

### 📌 Impact at work

| 🚀 **10x+** | ⏱️ **18s → 5s** | 👥 **5 devs** |
|:-----------:|:---------------:|:-------------:|
| Faster bulk order loading on the Engage platform | Backend API response time on the Vodafone IoT platform | Backend team led: reviews, sprint planning, delivery |

---

## 🚀 Featured Projects

### 🏬 [Mall Management System](https://github.com/bhaktaji/mall-management-system)

> A Java backend platform for managing mall operations, and the foundation my POS application is built on.

- 🏗️ Spring Boot backend on MongoDB, structured so new modules can be added on top of it
- 🧾 The **POS Application** below is the first extension built on this platform

| Layer   | Technology        |
|---------|-------------------|
| Backend | Java · Spring Boot |
| Data    | MongoDB           |

---

### 🧾 [POS Application](https://github.com/bhaktaji/pos-system)

> Billing, invoicing, inventory and accounting for mall tenants, built as an extension of the Mall Management System.

- 📐 Design-first: HLD, LLD and ER diagrams written up front and aligned to the Mall Management System stack
- ✅ Backend (`pos-backend`) is complete and tested; the `pos-frontend` build and integration are in progress
- 🧩 Same stack as the parent platform, so it plugs in without introducing new infrastructure

| Layer    | Technology                                          |
|----------|-----------------------------------------------------|
| Backend  | Java · Spring Boot                                  |
| Data     | MongoDB                                             |
| Frontend | In progress (`pos-frontend`)                        |
| Status   | 🚧 Backend done and tested, frontend integration underway |

---

### 💸 [Debt Reality Checker](https://github.com/bhaktaji/debt-reality-check)

> A deterministic, offline-first household solvency diagnostic that explains itself in plain English.

Enter income, essential costs, cash buffer and debts. It normalises every interest rate to a true APR (a "24% flat" loan quote can turn out to be 40% APR), computes a four-tier cash-flow verdict, compares Avalanche vs Snowball payoff strategies, and returns 3–5 concrete next actions. **No LLM in the financial path**: every verdict comes from pure functions over thresholds you can read and test.

- 🧮 One shared `core/` engine powering three surfaces: **React dashboard**, **CLI** and **WhatsApp bot**
- 🔒 Privacy by design: zero-PII, HMAC-pseudonymised user IDs, data purged on inactivity, dashboard runs fully in `localStorage` with no network calls
- ✅ **397 tests across 21 files** (unit, property, golden-fixture, parity, boundary), with CI on GitHub Actions
- 💱 Money handled as integer paise internally, `en-IN` formatting for display

| Layer     | Technology                                                    |
|-----------|---------------------------------------------------------------|
| Runtime   | Node.js 22+                                                   |
| Dashboard | React 18 + Vite 6                                             |
| Storage   | SQLite (`better-sqlite3` with `node:sqlite` fallback)         |
| Messaging | WhatsApp Cloud API + Baileys adapter + console channel        |
| Quality   | Vitest, ESLint 9, GitHub Actions                              |

---

### 📦 [OrderBridge — Multi-Tenant WhatsApp Order Capture](https://github.com/bhaktaji/whatsapp-order-processing-system)

> Turns messy WhatsApp orders into structured draft orders and syncs them to accounting software.

Built for distributors, wholesalers and small food brands whose buyers send orders as Hinglish text or voice notes (*"Bhaiya 5 peti Parle-G, 2 katta Basmati 25kg bhej do"*). Buyers need no signup, and the owner stops re-typing orders into Excel or Tally every night.

- 🧠 Hybrid **fuzzy-SKU + LLM extraction** with unit multipliers (`peti`, `katta`, `crate`) and per-line confidence scores
- 🔗 Exporters for **Tally Prime (XML vouchers), Xero, Zoho Books, QuickBooks** and Excel/CSV
- 🛡️ **Ban-resilient by design**: 24h-window guardrails, rate-limit protection, and failover to standby WhatsApp numbers, Twilio SMS, Telegram and zero-signup micro-store links
- 🏷️ White-label tenants with isolated config for branding, currency, tax engine (GST / VAT / Sales Tax) and custom unit dictionaries

| Layer     | Technology                                                    |
|-----------|---------------------------------------------------------------|
| Backend   | Python 3.11 · FastAPI                                         |
| Data      | PostgreSQL (multi-tenant schema via Prisma)                   |
| Frontend  | Single-file admin workbench and white-label studio (HTML)     |
| Infra     | Docker Compose                                                |

---

### 🔐 [HiddenText](https://github.com/bhaktaji/HiddenText)

Steganography project: hide information inside PNG images using custom encryption.

🔗 **Domain:** Cryptography · Steganography · Secure data hiding

### 🤖 [Building and Selling AI Agents — A Practical Guide](https://github.com/bhaktaji/Building-and-Selling-AI-Agents-A-Practical-Guide)

A practical guide to designing, building and monetizing AI agents.

🔗 **Domain:** Generative AI · Agent architecture · Productization

### 🍛 [The Biryani Project](https://github.com/bhaktaji/The-Biryani-Project)

A biryani shop Android app built for fun: menu, cart and order tracking with offline storage.

🔗 **Stack:** Kotlin · Jetpack Compose (Material 3) · MVVM · Room · Hilt · Coroutines & Flow

---

## 🛠️ Currently Building

| Project | What it is | Stack |
|---------|-----------|-------|
| **Carbon Co-Pilot** | Early-stage multi-cloud carbon and FinOps dashboard: tracks spend and emissions across AWS, Azure and GCP with AI-driven workload migration suggestions. | [Live prototype](https://lovable.dev/products/eco-pilot-spark) |

---

## 🔗 How My Day Job Shapes My Side Projects

| At work | In my side projects |
|---------|---------------------|
| Identity governance and PGP encryption (SailPoint IdentityIQ) | Privacy-by-design in Debt Reality Checker: pseudonymised IDs, zero-PII, data minimisation |
| Enterprise integrations (SailPoint connectors, Aetna/CVS insurance modules) | OrderBridge's ERP connectors: Tally, Xero, Zoho Books, QuickBooks |
| Production reliability (Jenkins pipelines, async + batching + caching at scale) | Test-first builds, CI, and failover-first design |

---

## 💼 Professional Experience

### 🏢 Tata Consultancy Services (TCS) · Sep 2023 – Present

<details open>
<summary><b>Java Backend Lead — Engage, Virgin Media O2 (VMO2)</b> · <i>Feb 2025 – Present</i></summary>
<br>

- Own backend architecture, technical design and delivery for the Engage platform
- Lead a team of 5 Java developers: code reviews, sprint planning, task breakdown
- Designed an optimized solution (parallel processing, async scheduling, batching, caching, query optimization) that improved bulk order loading performance **10x+**
- Standardized Jenkins deployment pipelines, improving release reliability across prod/QA/dev
- Evaluated AI-driven automation opportunities across the platform with architects and leadership

</details>

<details>
<summary><b>Java Consultant — User Access Management (SailPoint IdentityIQ)</b> · <i>Nov 2024 – Feb 2025</i></summary>
<br>

- Delivered Identity Governance & Administration (IGA) solutions on SailPoint IdentityIQ
- Built secure Java REST integrations between SailPoint and enterprise apps via Web Service Connectors
- Built a Java PoC for PGP encryption/decryption of sensitive client files, automating onboarding workflows

</details>

<details>
<summary><b>Senior Java Developer — Vodafone IoT Platform</b> · <i>Sep 2023 – Nov 2024</i></summary>
<br>

- Designed scalable Spring Boot microservices for IoT device management and telemetry
- Built REST APIs on MongoDB handling high-volume, low-latency IoT transactions
- Cut backend API response times from **18s → 5s** via indexing, aggregation, async processing and AWS scaling

</details>

### 🏢 Infosys Limited · Jul 2021 – Jun 2023

<details>
<summary><b>System Engineer, Application Development — Aetna / CVS Health Insurance Platform</b></summary>
<br>

- Worked across Majesco L&A, ICD and ICM modules for enterprise insurance applications
- Built Java backend components integrated with frontend applications
- Used Cassandra and MySQL for large-scale data persistence
- Integrated Apache Spark for large-scale real-time data processing
- Optimized SQL through Java transformers, speeding up large data copy jobs to Cassandra

</details>

---

## 🛠️ Tech Stack

**Languages**

![Languages](https://skillicons.dev/icons?i=java,python,js,kotlin)

**Backend & Frameworks**

![Backend](https://skillicons.dev/icons?i=spring,hibernate,tomcat,fastapi,nodejs,react,vite)

**Databases**

![Databases](https://skillicons.dev/icons?i=mongodb,cassandra,mysql,postgres,sqlite)

**Cloud & DevOps**

![DevOps](https://skillicons.dev/icons?i=aws,docker,jenkins,gitlab,githubactions,sonarqube)

**Dev Tools**

![Tools](https://skillicons.dev/icons?i=eclipse,idea,androidstudio,postman,git,linux,vscode)

---

## 🎓 Certifications

| Certification | Year |
|---------------|:----:|
| React JS Intermediate | 2025 |
| Gen AI E1 | 2024 |
| Software Security Assurance | 2024 |
| Certified Ethical Hacker | 2017 |

---

## 📊 GitHub Stats

<div align="center">

![Aakash's GitHub Stats](https://github-readme-stats.vercel.app/api?username=bhaktaji&show_icons=true&theme=nord&border_color=7dd3fc&title_color=7dd3fc&icon_color=7dd3fc&text_color=c9d1d9&bg_color=0d1117&cache_seconds=86400)
![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=bhaktaji&layout=compact&theme=nord&border_color=7dd3fc&title_color=7dd3fc&text_color=c9d1d9&bg_color=0d1117&cache_seconds=86400)

![GitHub Streak](https://streak-stats.demolab.com/?user=bhaktaji&theme=nord&border=7dd3fc&ring=7dd3fc&fire=7dd3fc&currStreakLabel=7dd3fc&background=0d1117)

![GitHub Trophies](https://trophygithubreadmelang.cybee.dpdns.org/?username=bhaktaji&theme=nord&border_color=7dd3fc&title_color=7dd3fc&text_color=c9d1d9&bg_color=0d1117&cache_seconds=86400)

</div>

## 🤝 Connect With Me

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/aakash-bhakta/)
[![Twitter/X](https://img.shields.io/badge/Twitter-000000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/bhaktaji_)
[![Email](https://img.shields.io/badge/Email-7DD3FC?style=for-the-badge&logo=gmail&logoColor=0b0f19)](mailto:YOUR_EMAIL@example.com)

![footer](https://capsule-render.vercel.app/api?type=waving&color=7dd3fc&height=150&section=footer&animation=twinkling)

</div>
