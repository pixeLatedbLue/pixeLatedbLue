<div align="center">

# Naval Agarwal

**CSE (AI/ML) · VIT Vellore** &nbsp;·&nbsp; **Autonomous software at Team Ojas Racing**

<br/>

<img src="https://img.shields.io/badge/VIT_Vellore-CSE_(AI%2FML)-2563EB?style=flat-square&labelColor=0D1117" alt="VIT Vellore" />
<img src="https://img.shields.io/badge/Team_Ojas_Racing-Formula_Student_Driverless-2563EB?style=flat-square&labelColor=0D1117" alt="Team Ojas Racing" />
<img src="https://img.shields.io/badge/Mumbai-India-30363D?style=flat-square&labelColor=0D1117" alt="Mumbai, India" />

<img src="https://img.shields.io/badge/CodeChef-Gold-30363D?style=flat-square&labelColor=0D1117&logo=codechef" alt="CodeChef Gold" />
<img src="https://img.shields.io/badge/IEEE-VIT_Member-30363D?style=flat-square&labelColor=0D1117&logo=ieee" alt="IEEE VIT Member" />

<br/><br/>

[About](#about) &nbsp;·&nbsp; [What I'm working on](#what-im-working-on) &nbsp;·&nbsp; [Selected projects](#selected-projects) &nbsp;·&nbsp; [Stack](#stack) &nbsp;·&nbsp; [Elsewhere](#elsewhere)

</div>

---

## About

I'm a second-year CSE (AI/ML) student at VIT Vellore. Most of my time goes into the
autonomous software for our Formula Student driverless car at **Team Ojas Racing** —
the perception, planning and control that has to run in real time, on a real car,
with nobody touching the wheel.

Away from the team I build a fairly wide mix of things: an LLM robustness research
framework, a few C++ decision engines, some security tooling, and the occasional web app.
The common thread is that I like problems where the program has to actually *decide*
something — pick a racing line, flag a risky user, choose which loan to pay off first —
and where being wrong has a real cost.

## What I'm working on

**Team Ojas Racing — Formula Student Driverless (EV).**
Autonomous Software Developer, and Operations / CR on the side.

I work across the autonomy stack on a ROS2 Jazzy architecture: stereo depth from an
Intel RealSense D435i fused with an SBG Ellipse N IMU for perception, the planning and
control that turns that into steering and throttle, and getting all of it to run on a
Jetson Orin Nano on the car. The interesting part isn't making it work once — it's
making it correct enough to trust at speed.

## Currently learning

Tighter sensor fusion and SLAM, getting perception to run faster on the Jetson
(CUDA / TensorRT), and reinforcement learning for control rather than just for games.

## Selected projects

**Autonomy & robotics**

- **[TOR27 — FSD Path Planning](https://github.com/pixeLatedbLue/TOR27_PathPlanning_v0)** · `Python`
  A path-planning pipeline for the driverless car, with a live viewer so you can watch it
  think. It maps the track from cone detections, plans a line through it, and drives all
  four Formula Student missions — acceleration, skidpad, autocross and trackdrive. It also
  models the safety side: the AS state machine, the ASMS / RES / R2D arming sequence, and
  emergency braking. Still being validated on hardware, so it's honestly work in progress.

- **[speed-racer-rl](https://github.com/pixeLatedbLue/speed-racer-rl)** · `C++`
  A custom 2D racing simulator with a Deep Q-Network agent (libtorch). The car perceives
  the track through 13 LIDAR-style raycasts (an 18-dimensional state), trains headless,
  and trained models can be replayed visually with Raylib.

- **[SBG Ellipse N IMU nodes](https://github.com/pixeLatedbLue/sbgSystems-Ellipse-N-IMU)** · `Python · ROS`
  Three ROS nodes — publisher, processing and telemetry — for the SBG Ellipse N IMU that
  feeds the car's autonomous stack.

**ML & AI research**

- **[G0DM0D3](https://github.com/pixeLatedbLue/Self_G0DMODE3)** · `TypeScript`
  A modular framework for studying how large language models behave at inference time,
  without any access to their weights. Four composable pieces: AutoTune (context-aware
  sampling), Parseltongue (character-level input perturbation for red-teaming), STM
  (output normalization), and ULTRAPLINIAN, which races up to 51 models in parallel and
  scores them on one metric — plus an EMA feedback loop that learns from ratings.
  ~3,300 lines of TypeScript, with the full write-up in
  [PAPER.md](https://github.com/pixeLatedbLue/Self_G0DMODE3/blob/main/PAPER.md).

- **[ML-Assisted Adaptive Cache](https://github.com/pixeLatedbLue/ML-Assisted-Adaptive-Cache-Register-)** · `ML · Systems`
  Most CPUs run one fixed cache configuration no matter what the program is doing. This is
  an attempt to learn the workload instead — watch hit/miss rate, IPC and memory access
  frequency at runtime, then predict a better cache configuration for the current phase.

**Web & tools**

- **[CodeLens](https://codective-sand.vercel.app)** · `TypeScript · Next.js` · [source](https://github.com/pixeLatedbLue/Codective)
  Paste a GitHub repo URL and get a code-quality score with a breakdown — complexity,
  maintainability, style and bug safety — across 15+ languages. Live on Vercel.

**Security**

- **[Insider Fraud Detection](https://github.com/pixeLatedbLue/InsiderThreatRiskDetector)** · `Python`
  Endpoint and network monitoring for insider risk: device discovery, per-device traffic,
  USB events and remote agents, feeding an Isolation Forest model that scores users — and
  uses SHAP to explain *why* someone got flagged, including Big-Five behavioural signals.
  All of it behind a dashboard.

**Systems & embedded**

- **[Adaptive Loan Repayment Scheduler](https://github.com/pixeLatedbLue/Adaptive-Loan-Payment-Scheduler)** · `C++`
  Give it a set of loans and a monthly budget; it recomputes repayment priority every
  cycle from interest, tenure and balance, and returns the cheapest order to clear them.

- **[Tremor Stabilization Device](https://github.com/pixeLatedbLue/Tremor-Stabilization-Device-)** · `C++ · Arduino`
  An assistive device that keeps a spoon or brush steady for people with Parkinson's or
  essential tremor. An MPU6050 reads the tremor, an Arduino Nano classifies it, and a
  servo applies counterforce in real time.

## Stack

| | |
|---|---|
| **Languages** | Python · C++ · TypeScript / JavaScript · C |
| **ML / AI** | PyTorch · scikit-learn · Isolation Forest · SHAP · RL (DQN) · LLM evaluation |
| **Robotics & embedded** | ROS2 Jazzy · Gazebo · Jetson Orin Nano · Intel RealSense D435i · SBG Ellipse IMU · Arduino |
| **Web** | Next.js · React · Tailwind · Node / Express · Vercel |
| **Tools** | Linux · Git |

## Elsewhere

Reach me on **[LinkedIn](https://www.linkedin.com/in/naval-agarwal-48b678205/)** or at **navalag123@gmail.com**.
