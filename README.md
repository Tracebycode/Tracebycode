<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=220&section=header&text=Abhishek%20Barik&fontSize=48&fontColor=ffffff&fontAlignY=35&desc=Backend%20%7C%20Distributed%20Systems%20%7C%20Infrastructure&descSize=20&descAlignY=55&descAlign=50" width="100%" />

<br/>

<a href="https://www.linkedin.com/in/abhishek-barik-735a911b1/">
<img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/>
</a>
<a href="mailto:abhishekbarik974@gmail.com">
<img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white"/>
</a>
<a href="https://github.com/Tracebycode">
<img src="https://img.shields.io/badge/GitHub-111111?style=for-the-badge&logo=github&logoColor=white"/>
</a>

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=Tracebycode&label=PROFILE%20VIEWS&color=2c5364&style=for-the-badge"/>

</div>

---

<div align="center">

### `Backend Engineering` • `Distributed Systems` • `Infrastructure` • `High Performance`

**Building systems that are reliable, observable, event-driven and performance conscious.**

</div>

---

## 🧑‍💻 `whoami`

```text
Abhishek Barik
├── Computer Engineering @ D.Y. Patil Technical Campus
├── Backend / Systems Engineering
├── Distributed & Event-Driven Systems
├── Infrastructure & Cloud-Native Engineering
└── Exploring High-Performance & Trading Systems
```

I'm a **Computer Engineering student graduating in 2027**, focused on backend and systems engineering.

My current work sits around the intersection of:

```text
        BACKEND
           │
           ▼
   DISTRIBUTED SYSTEMS
           │
     ┌─────┴─────┐
     ▼           ▼
 INFRASTRUCTURE  DATA SYSTEMS
     │           │
     └─────┬─────┘
           ▼
    HIGH PERFORMANCE
```

I enjoy understanding what happens **below the abstraction** — concurrency, memory, networking, queues, databases, processes, containers and distributed state.

---

## ⚡ Current Engineering Focus

<table>
<tr>
<td width="50%" valign="top">

### 📈 Trading Infrastructure

Building backend infrastructure around **market data and automated trading systems**.

- Historical market-data pipelines
- Multi-timeframe candle generation
- Kafka event streaming
- Redis live state
- Indicator computation
- Strategy execution
- PostgreSQL data storage
- Zero look-ahead / repainting prevention

`Python` `Kafka` `PostgreSQL` `Redis`

</td>

<td width="50%" valign="top">

### ⚙️ Distributed Job Systems

Building a **distributed job queue and worker execution engine**.

- Job scheduling
- Worker execution
- Retry & recovery
- Dead-letter queues
- Delayed jobs
- Concurrency
- Failure handling
- Distributed state

`Node.js` `TypeScript` `Redis`

</td>
</tr>

<tr>
<td width="50%" valign="top">

### ☸️ Infrastructure

Working with production-style deployment infrastructure.

- Kubernetes
- Containerized services
- GitLab CI/CD
- Ingress
- Linux
- Terraform
- Observability
- Centralized logging

`Kubernetes` `Linux` `GitLab` `Terraform`

</td>

<td width="50%" valign="top">

### 🧠 Systems & Performance

Deepening fundamentals that sit underneath backend systems.

- C++
- Data Structures & Algorithms
- Operating Systems
- Linux internals
- Networking
- Concurrency
- Computer architecture
- Performance engineering

</td>
</tr>
</table>

---

# 🏗️ Engineering Projects

<div align="center">

<a href="https://github.com/Tracebycode/Job-queue-distribution-system">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=Tracebycode&repo=Job-queue-distribution-system&theme=tokyonight&hide_border=true" width="48%"/>
</a>

<a href="https://github.com/Tracebycode/stockmarket-Backtesting-Engine">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=Tracebycode&repo=stockmarket-Backtesting-Engine&theme=tokyonight&hide_border=true" width="48%"/>
</a>

<br/>

<a href="https://github.com/Tracebycode/Asha-Ehr-Backend-">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=Tracebycode&repo=Asha-Ehr-Backend-&theme=tokyonight&hide_border=true" width="48%"/>
</a>

<a href="https://github.com/Tracebycode/Task-Management-Navicon-Infraprojects-">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=Tracebycode&repo=Task-Management-Navicon-Infraprojects-&theme=tokyonight&hide_border=true" width="48%"/>
</a>

</div>

---

## 🔬 Systems I've Worked On

### 01 — Distributed Job Queue

```text
                    ┌──────────────┐
                    │    Client    │
                    └──────┬───────┘
                           │
                           ▼
                    ┌──────────────┐
                    │  Job Queue   │
                    └──────┬───────┘
                           │
              ┌────────────┼────────────┐
              ▼            ▼            ▼
          Worker 1     Worker 2     Worker N
              │            │            │
              └────────────┼────────────┘
                           ▼
                    ┌──────────────┐
                    │  Completed   │
                    │ / Retry / DLQ│
                    └──────────────┘
```

