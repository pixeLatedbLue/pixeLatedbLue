<!-- Header -->
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Naval%20Agarwal&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32&desc=CSE%20(AI%2FML)%20%E2%80%A2%20Autonomous%20Systems%20%E2%80%A2%20ML%20%26%20Systems%20Engineer&descAlignY=54&descSize=16" width="100%"/>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=15&duration=3000&pause=800&color=E63946&center=true&vCenter=true&width=620&lines=Building+systems+that+make+decisions+%E2%80%94+not+just+interfaces.;Autonomous+Software+%40+Team+Ojas+Racing+%7C+Formula+Student+EV;ROS2+%C2%B7+ML+%C2%B7+C%2B%2B+%C2%B7+Embedded+Systems+%C2%B7+XAI" alt="Typing SVG" />

<br/>

<img src="https://img.shields.io/badge/VIT%20Vellore-CSE%20AI%2FML-E63946?style=for-the-badge&labelColor=0D0D0D" />
&nbsp;
<img src="https://img.shields.io/badge/Team%20Ojas%20Racing-Formula%20Student%20EV-FF9F1C?style=for-the-badge&labelColor=0D0D0D" />
&nbsp;
<img src="https://img.shields.io/badge/Mumbai-India-5BC0BE?style=for-the-badge&labelColor=0D0D0D" />

<br/><br/>

<img src="https://img.shields.io/badge/IEEE-VIT%20Member-888?style=flat-square&labelColor=0D0D0D" />
&nbsp;
<img src="https://img.shields.io/badge/CodeChef-Gold%20Badge-FFD700?style=flat-square&logo=codechef&labelColor=0D0D0D" />
&nbsp;
<img src="https://img.shields.io/badge/Building-In%20Public-E63946?style=flat-square&labelColor=0D0D0D" />

</div>

---

## `> about_me`

I build systems that **make decisions** — not just interfaces.

Second-year CSE (AI & ML) student at VIT Vellore, developing real-time autonomous vehicle software at **Team Ojas Racing** (Formula Student EV). My work sits at the intersection of perception pipelines, explainable ML, and low-level C++ — where software has to be *correct*, not just functional.

```
Focus Areas
├── Autonomous Systems & Robotics      (ROS2 Jazzy, sensor fusion, perception)
├── Machine Learning & Explainable AI  (Isolation Forest, SHAP, behavioral modeling)
├── System-Level C++ Engineering       (real-time decision engines, optimization)
└── Embedded Systems                   (Jetson Orin Nano, Arduino, RealSense, SBG IMU)
```

---

## `> autonomous_engineering`

<div align="center">

### 🏎️ Team Ojas Racing — Formula Student EV

**Autonomous Software Developer & Operations Team Member (CR)**

</div>

Building the software stack that makes the car think — and the team that makes it run:

| Domain | Responsibility |
|:---|:---|
| 🧠 Architecture | ROS2 Jazzy modular autonomous system design |
| 👁️ Perception | Sensor fusion — Intel RealSense stereo depth + SBG Ellipse IMU |
| ⚡ Decision | Real-time autonomous planning & control systems |
| 💻 Compute | Nvidia Jetson Orin Nano — edge AI inference & onboard processing |
| 🔒 Reliability | Safety-critical environment engineering |
| 📋 Operations | Team coordination, race logistics & cross-role ops (CR) |

**Hardware stack in use:**

```
Intel RealSense D435i  ──┐
                          ├──▶  ROS2 Jazzy (perception nodes)  ──▶  Decision Stack
SBG Ellipse N IMU      ──┘                                              │
                                                                         ▼
                                                            Nvidia Jetson Orin Nano
                                                            (onboard edge compute)
```

---

## `> selected_projects`

<details>
<summary><b>🔐 Insider Threat Dashboard &nbsp;—&nbsp; Internal Data Leak Risk Detector</b> &nbsp;<code>Python · Streamlit · ML · XAI</code></summary>

<br/>

> *A full-stack ML surveillance system for detecting insider threats before they happen*

A production-grade **Streamlit dashboard + simulation suite** for insider-risk monitoring. Ingests daily user activity (USB interactions, email metadata, psychometric profiles) and flags anomalous behavior with explainable AI insights.

**Core ML Pipeline:**
- **Isolation Forest** trained monthly on cumulative user activity features
- **SHAP TreeExplainer** provides per-user, per-feature risk attribution
- Dynamic + hard-limit policy checks (USB insertions, sensitive file ratios, external email ratios)
- Severity classification: `Critical → High → Elevated → Normal` via threshold quantiles

**Data Model:**
- Email signals: `total_emails`, `external_emails`, `attachments_sent`, `bcc_in_email`, `avg_email_size`
- USB signals: `usb_insertions`, `files_accessed`, `sensitive_files_accessed`
- **Big Five psychometrics** (`O`, `C`, `E`, `A`, `N`) — with `C` and `A` inverted for risk alignment

**System Architecture:**
```
Daily CSV ingestion → Cumulative aggregation → Anomaly scoring
       ↓                       ↓                      ↓
 Simulation engine    Monthly retraining         SHAP logging
       ↓                       ↓                      ↓
  Streamlit dashboard ← Flagged users + risk explanations
```

**Advanced Features:**
- Synthetic multi-month data generation (`full_generator.py`)
- CLI orchestration engine for automated month-cycling & retraining
- Web3 integration blueprint — wallet-auth, on-chain threshold governance, IPFS alert anchoring

