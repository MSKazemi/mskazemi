<h1 align="center">Mohsen Seyedkazemi Ardebili</h1>

<p align="center">
  <b>AI Platform &amp; Agentic AI Infrastructure Engineer</b><br/>
  Agentic AI · MLOps/LLMOps · Kubernetes &amp; HPC · Research Fellow, University of Bologna
</p>

<p align="center">
  <a href="https://mskazemi.com/"><img src="https://img.shields.io/badge/Website-mskazemi.com-222222?style=flat&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://www.linkedin.com/in/mskazemi/"><img src="https://img.shields.io/badge/LinkedIn-mskazemi-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="https://mskazemi.com/hire/"><img src="https://img.shields.io/badge/Open%20to-full--time%20·%20contract%20·%20freelance-3FD79A?style=flat" alt="Open to full-time, contract and freelance work, remote across the EU" /></a>
</p>

I build **autonomous AI that acts on infrastructure — with a human at the gate.**

I design and operate the platforms that let AI agents and ML models run in production without
anyone losing control of them: approval gates, scoped RBAC, model registries, replay and audit
trails. I came to it the unusual way round — nearly nine years in enterprise IT and network
operations, six of them as IT and network administrator of a combined-cycle power plant of more
than 1,000 MW, where there is no staging environment and a bad change measures in megawatts, then
a PhD in high-performance computing.