Focus:

`Concurrency` `Retries` `Failure Recovery` `DLQ` `Workers` `Redis`

---

### 02 — Market Data Pipeline

```text
       Market Data
            │
            ▼
    ┌───────────────┐
    │   Ingestion   │
    └───────┬───────┘
            │
            ▼
        ┌───────┐
        │ Kafka │
        └───┬───┘
            │
     ┌──────┴──────┐
     ▼             ▼
  Candle        Indicator
  Engine          Engine
     │             │
     └──────┬──────┘
            ▼
       Strategy Engine
            │
            ▼
      Signal Generation
```

Focus:

`Event-Driven Architecture` `Kafka` `Redis` `PostgreSQL` `Indicators` `Trading`

---

# 🧰 Technology Radar

<div align="center">

<img src="https://skillicons.dev/icons?i=cpp,python,typescript,javascript,nodejs,express,postgres,redis&perline=8&theme=dark"/>

<br/><br/>

<img src="https://skillicons.dev/icons?i=kafka,docker,kubernetes,linux,git,gitlab,githubactions,terraform&perline=8&theme=dark"/>

<br/><br/>

<img src="https://skillicons.dev/icons?i=aws,prometheus,grafana,mongodb,react,nextjs,postman&perline=8&theme=dark"/>

</div>

---

# 🧠 What I'm Learning

<table>
<tr>
<td>

### Systems

- Linux Internals
- Operating Systems
- Networking
- Computer Architecture
- Concurrency
- Memory & Processes

</td>

<td>

### Distributed Systems

- Kafka
- Redis
- Message Queues
- Fault Tolerance
- Event-Driven Architecture
- Distributed State

</td>

<td>

### Performance

- C++
- DSA
- Algorithms
- CPU & Cache Behavior
- Low-Level Optimization
- High-Performance Systems

</td>
</tr>
</table>

---

# ☁️ Infrastructure

```text
Developer
   │
   ▼
Git
   │
   ▼
GitLab CI/CD
   │
   ├──────────────► Test
   │
   ├──────────────► Build
   │
   └──────────────► Deploy
                         │
                         ▼
                    Kubernetes
                         │
              ┌──────────┼──────────┐
              ▼          ▼          ▼
           Backend     Jobs      Services
              │          │          │
              └──────────┼──────────┘
                         ▼
                 Observability
                         │
                    ┌────┴────┐
                    ▼         ▼
                   Loki     Grafana
```

Currently working with:

`Kubernetes` `GitLab CI/CD` `Linux` `Terraform` `Podman` `AWS`

---

# 📊 GitHub Activity

<div align="center">

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Tracebycode&theme=tokyo-night&hide_border=true&area=true&custom_title=Contribution%20Activity" width="100%"/>

<br/><br/>

<img src="https://github-readme-stats.vercel.app/api?username=Tracebycode&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&rank_icon=github" height="170"/>

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Tracebycode&layout=compact&theme=tokyonight&hide_border=true" height="170"/>

<br/><br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Tracebycode&theme=tokyonight&hide_border=true" height="170"/>

</div>

---

# 🏆 GitHub Trophies

<div align="center">

<img src="https://github-profile-trophy.vercel.app/?username=Tracebycode&theme=tokyonight&no-frame=true&no-bg=true&margin-w=5&column=7" width="100%"/>

</div>

---

# 📊 Engineering Metrics

<div align="center">

<img src="./github-metrics.svg" width="98%" alt="GitHub Engineering Metrics"/>

</div>

---

# 🧭 Engineering Philosophy

<div align="center">

### `Understand the system before using the abstraction.`

</div>

I like asking questions such as:

```text
What actually happens inside the runtime?
        ↓
Where does the data go?
        ↓
Where is state stored?
        ↓
What happens when something fails?
        ↓
What happens under concurrency?
        ↓
Where does the latency come from?
        ↓
How does the system behave at scale?
```

For me, engineering isn't just about making something work.

It's about understanding **why it works, how it fails, and how it behaves under pressure.**

---

# 🎯 Long-Term Direction

```text
             Backend Engineering
                     │
                     ▼
             Distributed Systems
                     │
             ┌───────┴───────┐
             ▼               ▼
       Infrastructure    Data Systems
             │               │
             └───────┬───────┘
                     ▼
             Systems Engineering
                     │
                     ▼
          High-Performance Systems
                     │
                     ▼
            Trading Infrastructure
```

---

<div align="center">

## Let's Build Systems.

<a href="https://github.com/Tracebycode">
<img src="https://img.shields.io/badge/GitHub-Explore%20My%20Work-181717?style=for-the-badge&logo=github"/>
</a>

<a href="https://www.linkedin.com/in/abhishek-barik-735a911b1/">
<img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin"/>
</a>

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f2027,50:203a43,100:2c5364&height=110&section=footer" width="100%"/>

</div>
