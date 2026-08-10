<h1 align="center">Mohsen Seyedkazemi Ardebili</h1>

<p align="center">
  <b>AI Infrastructure · AI SRE &amp; AIOps · MLOps · HPC</b><br/>
  Research Fellow, University of Bologna · Bologna, Italy
</p>

<p align="center">
  <a href="https://mskazemi.com/"><img src="https://img.shields.io/badge/Website-mskazemi.com-222222?style=flat&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://mskazemi.com/hire/"><img src="https://img.shields.io/badge/Available%20for%20freelance-remote%20·%20EU-3FD79A?style=flat" alt="Available for freelance work, remote across the EU" /></a>
  <a href="https://www.linkedin.com/in/mskazemi/"><img src="https://img.shields.io/badge/LinkedIn-mskazemi-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://scholar.google.com/citations?user=xP64pZsAAAAJ"><img src="https://img.shields.io/badge/Google-Scholar-4285F4?style=flat&logo=googlescholar&logoColor=white" alt="Google Scholar" /></a>
  <a href="https://orcid.org/0000-0002-1166-6559"><img src="https://img.shields.io/badge/ORCID-0000--0002--1166--6559-A6CE39?style=flat&logo=orcid&logoColor=white" alt="ORCID" /></a>
  <a href="https://doi.org/10.1007/s10723-026-09837-6"><img src="https://img.shields.io/badge/Peer--reviewed-J.%20Grid%20Computing-b31b1b?style=flat&logo=doi&logoColor=white" alt="Peer-reviewed in the Journal of Grid Computing" /></a>
</p>

---

I build autonomous AI systems that **act** on infrastructure — not just explain it.

I came to this the unusual way round. Before the PhD I spent seven years as the IT and network
administrator of a combined-cycle power plant of more than 1,000 MW: no staging environment, and a
bad change measured in megawatts rather than in error budgets. Then a doctorate in high-performance
computing at the University of Bologna, and since then research and platform engineering on
EuroHPC-funded projects.

That background is why my systems ask before they act. Everything below is one attempt at the same
question: **how much of an operator's judgement can a machine take over, and how do you prove
afterwards that it was right to?**