[![Repo](https://img.shields.io/badge/View%20Repo-Internal--Data--Leak--Risk--Detector-E63946?style=flat-square&logo=github&labelColor=0D0D0D)](https://github.com/pixeLatedbLue/Internal-Data-Leak-Risk-Detector)

</details>

---

<details>
<summary><b>🤖 Scrape-Krunch &nbsp;—&nbsp; Real-Time News Intelligence Pipeline</b> &nbsp;<code>Python · Ollama · LLM</code></summary>

<br/>

> *Multi-domain news scraper feeding a local LLM for contextual analysis*

End-to-end pipeline that turns raw web noise into structured intelligence:
- Scrapes multi-domain news sources in real time
- Feeds structured, normalized data into a locally hosted LLM via **Ollama**
- Delivers contextual summarization, cross-domain correlation, and on-demand analysis
- Fully offline-capable — no external API dependencies

[![Repo](https://img.shields.io/badge/View%20Repo-Scrape--Krunch-E63946?style=flat-square&logo=github&labelColor=0D0D0D)](https://github.com/pixeLatedbLue/Scrape-Krunch)

</details>

---

<details>
<summary><b>💰 Adaptive Loan Repayment Scheduler</b> &nbsp;<code>C++ · Optimization · Decision Systems</code></summary>

<br/>

> *Dynamic priority-based financial decision engine*

A C++ system that acts as an automated financial advisor, reasoning over multiple loans simultaneously:
- Multi-factor decision logic: interest rate, remaining tenure, outstanding balance
- Dynamic repayment priority recomputed at each cycle
- Outputs the globally optimal repayment sequence under budget constraints

[![Repo](https://img.shields.io/badge/View%20Repo-Adaptive--Loan--Payment--Scheduler-E63946?style=flat-square&logo=github&labelColor=0D0D0D)](https://github.com/pixeLatedbLue/Adaptive-Loan-Payment-Scheduler)

</details>

---

<details>
<summary><b>🤲 Hand Tremor Stabilization Device</b> &nbsp;<code>C++ · Arduino · Embedded · Assistive Tech</code></summary>

<br/>

> *Low-cost real-time assistive device for Parkinson's & essential tremor patients*

An embedded hardware system that restores independence for people with involuntary hand movements — stabilizing spoons and brushes in real time:

| Component | Role |
|:---|:---|
| MPU6050 | 6-DOF motion sensing — detects & classifies tremor signatures |
| Arduino Nano | Embedded control loop & signal processing |
| Servo Motor | Real-time physical counterforce stabilization |
| USB Power | Portable & accessible form factor |

**Signal flow:** `Sensor reads → Tremor classification → Servo actuation` *(continuous loop)*

[![Repo](https://img.shields.io/badge/View%20Repo-Tremor--Stabilization--Device-E63946?style=flat-square&logo=github&labelColor=0D0D0D)](https://github.com/pixeLatedbLue/Tremor-Stabilization-Device-)

</details>

---

## `> tech_stack`

<div align="center">

**Languages**

<img src="https://skillicons.dev/icons?i=python,cpp,c,js,html,css,react&theme=dark" />

**AI / ML & XAI**

<img src="https://skillicons.dev/icons?i=pytorch,tensorflow,sklearn&theme=dark" />

`Isolation Forest` &nbsp;·&nbsp; `SHAP` &nbsp;·&nbsp; `Behavioral Modeling` &nbsp;·&nbsp; `Streamlit`

**Autonomous & Embedded**

<img src="https://skillicons.dev/icons?i=linux,git,github&theme=dark" />

`ROS2 Jazzy` &nbsp;·&nbsp; `Arduino` &nbsp;·&nbsp; `Nvidia Jetson Orin Nano` &nbsp;·&nbsp; `Intel RealSense D435i` &nbsp;·&nbsp; `SBG Ellipse IMU` &nbsp;·&nbsp; `Ollama` &nbsp;·&nbsp; `Decision Systems`

</div>

---

## `> achievements`

```
🥇  Gold Badge Problem Solver          CodeChef
📡  Active Member                      IEEE-VIT
🏁  Autonomous Software Developer      Team Ojas Racing — Formula Student EV
📋  Operations Team Member (CR)        Team Ojas Racing — Formula Student EV
```

---

## `> github_analytics`

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=pixeLatedbLue&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0D0D0D&title_color=E63946&icon_color=FF9F1C&text_color=C8C5BF&rank_icon=github" />

<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=pixeLatedbLue&layout=compact&theme=tokyonight&hide_border=true&bg_color=0D0D0D&title_color=E63946&text_color=C8C5BF" />

<img src="https://github-readme-streak-stats.herokuapp.com/?user=pixeLatedbLue&theme=tokyonight&hide_border=true&background=0D0D0D&ring=E63946&fire=FF9F1C&currStreakLabel=C8C5BF&sideLabels=C8C5BF&dates=888580" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=pixeLatedbLue&theme=tokyo-night&bg_color=0D0D0D&color=C8C5BF&line=E63946&point=FF9F1C&area=true&hide_border=true" width="100%" />

</div>

---

## `> connect`

<div align="center">

<a href="https://www.linkedin.com/in/naval-agarwal-48b678205/">
  <img src="https://img.shields.io/badge/LinkedIn-Naval%20Agarwal-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white&labelColor=0D0D0D" />
</a>
&nbsp;&nbsp;
<a href="https://github.com/pixeLatedbLue">
  <img src="https://img.shields.io/badge/GitHub-pixeLatedbLue-E63946?style=for-the-badge&logo=github&logoColor=white&labelColor=0D0D0D" />
</a>

</div>

---

<div align="center">

<img src="https://komarev.com/ghpvc/?username=pixeLatedbLue&style=flat-square&color=E63946&label=profile+views" />

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=100&section=footer&animation=twinkling" width="100%"/>

</div>
