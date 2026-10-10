<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0e75b6,100:1b1f3b&height=180&section=header&text=Abhishek%20Barik&fontColor=ffffff&fontSize=46&fontAlignY=38&desc=Backend%20%26%20Systems%20Engineer&descAlignY=60&descSize=18" width="100%" alt="Abhishek Barik, Backend & Systems Engineer"/>

<a href="https://github.com/Tracebycode">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=500&size=18&duration=3200&pause=900&color=0E75B6&center=true&vCenter=true&width=640&lines=Distributed+systems+%26+event-driven+pipelines;Market-data+%26+trading+infrastructure;Kafka+%C2%B7+Redis+%C2%B7+PostgreSQL+%C2%B7+Kubernetes;Understand+the+system+before+the+abstraction" alt="Typing animation"/>
</a>

<br/>

<a href="https://linkedin.com/in/YOUR_LINKEDIN_USERNAME"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="mailto:YOUR_EMAIL@example.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
<a href="https://github.com/Tracebycode?tab=repositories"><img src="https://img.shields.io/badge/Repositories-181717?style=for-the-badge&logo=github&logoColor=white" alt="Repositories"/></a>

</div>

---

## 👋 About

Computer Engineering student who builds backend systems that stay correct under load and failure.

I work at the intersection of **event-driven architecture**, **data-intensive services**, and **market-data infrastructure**, and I like knowing *why* something works before I rely on the abstraction on top of it.

|  |  |
|---|---|
| 🔭 **Building** | A distributed job queue, a market-data and strategy engine, and a Kubernetes lab |
| 🌱 **Going deeper on** | Linux internals, networking, concurrency, C++ and CPU/cache behavior |
| 💬 **Ask me about** | Kafka, Redis-backed state, retries and dead-letter queues, look-ahead-free backtesting |

---

## 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

### ⚡ Distributed Job Queue & Worker Engine
Reliable async job processing built for failure.

- Retries with backoff and dead-letter queues
- Delayed jobs and failure recovery
- Concurrent workers, Redis-backed distributed state
- Durable job records in PostgreSQL

`Node.js` `TypeScript` `Redis` `PostgreSQL`

[**View repo →**](#) <!-- add link -->

</td>
<td width="50%" valign="top">

### 📈 Market Data & Trading Engine
Historical and real-time market-data processing.

- Historical candle ingestion
- Multi-timeframe candle generation
- Kafka event streaming, Redis live state
- Indicators and strategy execution with **zero look-ahead / repainting**

`Python` `Kafka` `Redis` `PostgreSQL`

[**View repo →**](#) <!-- add link -->

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ☸️ Kubernetes Infrastructure Lab
Production-style cloud-native setup.

- Containerized services and ingress/service networking
- GitLab CI/CD pipelines
- Centralized logging and observability
- Infrastructure automation with Terraform

`Kubernetes` `Linux` `GitLab CI/CD` `Terraform`

[**View repo →**](#) <!-- add link -->

</td>
<td width="50%" valign="top">

### 📞 Asterisk VoIP System
Real-time voice communication for low-bandwidth networks.

- Call handling on constrained links
- Containerized deployment

`Asterisk` `Linux` `Docker`

[**View repo →**](#) <!-- add link -->

</td>
</tr>
</table>

---

## 🧩 How the Market Data Engine Fits Together

```mermaid
flowchart LR
    A[Historical data] --> C[Candle ingestion]
    B[Live market feed] --> K[(Kafka)]
    C --> P[(PostgreSQL)]
    K --> T[Multi-timeframe<br/>candle builder]
    T --> R[(Redis<br/>live state)]
    T --> P
    R --> I[Indicators]
    I --> S[Strategy engine]
    S --> O[Signals / orders]
```

Strategies only ever see **closed** candles, so signals can't repaint or peek at future data.

---

## 🛠️ Tech Stack

<p align="center">
  <img src="https://skillicons.dev/icons?i=cpp,py,ts,js,nodejs,express&perline=6" alt="Languages and backend"/>
  <br/>
  <img src="https://skillicons.dev/icons?i=postgres,redis,kafka,mongodb&perline=4" alt="Data and messaging"/>
  <br/>
  <img src="https://skillicons.dev/icons?i=linux,kubernetes,docker,gitlab,terraform,aws&perline=6" alt="Infrastructure"/>
  <br/>
  <img src="https://skillicons.dev/icons?i=git,github,postman&perline=3" alt="Tools"/>
</p>

<details>
<summary><b>Full list</b></summary>

| | |
|---|---|
| **Languages** | C++ · Python · TypeScript · JavaScript |
| **Backend** | Node.js · Express · REST APIs |
| **Data & messaging** | PostgreSQL · Redis · Kafka · MongoDB |
| **Infra & DevOps** | Linux · Kubernetes · Podman · GitLab CI/CD · Terraform · AWS |
| **Tools** | Git · GitHub · Postman |

</details>

---

## 📚 Currently Learning

| Systems | Backend | Performance |
|---|---|---|
| Linux internals | Kafka | C++ |
| Networking | PostgreSQL internals | Memory management |
| Operating systems | Node.js internals | CPU / cache behavior |
| Concurrency | System design | Data structures & algorithms |

---

## 🎯 Engineering Philosophy

> **Understand the system before using the abstraction.**

<details>
<summary><b>Questions I keep coming back to</b></summary>

- What actually happens inside the runtime?
- Where does latency come from?
- What happens when a service fails halfway through a job?
- How do we guarantee correctness under concurrency?
- How can a system scale without becoming fragile?

</details>

---

## 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=Tracebycode&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" height="165" alt="GitHub stats"/>
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Tracebycode&layout=compact&theme=tokyonight&hide_border=true" height="165" alt="Top languages"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Tracebycode&theme=tokyonight&hide_border=true" height="165" alt="Contribution streak"/>

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:1b1f3b,100:0e75b6&height=90&section=footer" width="100%" alt=""/>