📍 Bologna, Italy · remote across the EU &nbsp;·&nbsp; 🧭 [mskazemi.com](https://mskazemi.com/) &nbsp;·&nbsp; 💼 [available for freelance work](https://mskazemi.com/hire/)

---

## Featured Project

### [KubeIntellect](https://github.com/MSKazemi/kubeintellect) — a human-governed AI SRE for Kubernetes

> Ask your Kubernetes cluster a question in plain English. It gathers live evidence from tools such
> as kubectl, Prometheus and Loki, works out what is actually wrong — and pauses for your explicit
> approval before it changes anything.

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://github.com/MSKazemi/kubeintellect)
[![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat&logo=langchain&logoColor=white)](https://github.com/MSKazemi/kubeintellect)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)](https://github.com/MSKazemi/kubeintellect)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)](https://github.com/MSKazemi/kubeintellect)

- It **executes** cluster operations, behind a human approval gate — that is the whole point, and it
  is what separates it from a chat window next to a terminal
- LangGraph FSM supervisor with PostgreSQL checkpoints and human-in-the-loop approval gates
- Dynamic Code-Generator agent: writes and validates new tools at runtime, with registration routed
  through human approval
- Modular domain agents: logs, metrics, RBAC, lifecycle, scheduling, exec, proxy
- **Peer-reviewed** — *Journal of Grid Computing* (2026), [10.1007/s10723-026-09837-6](https://doi.org/10.1007/s10723-026-09837-6)

---

## Other Projects

| Project | What it does | Evidence | Stack |
|---|---|---|---|
| **[NovaFabric](https://github.com/MSKazemi/novafabric)** | A time machine for AI systems — capture, replay, diff and audit any agent or HPC run, with no code changes. Self-hosted. | Apache-2.0 · experimental · [novafabric.ai](https://novafabric.ai) | Python, OpenTelemetry |
| **[YazSes](https://github.com/MSKazemi/yazses)** | Push-to-talk voice dictation for Linux, macOS and Windows. Hold a key, speak, release — on-device speech-to-text types into any app. Also transcribes recordings and labels meeting speakers. | Fully offline **by default** · CPU-only, no GPU · Apache-2.0 · outside contributors merging PRs | Python, faster-whisper |
| **[AOBench](https://github.com/MSKazemi/aobench)** | Benchmark for LLM agents doing real HPC operations work. Role-aware and permission-enforced: a policy violation hard-fails the task, however correct the answer looked. | 88 tasks (10 categories × 5 roles) · 29 environment bundles, 6 from real Marconi100 telemetry · [archived with a DOI](https://doi.org/10.5281/zenodo.21854863) · paper under review | Python, MCP, Slurm |
| **[ExaMLOps](https://github.com/MSKazemi/ExaMLOps)** | End-to-end MLOps platform for HPC, built for the EuroHPC **SEANERGYS** project. Any of the sixteen consortium partners registers a model; the platform trains, versions, governs and serves it. Architect and lead developer. | In production at LuxProvide (MeluXina) · train → version → govern → serve, behind a sysadmin approval gate | Prefect, MLflow, Ray Serve, Slurm, FastAPI, React |
| **[kube-q](https://github.com/MSKazemi/kubeintellect/tree/main/v4/packages/kube-q)** | CLI and Python SDK for KubeIntellect — `pip install kube-q` | Streaming responses, Rich TUI · AGPL-3.0 | Python |
| **[GRAAFE](https://github.com/MSKazemi/GRAAFE)** | Graph neural network that anticipates compute-node anomalies on exascale HPC, trained offline and served online through a Kubeflow pipeline on live telemetry. | Published, *FGCS* 2024 · CINECA Marconi100 | Python, GNN, Kubeflow |
| **[HazardNet](https://github.com/MSKazemi/HazardNet)** | Thermal-hazard prediction for datacenters, over a year of temperature and power telemetry from 3,312 nodes of CINECA's Marconi A2. Six-hour horizon, chosen with the facility manager. | Published, *FGCS* 2024 · [1 GB dataset on Zenodo](https://doi.org/10.5281/zenodo.10050368), CC BY 4.0 | Python, TCN/LSTM/SVM |

---

## Available for freelance work

Remote across the EU, in three areas — each starting with a fixed-price audit so you can see the
work before committing to a project:

- **Kubernetes reliability & AIOps** — health-checks, observability, hardening, incident root-cause analysis
- **MLOps & ML in production** — registry, serving, drift detection, governed retraining, monitoring
- **Production LLM agents** — tool boundaries, scoped RBAC, human-in-the-loop safety, tracing, audit trails

Based in Bologna, Italy — working remotely across the EU on CET.

**→ [Engagements, rates and how it works](https://mskazemi.com/hire/)**

---

## Research

**PhD:** Design, Analysis, and Management of High-Performance Computing Systems · University of Bologna (2018–2022)

**EU projects:** SEANERGYS (EuroHPC-JU — MLOps platform architect & lead developer, WP task lead) · DECICE · Graph-Massivizer · EUROPEAN PILOT · REGALE · EPI SGA1

**Impact** *(Google Scholar, read 2026-08-10 — see the live profile for current figures)*:
**218 citations · h-index 8 · i10-index 7**, across 17 published or accepted peer-reviewed works.
The trend is the interesting part: 9 citations in 2022, 15 in 2023, 24 in 2024, 76 in 2025, and 65
in the first seven months of 2026 — more in the last twenty months than in the preceding eighteen
years combined.

### Selected Publications

| Title | Venue | Year |
|-------|-------|------|
| [KubeIntellect: A Modular LLM-Orchestrated Agent Framework for Kubernetes Management](https://doi.org/10.1007/s10723-026-09837-6) | *Journal of Grid Computing* | 2026 |
| [M100 ExaData: A Data Collection Campaign on CINECA's Marconi100 Tier-0 Supercomputer](https://www.nature.com/articles/s41597-023-02174-3) | *Nature Scientific Data* | 2023 |
| [PM100: A Job Power Consumption Dataset of a Large-Scale Production HPC System](https://doi.org/10.1145/3624062.3624263) | SC'23 Workshops | 2023 |
| [GRAAFE: GRaph Anomaly Anticipation Framework for Exascale HPC Systems](https://doi.org/10.1016/j.future.2024.06.032) | *FGCS* | 2024 |
| [HazardNet: A Thermal Hazard Prediction Framework for Datacenters](https://doi.org/10.1016/j.future.2024.01.031) | *FGCS* | 2024 |
| [Elevating Datacenter Resilience with ThermADNet: A Thermal Anomaly Detection System](https://doi.org/10.1016/j.future.2025.108311) | *FGCS* | 2026 |
| [Multi-level Anomaly Prediction in Tier-0 Datacenter](https://doi.org/10.1145/3528416.3530864) | *ACM Computing Frontiers* | 2022 |

**Open data.** I co-author three CC BY 4.0 datasets from CINECA's Tier-0 supercomputers — roughly
26 GB in total: [M100 ExaData](https://doi.org/10.5281/zenodo.7541722) (24.8 GB of Marconi100
telemetry), the [HazardNet thermal dataset](https://doi.org/10.5281/zenodo.10050368) (3,312 nodes,
first author) and [PM100](https://doi.org/10.5281/zenodo.10127767) (per-job power). Free to download,
commercial use permitted.

[Full list, with current citation counts → Google Scholar](https://scholar.google.com/citations?user=xP64pZsAAAAJ) · [ORCID](https://orcid.org/0000-0002-1166-6559) · [dblp](https://dblp.org/pid/282/6179) · [OpenAlex](https://openalex.org/A5013086540)

---

## Stack

| Area | Tools |
|---|---|
| **Platform & infrastructure** | Kubernetes · Helm · Terraform · Docker · Linux · Azure |
| **AI / ML** | Python · PyTorch · LangGraph · FastAPI · MLflow · Ray Serve |
| **HPC** | Slurm · MPI · OpenMP · Prefect |
| **Observability** | Prometheus · Grafana · Loki · OpenTelemetry |
| **Data & ML systems** | GNNs · TCN/LSTM · anomaly detection · time-series telemetry at datacenter scale |

---

## Academic Service

**PC Member:** PDP 2025 · PDP 2026 · AsHES 2026

**Reviewer:** IEEE TCAD · FGCS · Journal of Grid Computing · SC · ACM CF · DATE · PDP · AsHES

**Supervision:** 2 PhD co-advisees (ongoing) · 5 MSc theses completed · Lab of Big Data Architectures, UniBo (2020–2024)

---

<p align="center">
  <b>Hiring, or need an audit?</b> → <a href="https://mskazemi.com/hire/">mskazemi.com/hire</a><br/>
  <sub>
    <a href="https://mskazemi.com/">Website</a> ·
    <a href="https://mskazemi.com/about/">About</a> ·
    <a href="https://www.linkedin.com/in/mskazemi/">LinkedIn</a> ·
    <a href="https://gitlab.com/mskazemi">GitLab</a> ·
    <a href="https://mastodon.social/@mskazemi">Mastodon</a> ·
    <a href="https://scholar.google.com/citations?user=xP64pZsAAAAJ">Scholar</a> ·
    <a href="https://orcid.org/0000-0002-1166-6559">ORCID</a>
  </sub>
</p>
