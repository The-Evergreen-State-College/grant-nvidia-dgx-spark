## Grant Proposal Summary: Desktop Supercomputing for Interdisciplinary STEM & Local AI Workflows

* **Applicant & Fiscal Agent:** The Evergreen State College Foundation (501(c)(3) Public Charity, EIN `13-1837418`)
* **Primary Beneficiary Unit:** Computer Applications Lab for Scientific Computing, Academic Affairs, The Evergreen State College (Olympia, WA)
* **Equipment Requested:** One (1) 4-Node **NVIDIA DGX Spark HPC Developer Kit**
* **Total Funding Request:** **$32,000**
* **Procurement Pathway:** Direct Foundation purchase and Gift-in-Kind equipment transfer to Academic Affairs

---

### Executive Summary

The Evergreen State College Foundation requests **$32,000** to acquire one four-node **NVIDIA DGX Spark HPC Developer Kit** for the **Computer Applications Lab for Scientific Computing** at The Evergreen State College in Olympia, Washington. While proficiency in artificial intelligence, GPU-accelerated simulation, and large-scale data analysis has become foundational across the natural and computational sciences, undergraduate students at public liberal arts and sciences institutions face steep financial and privacy barriers when relying on commercial cloud GPU rentals or proprietary APIs. Recurring per-token and compute charges restrict hands-on experimentation, while transmitting unpublished environmental, biological, or community datasets to third-party cloud providers creates data-sovereignty and compliance risks.

Deploying a local, desk-scale **NVIDIA DGX Spark HPC Developer Kit**—featuring four Grace Blackwell GB10 nodes linked in a switchless 200 Gbps ConnectX-7 ring with 512 GB of aggregate coherent unified memory—eliminates recurring cloud expenses while giving Evergreen students direct access to supercomputing-class hardware. To ensure rapid, streamlined acquisition, **The Evergreen State College Foundation** will serve as the direct grant recipient and purchaser, acquiring the hardware directly from an authorized NVIDIA partner and transferring title to Academic Affairs via a Gift-in-Kind agreement.

---

### Institutional Need & STEM Curriculum Integration

Evergreen’s interdisciplinary, team-taught curriculum emphasizes experiential, inquiry-driven science where undergraduates work directly with primary instrumentation and real-world datasets from their first year through senior capstone research. Currently, student computing capacity in the **Computer Applications Lab for Scientific Computing** is constrained to standard CPU workstations and consumer-grade GPUs incapable of running modern foundation models, multi-node MPI simulations, or local retrieval-augmented generation (RAG) pipelines.

The NVIDIA DGX Spark HPC Developer Kit will be integrated immediately into upper- and lower-division STEM offerings across four core instructional workflows:

* **Local Large Language Model (LLM) & Agentic AI Engineering:** Students in computer science and data science programs will deploy, quantize, fine-tune (LoRA), and evaluate open-weight models (up to 120B–700B parameters in NVFP4 precision) using **vLLM**, **llama.cpp**, **Ollama**, and open-source agentic frameworks (**OpenClaw**, **Hermes Agent**, and **NVIDIA Nemotron** recipes) without external API throttling or data leakage.
* **Bioacoustics & Ecological Data Science:** Supporting Evergreen’s active field ecology and ornithology research, students will run GPU-accelerated spectral analysis, species classification, and automated acoustic event detection across multi-terabyte field recording archives stored locally on the cluster's NVMe array.
* **Molecular Dynamics & Computational Chemistry:** Using the **NVIDIA HPC SDK** and pre-validated playbooks for **LAMMPS (with Kokkos)**, **NAMD**, **GROMACS**, and **OpenFold3 / Boltz-2** microservices, chemistry and biology students will execute multi-node protein-ligand and materials simulations on campus rather than waiting days in external shared cluster queues.
* **Climate, Watershed & Geospatial Modeling:** Environmental studies students analyzing Puget Sound marine and watershed datasets will run GPU-accelerated **WRF** weather models, **OpenFOAM** fluid dynamics, and spatial machine learning pipelines (**cuML**) locally.

---

### Technical Architecture: NVIDIA DGX Spark HPC Developer Kit

The requested **NVIDIA DGX Spark HPC Developer Kit** provides data-center-grade CUDA and Grace Blackwell architecture in a quiet, energy-efficient desktop footprint engineered specifically for academic laboratories:

