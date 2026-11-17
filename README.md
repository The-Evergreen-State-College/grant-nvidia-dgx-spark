# Grant Proposal: NVIDIA DGX Spark HPC Developer Kit for Interdisciplinary STEM & Local AI Workflows

Repository for grant development, technical documentation, budget justification, and funder outreach supporting the acquisition of an **NVIDIA DGX Spark HPC Developer Kit** for the **Computer Applications Lab for Scientific Computing** at **The Evergreen State College** (Olympia, WA).

---

## Project Overview

* **Applicant & Fiscal Agent:** The Evergreen State College Foundation (501(c)(3) Public Charity, EIN `13-1837418`)
* **Primary Beneficiary Unit:** Computer Applications Lab for Scientific Computing, Academic Affairs, The Evergreen State College
* **Equipment Requested:** One (1) 4-Node **NVIDIA DGX Spark HPC Developer Kit**
* **Total Funding Target:** **$32,000**
* **Acquisition Pathway:** Direct 501(c)(3) Foundation purchase and formal **Gift-in-Kind** equipment transfer to Academic Affairs

### Core Objective
Provide Evergreen undergraduate and graduate STEM students with dedicated, on-campus desktop supercomputing capacity for local large language model (LLM) engineering, agentic AI workflows, and GPU-accelerated scientific simulation—eliminating recurring commercial cloud GPU costs while keeping unpublished ecological, biological, and community datasets local and secure.

---

## Technical Architecture

The requested **NVIDIA DGX Spark HPC Developer Kit** delivers data-center-grade CUDA and Grace Blackwell architecture in a quiet, energy-efficient deskside cluster engineered for academic laboratories:

| Component | Specification | Instructional & Research Capability |
| :--- | :--- | :--- |
| **Compute Nodes** | 4 x NVIDIA DGX Spark systems (GB10 Grace Blackwell Superchip; 20-core Arm CPU + Blackwell GPU per node) | Up to **4 PFLOPs FP4** aggregate AI compute; supports multi-node MPI and distributed training |
| **Unified Memory** | **512 GB** coherent LPDDR5x aggregate memory (4 x 128 GB at 273 GB/s per node) | Local inference up to **700B parameters** (NVFP4) and multi-node LoRA fine-tuning on 120B+ models |
| **Cluster Interconnect** | Switchless **200 Gbps NVIDIA ConnectX-7** QSFP112 direct-ring topology | High-speed NCCL/RDMA node-to-node communication without requiring a separate 200GbE switch |
| **Local Storage** | **16–20 TB** aggregate high-speed NVMe M.2 self-encrypting SSD storage | Houses open-weight model checkpoints, bioacoustics archives, and environmental corpora on-site |
| **Software Stack** | **NVIDIA DGX OS** (Ubuntu-based), CUDA, NVIDIA HPC SDK, Docker, PyTorch, `vLLM`, `llama.cpp` | Standard Linux/CUDA toolchain aligned with national supercomputing centers and industry workflows |

---

## STEM Curriculum & Research Workflows

The cluster will be integrated directly into lower- and upper-division interdisciplinary STEM programs across four primary domains:

1. **Local LLM & Agentic AI Engineering:** Deploying, quantizing, fine-tuning (LoRA), and benchmarking open-weight models using `vLLM`, `llama.cpp`, `Ollama`, and open-source agentic frameworks (`OpenClaw`, `Hermes Agent`, and `NVIDIA Nemotron` recipes) without API rate limits or external data exposure.
2. **Bioacoustics & Ecological Data Science:** GPU-accelerated spectral analysis, species classification, and automated acoustic event detection across multi-terabyte field recording archives.
3. **Molecular Dynamics & Computational Chemistry:** Multi-node protein-ligand and materials simulations using the **NVIDIA HPC SDK** with `LAMMPS` (Kokkos), `NAMD`, `GROMACS`, and `OpenFold3` / `Boltz-2` microservices.
4. **Climate, Watershed & Geospatial Modeling:** Local execution of GPU-accelerated `WRF` weather modeling, `OpenFOAM` computational fluid dynamics, and spatial machine learning pipelines (`cuML`) for Puget Sound marine and watershed datasets.

---

## Itemized Project Budget

| Line Item | Description | Unit Cost | Qty | Total |
| :--- | :--- | :--- | :--- | :--- |
| **NVIDIA DGX Spark Nodes** | 128 GB Unified Memory, GB10 Grace Blackwell Superchip, 4 TB NVMe SSD, DGX OS | $6,950 | 4 | $27,800 |
| **Interconnects & Power** | NVIDIA ConnectX-7 200 GbE QSFP112 Direct-Attach Copper (DAC) ring cables & dedicated lab UPS/surge protection | $300 | 4 | $1,200 |
| **Freight & Handling** | Insured commercial shipping and delivery to campus | — | — | $91 |
| **Subtotal — Equipment & Delivery** | | | | **$29,091** |
| **Washington State Sales Tax** | Combined State & City of Olympia sales tax (10.0% rate) | — | — | $2,909 |
| **Total Grant Request** | | | | **$32,000** |