📍 Bologna, Italy · remote across the EU &nbsp;·&nbsp; 🧭 [mskazemi.com](https://mskazemi.com/) &nbsp;·&nbsp; 💼 [open to full-time · contract · freelance](https://mskazemi.com/hire/)

---

## Proof of work

### [ExaMLOps](https://github.com/MSKazemi/ExaMLOps) — production MLOps platform for HPC

**My role:** architect and lead developer.

|  |  |
|---|---|
| **Problem** | Sixteen partners on a EuroHPC consortium each needed to train, version, govern and serve models on a Tier-0 supercomputer — with no shared platform to do it on. |
| **What I built** | An end-to-end MLOps platform: a partner registers a model, the platform trains, versions, governs and serves it, behind a sysadmin approval gate. |
| **Proof** | In production at LuxProvide (MeluXina), for the EuroHPC **SEANERGYS** project. |

`Prefect` · `MLflow` · `Ray Serve` · `Slurm` · `FastAPI` · `React`

### [KubeIntellect](https://github.com/MSKazemi/kubeintellect) — a human-governed AI SRE for Kubernetes

**My role:** creator and first author of the peer-reviewed paper.

|  |  |
|---|---|
| **Problem** | Diagnosing a live Kubernetes fault means correlating kubectl, Prometheus and Loki by hand under time pressure — and any tool that fixes it automatically is a tool nobody will run in production. |
| **What I built** | Ask the cluster a question in plain English. It gathers live evidence, works out what is actually wrong, and **executes** the remediation — pausing for explicit human approval before it changes anything. |
| **Proof** | Peer-reviewed in the *Journal of Grid Computing* (2026), [10.1007/s10723-026-09837-6](https://doi.org/10.1007/s10723-026-09837-6) · [live demo](https://kubeintellect.com/demo) · `pip install kubeintellect` |

That it acts, behind a gate, is the whole point — it is what separates it from a chat window next to
a terminal. Domain agents cover logs, metrics, RBAC, lifecycle, scheduling, exec and proxy; the
supervisor is a LangGraph state machine with PostgreSQL checkpoints, and a code-generator agent
writes and validates new tools at runtime with registration routed through the same human approval.

`Python` · `LangGraph` · `FastAPI` · `Kubernetes` · `PostgreSQL`

### [AOBench](https://github.com/MSKazemi/aobench) — evaluation and permission infrastructure for AI agents

**My role:** creator.

|  |  |
|---|---|
| **Problem** | Agent benchmarks score whether the answer looked correct. In operations, an agent that reaches the right answer by exceeding its permissions has failed. |
| **What I built** | A role-aware, permission-enforced benchmark for LLM agents doing real HPC operations work: a policy violation hard-fails the task, however correct the output. |
| **Proof** | 88 tasks across 10 categories × 5 roles · [archived with a DOI](https://doi.org/10.5281/zenodo.21854863) · paper under review. |

`Python` · `MCP` · `Slurm` · `RBAC`

---

## Also shipped

| Project | What it does | Evidence | Stack |
|---|---|---|---|
| **[YazSes](https://github.com/MSKazemi/yazses)** | Offline voice dictation that never phones home. Hold a key, speak, release — speech-to-text runs on your own CPU and the words are typed into whatever window has focus. **Works on Wayland**, where most dictation tools silently fail. | Apache-2.0 · cross-platform · built in the open by outside contributors, [good first issues tagged](https://github.com/MSKazemi/yazses/issues?q=is%3Aopen+label%3A%22good+first+issue%22) · [measured accuracy, published method](https://mskazemi.com/yazses/benchmarks.html) | Python, faster-whisper, Linux/macOS/Windows |
| **[NovaFabric](https://github.com/MSKazemi/novafabric)** | A time machine for AI systems — capture, replay, diff and audit any agent or HPC run, with no code changes. Self-hosted. | Apache-2.0 · experimental · [novafabric.ai](https://novafabric.ai) | Python, OpenTelemetry |
| **[kube-q](https://github.com/MSKazemi/kubeintellect/tree/main/v4/packages/kube-q)** | CLI and Python SDK for KubeIntellect — `pip install kube-q` | Streaming responses, Rich TUI · AGPL-3.0 | Python |

## Research systems

| Project | What it does | Evidence |
|---|---|---|
| **[GRAAFE](https://github.com/MSKazemi/GRAAFE)** | Graph neural network that anticipates compute-node anomalies on exascale HPC — trained offline, served online through a Kubeflow pipeline on live telemetry. | Published, *FGCS* 2024 · CINECA Marconi100 |
| **[HazardNet](https://github.com/MSKazemi/HazardNet)** | Thermal-hazard prediction for datacenters, over a year of telemetry from 3,312 nodes of CINECA's Marconi A2. Six-hour horizon, chosen with the facility manager. | Published, *FGCS* 2024 · [1 GB dataset on Zenodo](https://doi.org/10.5281/zenodo.10050368), CC BY 4.0 |

---

## Stack

| Area | Tools |
|---|---|
| **Platform & infrastructure** | Kubernetes · OpenShift · Helm · Terraform · Docker · Linux · Azure |
| **Agentic AI & LLM** | LangGraph · MCP · A2A · RAG · vLLM · FastAPI |
| **MLOps & pipelines** | MLflow · Kubeflow · Prefect · Ray Serve · KServe |
| **HPC** | Slurm · MPI · OpenMP |
| **Observability** | Prometheus · Grafana · Loki · OpenTelemetry |
| **ML systems** | Python · PyTorch · GNNs · TCN/LSTM · anomaly detection · time-series telemetry at datacenter scale |

---

## Research

**PhD:** Design, Analysis, and Management of High-Performance Computing Systems · University of Bologna (2018–2022)

Selected peer-reviewed work:

| Paper | Venue | Year |
|---|---|---|
| [KubeIntellect: A Modular LLM-Orchestrated Agent Framework for Kubernetes Management](https://doi.org/10.1007/s10723-026-09837-6) | *Journal of Grid Computing* | 2026 |
| [M100 ExaData: A Data Collection Campaign on CINECA's Marconi100 Tier-0 Supercomputer](https://www.nature.com/articles/s41597-023-02174-3) | *Nature Scientific Data* | 2023 |
| [GRAAFE: GRaph Anomaly Anticipation Framework for Exascale HPC Systems](https://doi.org/10.1016/j.future.2024.06.032) | *FGCS* | 2024 |

Three open datasets, 26 GB in total: [M100 ExaData](https://doi.org/10.5281/zenodo.7541722),
the [HazardNet thermal dataset](https://doi.org/10.5281/zenodo.10050368) (first author) and
[PM100](https://doi.org/10.5281/zenodo.10127767) — free to download, no registration.

[Full publication list and current citation counts → Google Scholar](https://scholar.google.com/citations?user=xP64pZsAAAAJ) · [ORCID](https://orcid.org/0000-0002-1166-6559) · [dblp](https://dblp.org/pid/282/6179)

Reviewer for IEEE TCAD · FGCS · *Journal of Grid Computing* · SC · ACM CF · DATE · PDP · AsHES.
PC member: PDP 2025 · PDP 2026 · AsHES 2026.

---

## Two ways to work with me

**Hiring for AI Platform · Agentic AI · MLOps/LLMOps · Kubernetes?**
Remote across the EU, on CET. Full background and experience on
**[LinkedIn](https://www.linkedin.com/in/mskazemi/)** — or email
**[mohsen@mskazemi.com](mailto:mohsen@mskazemi.com)**.

**Need a consulting engagement or an audit?** Three areas, each starting with a fixed-price audit so
you can see the work before committing to a project:

- **Kubernetes reliability & AIOps** — health-checks, observability, hardening, incident root-cause analysis
- **MLOps & ML in production** — registry, serving, drift detection, governed retraining, monitoring
- **Production LLM agents** — tool boundaries, scoped RBAC, human-in-the-loop safety, tracing, audit trails

**→ [Engagements, rates and how it works](https://mskazemi.com/hire/)**

---

<p align="center">
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
