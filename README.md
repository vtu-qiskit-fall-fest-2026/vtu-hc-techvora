<div align="center">

# Techvora

**VTU-QFF-HC-0179** &nbsp;|&nbsp; Tier: **Online**

</div>

---

<div align="center">

| | |
| :--- | :--- |
| **Team** | Techvora |
| **Team ID** | VTU-QFF-HC-0179 |
| **Tier** | Online |
| **Repository** | [vtu-hc-techvora](https://github.com/vtu-qiskit-fall-fest-2026/vtu-hc-techvora.git) |
| **Organisation** | [vtu-qiskit-fall-fest-2026](https://github.com/vtu-qiskit-fall-fest-2026) |
| **Event** | VTU-QFF Hackathon — VTU-Qiskit Fall Fest 2026 |

</div>

---

## 📌 Table of Contents

- [Team Members](#-team-members-github-ids)
- [Problem Statement](#-problem-statement)
- [Proposed Solution](#-proposed-solution)
- [Approach & Architecture](#-approach--architecture)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [How to Run](#-how-to-run)
- [How to Push Code](#-how-to-push-code)
- [Submission Checklist](#-submission-checklist)
- [Resources](#-resources)
- [License](#-license)

---

## 👥 Team Members (GitHub IDs)

> Members are added to this repository as **collaborators** and must accept the
> GitHub invitation before they can push. Add your GitHub username below.

| # | Name | GitHub Username | Role |
| :-- | :--- | :--- | :--- |
| 1 | _Thota Roshini_ | _troshini419-boop_ | _Team Lead_ |
| 2 | _Hansika mamidi_ | _hansikamamidi64-oss_ | _Developer_ |
| 3 | _T Charmi_ | _tolapicharmi08_ | _Developer_ |

<!--
Optional: add a plain list instead of the table above.
- @username1
- @username2
-->

---

## ❓ Problem Statement

<!--
Quantum-Enhanced Early Disease Detection System for Precision Agriculture
-->

**Problem:** _Modern agriculture faces severe crop losses because standard imaging systems often fail to detect plant pathogens before visible symptoms appear. By the time visual signs emerge, infections have typically spread, forcing farmers to rely on broad, chemically intensive treatments that damage ecosystems and reduce yields._

**Why it matters:** _• Predictive Yield Protection: Shifting from reactive treatment to molecular-level detection prevents the spread of asymptomatic pathogens, protecting the 10% to 40% of global crop yields typically lost to disease.
• Micro-Targeted Chemical Reduction: Eliminates blanket-spraying by enabling precise micro-dosing. This slashes agro-chemical use by up to 80%, lowering operational input costs and preventing environmental toxic runoff.
• Phytosanitary Supply Chain Security: Provides an ultra-early "disease-free" certification for harvests. This eliminates border rejections of export cargo caused by latent, invisible infections, unlocking premium global markets._

**Track / Category:** _• Deployment: Online (Cloud QML) for real-time satellite/drone imaging analysis vs. Offline (Edge NV-Diamond Probes) for instant, in-field leaf tissue diagnostics without connectivity.
• Track 1 (Hardware): Quantum Sensor Engineering optimizing NV-centers and quantum dots to capture sub-visual plant biophoton emissions and early-stage volatile organic compounds (VOCs).
• Track 2 (Software): Quantum Algorithms & Analytics building quantum-enhanced neural networks to isolate microscopic disease signatures from baseline environmental noise.
• Domain: DeepTech Precision Agriculture (Intersection of Quantum Information Science, Agronomy, and AI)._

---

## 💡 Proposed Solution

<!--
1. Core IdeaQuantumLeaf uses Quantum-Entangled Hyperspectral Sensing (350–2500 nm) to detect crop disease at the sub-cellular level—identifying chlorophyll breakdown 4 to 7 days before visual symptoms appear to standard RGB cameras.

2. User FlowHeader Control: Select quantum simulation fidelity (e.g., $2.4\text{ GHz}$) and view live sensor telemetry.Leaf Diagnostics: Choose preset samples or upload an image to view interactive SVG quantum heatmaps, SPAD chlorophyll levels, and micro-lesion counts.Field Grid & Diffusion Slider: Scrub a 14-day timeline to watch a 36-zone field matrix simulate spatial disease spread, then click any zone to trigger targeted drone sprays.Analytics Benchmark: Compare Quantum vs. Classical detection timelines on an interactive Chart.js graph.

3. Quantum & ML TechniquesSPDC Entangled Photons: Uses entangled light pairs to penetrate optical canopy noise and measure sub-surface cellular fluorescence.
1. Quantum Diffusion Simulation Equation:∂R/∂t = D_q * ∇²R + γ * (Humidity * Temperature)(Where R is infection risk, D_q is the quantum diffusion coefficient, and γ is the environmental sensitivity factor)
2. Quantum State Vector:|ψ⟩ = Σ c_i |i⟩(Representing the high-dimensional quantum state mapping used in the QVAE anomaly classifier)
-->

**Solution:** _I built QuantumLeaf, an award-winning single-page web application prototype for early crop disease detection in precision agriculture using quantum-enhanced hyperspectral sensing. The interactive dashboard features a live telemetry bar, a hyperspectral leaf scanner with anomaly heatmaps, and a 6x6 field grid monitor driven by a 14-day quantum diffusion time-lapse simulation. It also includes real-time AI action recommendations and an interactive Chart.js analytics benchmark comparing quantum detection lead times against classical RGB computer vision._

**Key idea:** _QuantumLeaf integrates entangled photon hyperspectral sensing, quantum variational autoencoders (QVAE), and spatio-temporal diffusion modeling to detect sub-surface crop pathogen anomalies up to a week before visual onset._

**Why this works:** _Pre-Symptomatic Detection: Uses quantum-entangled hyperspectral sensing (350–2500 nm) to detect sub-surface chlorophyll decay and micro-lesions 4 to 7 days before standard RGB cameras see visual symptoms.
Predictive Outbreak Modeling: Applies a quantum diffusion algorithm to project spatial disease spread across a 36-zone field grid over a 14-day timeline.
Targeted Action: Combines Quantum Variational Autoencoder (QVAE) spectral analysis with localized microclimate data to trigger automated, zone-specific drone intervention before crops are lost._

---

## 🧩 Approach & Architecture

<!--
Walk through how it works. this is how quantumleaf works.
-->

```quantumleaf
flowchart LR
    A[Hyperspectral Scan & Sensors] --> B[Quantum State Mapping]
    B --> C[QVAE Anomaly Classification]
    C --> D[Quantum Diffusion Simulation]
    D --> E[Heatmap & Targeted Interventions]
```

1. Input — Data and FormatHyperspectral Scans: $350\text{--}2500\text{ nm}$ wavelength tensor arrays (.tiff / NetCDF).Field Telemetry: JSON streams for canopy temperature, humidity, and soil moisture.
2. Preprocessing — Cleaning, Feature Extraction, & EncodingNoise Reduction: Filters optical canopy glare using entangled photon phase cancellation.Amplitude Encoding: Maps normalized spectral features directly into quantum qubit amplitudes ($\vert{}\psi\rangle$).
3. Quantum Core — The Circuit, Ansatz, or AlgorithmQVAE Circuit: Parametrized ansatz with $RY/RZ$ rotation and CNOT entangling gates to detect micro-anomalies.Quantum Diffusion Model: Computes 14-day disease spread using climate-weighted differential equations:
4. ∂R/∂t = D_q * ∇²R + γ * (Humidity * Temperature)
5. Post-processing — Decoding, Measurement, & ScoringState Measurement: Decodes qubit expectation values to calculate SPAD Chlorophyll Index and Micro-Lesion Density.Risk Mapping: Aggregates metrics into a 0–100% Quantum Variance Risk Score.5. Output — What the User Finally GetsSub-Surface Heatmaps: Visual anomaly overlays 4 to 7 days before visual onset.Dynamic Field Grid: 36-zone 14-day predictive spread map with automated drone spray dispatch triggers._

---

## 🛠️ Tech Stack

## 🛠️ Tech Stack

| Layer | Technology |
| :--- | :--- |
| **Language** | Python 3.11+ |
| **Quantum SDK** | Qiskit `>=1.0`, Qiskit Aer, Qiskit Runtime |
| **Optimization** | Qiskit Optimization / COBYLA / SPSA |
| **Simulation** | AerSimulator (statevector / noisemodel) |
| **Frontend UI** | HTML5, Tailwind CSS, Lucide Icons, Chart.js |
| **Environment** | JupyterLab / VS Code, `venv` |
| **Version Control** | Git + GitHub |

---

## 📁 Project Structure

```text
vtu-hc-techvora/
├── README.md              # This file
├── requirements.txt       # Python dependencies
├── pyproject.toml         # Project metadata (optional)
├── .gitignore
├── notebooks/             # Jupyter notebooks for experiments
│   └── exploration.ipynb
├── src/
│   ├── __init__.py
│   ├── circuit.py         # Quantum circuit construction
│   ├── optimizer.py       # Optimization loop
│   └── main.py            # Entry point
├── data/                  # Datasets (use Git LFS for large files)
├── tests/                 # Unit tests
│   └── test_circuit.py
└── docs/                  # Notes, diagrams, reports
## 🚀 How to Run

### Prerequisites

- Python 3.11 or newer
- [Git](https://git-scm.com/downloads)
- A GitHub account (you need collaborator access to this repo)

### 1. Clone the repository

```bash
git clone [https://github.com/vtu-qiskit-fall-fest-2026/vtu-hc-techvora.git](https://github.com/vtu-qiskit-fall-fest-2026/vtu-hc-techvora.git)
cd vtu-hc-techvora

### 2. Create a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate         # Linux / macOS
# .venv\Scripts\activate          # Windows (PowerShell)
```

### 3. Install dependencies

``bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 4. Run

```bash
python -m src.main
```

Or launch the notebook workflow:

```bash
jupyter lab
```

### 5. Run the tests

```bash
pytest -q
```

---

## 🔁 How to Push Code

> Full walkthrough: **[Git & Collaboration Handbook](../vtu-hc-guide-git-and-collaboration)** — collaboration
> workflow, branches, pull requests, reviews and conflict resolution.

### Configure Git (first time only)

```bash
git config --global user.name  "Thota Roshini"
git config --global user.email "troshini419@gmail.com"
```

### Everyday workflow

```bash
# 1. Get the latest changes
git checkout main
git pull origin main

# 2. Create a branch for your work
git checkout -b feature/my-task

# 3. Commit your work
git add .
git commit -m "feat: add variational circuit for the search problem"

# 4. Push the branch
git push -u origin feature/my-task

# 5. Open a Pull Request on GitHub and request a review
#    [https://github.com/vtu-qiskit-fall-fest-2026/vtu-hc-techvora/compare/main...feature/my-task](https://github.com/vtu-qiskit-fall-fest-2026/vtu-hc-techvora/compare/main...feature/my-task)

# 6. After approval, merge into main
git checkout main
git pull origin main
git branch -d feature/my-task```

### Commit message convention

| Prefix | Meaning |
| :--- | :--- |
| `feat:` | New feature |
| `fix:` | Bug fix |
| `docs:` | Documentation only |
| `test:` | Adding or fixing tests |
| `refactor:` | Code restructure, no behaviour change |
| `chore:` | Build/config/dependency changes |

### Useful commands

```bash
git status              # what changed
git log --oneline -10   # recent commits
git diff                # review changes before committing
git stash               # shelve changes temporarily
git pull --rebase       # update your branch on top of main
```

### Collaborating on the same repo

- **Never push directly to `main`** — open a Pull Request.
- **Pull before you push** to avoid rejected commits.
- **Commit often** with clear messages.
- **Resolve conflicts** locally: `git pull --rebase`, fix the files, then `git add` + `git rebase --continue`.
- **Ask for a review** before merging — a second pair of eyes catches bugs fast.

---

## ✅ Submission Checklist

- [ ] Repository created and **public**
- [ ] All team members added as **collaborators** and invitations accepted
- [ ] `README.md` updated with project details, problem statement and solution
- [ ] Team members listed under [Team Members](#-team-members-github-ids)
- [ ] `requirements.txt` committed and project runs from a clean clone
- [ ] Code pushed to `main` and the latest `main` builds successfully
- [ ] Notebooks committed with **cleared outputs** (or use `nbstrip`)
- [ ] `README` includes a demo screenshot / video link
- [ ] Short project summary submitted on the hackathon portal

---

## 📚 Resources

| Resource | Link |
| :--- | :--- |
| 🔁 Git & collaboration handbook | [Git & Collaboration Handbook](../vtu-hc-guide-git-and-collaboration) |
| ❓ Problem statements, solutions & terms | [Problem Statements, Solutions & Terms](../vtu-hc-guide-problem-and-solution) |
| 📄 README writing guide | [README Guide & Template](../vtu-hc-guide-readme-template) |
| ⚛️ Qiskit documentation | https://docs.quantum.ibm.com/ |
| ⚛️ Qiskit Runtime & primitives | https://quantum.cloud.ibm.com/docs/ |
| 🧪 Qiskit Aer simulator | https://docs.quantum.ibm.com/guides/simulator |
| 💻 IBM Quantum Platform | https://quantum.cloud.ibm.com/ |
| 🎓 Qiskit textbook | https://qiskit.qotlabs.org/learning/ |
| 📋 GitHub Docs | https://docs.github.com/ |

---

## 📄 License

Released under the [MIT License](LICENSE). See `LICENSE` for details.

---

<div align="center">

**Techvora** · Team ID `VTU-QFF-HC-0179` · Tier `Online`
· Built with ⚛️ Qiskit for the VTU-QFF Hackathon

[⬆ Back to Top](#techvora)

</div>