---

## Third-Party Procurement & Deployment Model

To ensure rapid equipment acquisition and dedicated lab stewardship:

* **501(c)(3) Foundation Fiscal Sponsorship:** Corporate and private foundation grants are awarded directly to **The Evergreen State College Foundation** (EIN `13-1837418`). The Foundation executes the hardware purchase directly with an authorized NVIDIA OEM/marketplace partner and transfers the completed system to Academic Affairs for the **Computer Applications Lab for Scientific Computing** as a formal **Gift-in-Kind**.
* **Isolated Laboratory Network Architecture:** The 4-node cluster operates on a dedicated local laboratory switch within the **Computer Applications Lab for Scientific Computing**, providing low-latency SSH, JupyterHub, and local web-UI access for coursework and student research without adding dependency on central campus endpoint management.
* **Zero Recurring Cloud Overhead:** All software components (`DGX OS`, `CUDA`, `NVIDIA HPC SDK`, and open-source AI/HPC frameworks) carry zero per-seat licensing fees, enabling sustainable operation over a projected 5-year instructional lifecycle.

---

## Target Funding Sources (Foundation Pass-Through Eligible)

The following regional corporate, bank, and community foundations allow or require public colleges to apply through their affiliated 501(c)(3) Foundation:

| Funder | Typical Award | Cycle / Timing | Primary Alignment |
| :--- | :--- | :--- | :--- |
| **Employees Community Fund (ECF) of Boeing Puget Sound** | Up to $50,000 | Quarterly / semi-annual windows | STEM workforce readiness & hands-on lab equipment |
| **The Norcliffe Foundation** (Seattle, WA) | $10,000 – $75,000+ | Rolling year-round (Board reviews every ~6–8 weeks) | Applied STEM & scientific computing capacity in Western WA |
| **The Boeing Company** (Corporate Citizenship) | $15,000 – $100,000+ | Annual / Advancement-coordinated | Post-secondary AI literacy & diverse technical talent pipelines |
| **U.S. Bank Foundation** (*Community Possible – Work*) | $10,000 – $90,000 | Rolling / regional invitation | Career-connected technical & AI training for first-generation students |
| **KeyBank Foundation** | $15,000 – $100,000+ | Rolling / regional review | Applied computational and AI skills aligned with regional employers |
| **Puget Sound Energy (PSE) Foundation** | $5,000 – $25,000 | Annual competitive & partnership cycles | Energy-efficient local AI compute for environmental & watershed modeling |
| **Community Foundation of South Puget Sound** (Olympia, WA) | $1,500 – $7,500 (Competitive)<br>Open (DAF) | Competitive opens Jan 2027; Donor-Advised Funds year-round | Single-node expansion or community-engaged environmental data projects |

---

## Measurable Outcomes (Year 1)

* **Student Reach:** Serve **120 to 160 undergraduate and graduate students annually** across computer science, data science, environmental studies, chemistry, and biology.
* **Curricular Integration:** Support at least **6 interdisciplinary academic programs** and **25+ senior capstone and faculty-mentored research projects** per academic year.
* **Cost Avoidance:** Eliminate an estimated **$15,000–$25,000 per year** in equivalent commercial cloud GPU rental costs while ensuring equitable hardware access for all enrolled students.

---

## Recommended Repository Structure

```text
grant-nvidia-dgx-spark/
├── README.md                     # Project overview, specs, budget, and funder matrix
├── docs/
│   ├── grant-summary.md          # Core executive summary and narrative modules
│   └── curriculum-workflows.md   # Course syllabi integrations and lab runbooks
├── budget/
│   └── budget-justification.md   # Itemized equipment, tax, and lifecycle cost breakdown
└── outreach/
    └── funder-tracking.md        # Advancement routing, LOI deadlines, and vendor quotes
```

---

## Institutional Coordination Notes

Per **The Evergreen State College Grants Policy**, proposals submitted through **The Evergreen State College Foundation** should be coordinated internally with:
1. **Academic Affairs Sponsor** (Academic Dean / Provost sign-off on lab priority and Gift-in-Kind acceptance)
2. **The Evergreen State College Foundation / Advancement** (`foundation@evergreen.edu`)
3. **Evergreen Grants and Contracts Office** (`grants@evergreen.edu`)