| Component | Technical Specification | Instructional & Research Capability |
| :--- | :--- | :--- |
| **Compute Nodes** | 4 × NVIDIA DGX Spark systems (GB10 Grace Blackwell Superchip; 20-core Arm CPU + Blackwell GPU per node) | Up to **4 PFLOPs FP4** aggregate AI compute; supports multi-node MPI and distributed training |
| **Unified Memory** | **512 GB** coherent LPDDR5x aggregate memory (4 × 128 GB @ 273 GB/s per node) | Local inference up to **700B parameters** (NVFP4) and multi-node LoRA fine-tuning on 120B+ models |
| **Cluster Interconnect** | Switchless **200 Gbps NVIDIA ConnectX-7** QSFP direct-ring topology | High-speed NCCL/RDMA node-to-node communication without requiring an expensive 200GbE switch |
| **Local Storage** | **16–20 TB** aggregate high-speed NVMe M.2 self-encrypting SSD storage | Houses large open-weight model checkpoints, genomics/bioacoustics corpora, and climate datasets on-site |
| **Software Ecosystem** | **NVIDIA DGX OS** (Ubuntu-based), CUDA, NVIDIA HPC SDK, Docker, PyTorch, vLLM, llama.cpp | Standard Linux/CUDA toolchain matching national supercomputing centers and industry workflows |

---

### Procurement, Deployment & Sustainability Plan

* **Third-Party Foundation Procurement:** Upon grant award, **The Evergreen State College Foundation** will receive the restricted funds and issue the purchase order directly to an authorized NVIDIA OEM/marketplace vendor. Upon delivery to campus, the Foundation will transfer ownership to Academic Affairs for the **Computer Applications Lab for Scientific Computing** as a formal **Gift-in-Kind**, ensuring dedicated academic stewardship and rapid classroom deployment.
* **Dedicated Lab Operations & Network Isolation:** The cluster will be housed in a secure, climate-controlled space within the **Computer Applications Lab for Scientific Computing** on a dedicated local laboratory switch, providing immediate, low-latency SSH, JupyterHub, and web-interface access to students and faculty across campus.
* **Zero Recurring Cloud Overhead:** Because DGX OS, CUDA, the NVIDIA HPC SDK, and the target open-source AI/simulation stacks carry no recurring per-seat licensing fees, the hardware will operate within existing **Computer Applications Lab for Scientific Computing** power and technical staffing budgets over a projected 5-year instructional lifecycle.

---

### Itemized Project Budget

| Line Item | Description | Unit Cost | Qty | Total |
| :--- | :--- | :--- | :--- | :--- |
| **NVIDIA DGX Spark Nodes** | 128 GB Unified Memory, GB10 Grace Blackwell Superchip, 4 TB NVMe SSD, DGX OS | $6,950 | 4 | $27,800 |
| **Cluster Interconnects & Power** | NVIDIA ConnectX-7 200 GbE QSFP112 Direct-Attach Copper (DAC) ring cables & dedicated lab UPS/surge protection | $300 | 4 | $1,200 |
| **Freight & Handling** | Insured commercial shipping and delivery to campus | — | — | $91 |
| **Subtotal — Equipment & Delivery** | | | | **$29,091** |
| **Washington State Sales Tax** | Combined State & City of Olympia sales tax (10.0% rate) | — | — | $2,909 |
| **Total Grant Request** | | | | **$32,000** |

---

### Measurable Student & Regional Workforce Outcomes

Within the first 12 months of installation, the NVIDIA DGX Spark HPC Developer Kit will deliver quantifiable educational and workforce impact across the South Puget Sound region:

1. **Direct Student Access:** Serve **120 to 160 undergraduate and graduate students annually** across interdisciplinary STEM programs in computer science, environmental studies, chemistry, biology, and data science.
2. **Open-Source Curriculum & Capstone Output:** Support at least **six interdisciplinary academic programs** and **25+ senior capstone and faculty-mentored research projects** per academic year, with student-developed workflows and documentation published openly.
3. **Cost Avoidance & Equitable Access:** Eliminate an estimated **$15,000–$25,000 per year** in equivalent commercial cloud GPU rental costs, ensuring first-generation, Pell-eligible, and rural Washington students gain hands-on experience with production CUDA and multi-node AI infrastructure regardless of personal hardware budgets.
