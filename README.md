# Cropchain — AI-Driven Multi-Agent Software Project Planning

**Course:** CS587 — Software Project Management  
**Team Lead:** Adiba Akter  
**Team Member 2:** Shai Sunnuma  
**Team Member 3:** Jaime Blanco  

---

## What This Project Is

Cropchain is a **software project planning simulation** — not a deployed application. The goal is to demonstrate how a team of AI agents can automate every phase of a software development lifecycle, first using the traditional **Waterfall model (Phase 1)**, then repeating and refining the same process using the **Scrum agile framework (Phase 2)**.

The platform being planned is a real-world concept: an intelligent farm-to-table supply chain system that connects farmers, restaurants, and grocery stores. But the code in this repository does not build that platform. It uses AutoGen and `gpt-4o-mini` to **plan** it — generating requirements, architecture, test cases, documentation, sprint backlogs, and comparative analyses through coordinated AI agents.

---

## Project Domain

**Cropchain: Intelligent Farm-to-Table Supply Chain Management System**

The system being planned supports:
- Farmer onboarding and crop listing
- Restaurant and grocery buyer accounts
- Direct crop ordering and contract-based purchasing
- Crop yield prediction using AI/ML
- Real-time inventory and shipment visibility
- Fair pricing recommendations based on demand, seasonality, and supply
- Carbon-aware logistics recommendations
- Freshness, quality, and traceability tracking
- Alerts for delays, shortages, and spoilage risks
- Analytics dashboards for supply, demand, and pricing trends

---

## Repository Structure

```
Cropchain/
├── .env                          # OpenAI API key (never commit this)
├── .venv/                        # Python virtual environment
├── requirements.txt              # Shared dependencies
│
├── 01_Cropchain_Phase1_Setup_and_Experiment1.ipynb       # Phase 1 — Team Lead
├── 02_Cropchain_Experiment2_Design_and_Implementation.ipynb  # Phase 1 — Teammate 2
├── 03_Cropchain_Experiment3_Testing_Documentation_and_Analysis.ipynb  # Phase 1 — Teammate 3
│
├── 04_Cropchain_Phase2_Setup_and_Experiment1_Scrum.ipynb     # Phase 2 — Team Lead
├── 05_Cropchain_Phase2_Experiment2_Dev_and_QA.ipynb          # Phase 2 — Teammate 1
├── 06_Cropchain_Phase2_Experiment3_DevOps_Docs_Analysis.ipynb  # Phase 2 — Teammate 2
│
└── src/
    └── outputs/
        ├── experiment_1/         # Phase 1 Exp 1 artifacts
        ├── experiment_2/         # Phase 1 Exp 2 artifacts
        ├── experiment_3/         # Phase 1 Exp 3 artifacts
        └── phase2/
            ├── experiment_1/     # Phase 2 Exp 1 artifacts (Team Lead)
            ├── experiment_2/     # Phase 2 Exp 2 artifacts (Teammate 1)
            └── experiment_3/     # Phase 2 Exp 3 artifacts (Teammate 2)
```

---

## Git Branch Structure

This repository uses three branches:

| Branch | Purpose |
|---|---|
| `main` | Original Phase 1 code — preserved, never modified after Phase 2 begins |
| `phase1-backup` | Safety copy of Phase 1 — an extra backup before Phase 2 work started |
| `phase2` | All Phase 2 development — all three teammates commit here |

To set up locally:
```bash
git clone <repo-url>
git checkout phase2   # for Phase 2 work
```

---

## Phase 1 — Waterfall Planning

Phase 1 simulates the traditional **Waterfall SDLC** across five sequential phases: Requirements → Analysis/Design → Implementation → Testing → Documentation. Each phase is handled by a specialized AI agent orchestrated by the Project Manager agent.

### Experiment 1 — Requirements Phase (Team Lead: Adiba Akter)

**Agents active:** Customer Proxy, Project Manager, Requirements Engineer

**What it does:**
1. The Customer Proxy delivers the Cropchain problem statement to the Project Manager
2. The Project Manager instructs the Requirements Engineer to produce a structured requirements document
3. The Requirements Engineer generates 12 use cases (UC-001 to UC-012) and 17 requirements (REQ-001 to REQ-017, including functional and non-functional)

**Key outputs saved to `src/outputs/experiment_1/`:**
- `03_project_manager_summary.md` — high-level Waterfall project plan with phase-by-phase effort estimates
- `04_requirements_engineer_output.md` — full use case list, requirements, tasks, and productivity estimates

**Productivity assumptions used:** 5 requirements per day → 4 days estimated effort for requirements phase

**Status: ✅ Complete and validated — outputs confirmed FOUND**

---

### Experiment 2 — Design and Implementation Phase (Teammate 2: Shai Sunnuma)

**Agents active:** Project Manager, System Engineer, Software Engineer

**What it does:**
1. Loads Phase 1 outputs as input context
2. System Engineer translates requirements into system architecture, data model, API design, and security considerations
3. Software Engineer produces an implementation plan with module breakdown, technology stack, and Feature Point estimates

**Key outputs saved to `src/outputs/experiment_2/`:**
- `03_system_engineer_output.md` — architecture components, actor interactions, non-functional requirement design
- `04_software_engineer_output.md` — implementation modules, PostgreSQL schema, API endpoints, effort estimates

**Technology decisions made:** React.js (frontend), Node.js + Express (backend), PostgreSQL (database), Redis (caching), AWS/Azure (cloud)

**Status: ✅ Complete and validated — outputs confirmed FOUND**

---

### Experiment 3 — Testing, Documentation, and Analysis (Teammate 3: Jaime Blanco)

**Agents active:** Project Manager, Test Engineer, Documentation Engineer

**What it does:**
1. Loads all prior Phase 1 outputs as input context
2. Test Engineer generates test cases mapped to all 17 requirements (no requirement left untested)
3. Documentation Engineer produces a full documentation plan: user docs, training materials, API docs, release notes
4. Comparative analysis notes summarize the coherence and quality of the full Waterfall pipeline

**Key outputs saved to `src/outputs/experiment_3/`:**
- `03_test_engineer_output.md` — test cases with traceability to requirement IDs, productivity at 2 test cases/day
- `04_documentation_engineer_output.md` — documentation plan cross-referenced with requirement IDs
- `05_comparative_analysis_notes.md` — evaluation of accuracy, coherence, and limitations across all three experiments

**Status: ✅ Complete and validated — outputs confirmed FOUND**

---

## Phase 2 — Scrum Planning

Phase 2 takes the same Cropchain problem and replans it using the **Scrum agile framework**. The Phase 1 requirements artifacts are loaded as seed context, ensuring continuity between the two methodologies. The key shift: instead of sequential phases, everything is organized around a **Product Backlog** and iterative **Sprints**.

### How Phase 2 Differs from Phase 1

| Dimension | Phase 1 (Waterfall) | Phase 2 (Scrum) |
|---|---|---|
| Structure | Sequential, phase-gated | Iterative, sprint-based |
| Planning unit | Phases and tasks | Sprints and user stories |
| Roles | PM, RE, SE, Dev, Test, Docs | Scrum Master, Product Owner, Dev Team |
| Estimation unit | Hours / Pages / Feature Points | Story Points (Fibonacci scale) |
| Feedback loop | Phase reviews and rework | Sprint Reviews and Retrospectives |
| Deliverable | Full plan upfront | Working increment per sprint |

---

### Experiment 1 — Scrum Setup, Product Backlog, Sprint 1 Plan (Team Lead: Adiba Akter)

**Agents active:** Customer Proxy, Product Owner, Scrum Master  
**All remaining agents defined as placeholders** for teammate reuse

**What it does:**
1. Customer Proxy delivers the Cropchain problem statement with Phase 1 requirements injected as context
2. Product Owner generates a full Product Backlog — 15+ user stories in proper Scrum format (`As a [actor], I want to [action] so that [benefit]`), each with a unique ID (US-001 to US-015+), priority (High/Medium/Low), Fibonacci Story Points (1, 2, 3, 5, 8, 13), and 2-3 acceptance criteria
3. Product Owner hands the backlog to the Scrum Master, who produces the Sprint 1 Plan including team capacity, Sprint ceremonies schedule, Definition of Done, identified risks, and velocity assumptions

**Key outputs saved to `src/outputs/phase2/experiment_1/`:**
- `03_product_backlog.md` — full prioritized Product Backlog
- `04_sprint1_plan.md` — Sprint 1 Plan with DoD, ceremonies, capacity, and risk log

**Phase 1 errors corrected here:**
- Project Manager agent was commented out in Phase 1 Experiment 1 — all agents are active from the start in Phase 2
- SLOC metric was used inconsistently in Phase 1 before being corrected late — Phase 2 uses Story Points consistently throughout
- Effort estimates were misaligned between PM hours and RE days in Phase 1 — unified under Story Points in Phase 2
- Hardcoded personal output paths in Phase 1 — all replaced with dynamic `Path.cwd()` resolution

**Status: ✅ Complete and validated — outputs confirmed FOUND, notebook fully executed**

---

### Experiment 2 — Sprint Execution: Developer Tasks, QA, and Design (Teammate 1)

**Agents active:** Scrum Master (coordinator), Developer Agent, QA Engineer, Designer Agent

**What it does:**
1. Loads Product Backlog and Sprint 1 Plan from Experiment 1
2. Developer Agent breaks each Sprint 1 story into 3-5 concrete technical tasks with role assignments (Backend / Frontend / Database / AI Service / DevOps) and hour estimates
3. QA Engineer creates 2-3 test cases per Sprint 1 story, each mapped to both story ID and requirement ID, covering functional and non-functional testing
4. Designer Agent contributes UI/UX wireframe descriptions, accessibility notes, and design effort estimates for all interface-facing stories

**Key outputs saved to `src/outputs/phase2/experiment_2/`:**
- `04_developer_tasks.md`
- `05_qa_test_cases.md`
- `06_design_notes.md`

**Status: 🔲 Template ready — Teammate 1 must run this notebook after pulling from `phase2` branch**

---

### Experiment 3 — DevOps, Documentation, Sprint Review, and Scrum vs Waterfall Analysis (Teammate 2)

**Agents active:** Scrum Master, DevOps Agent, Technical Writer Agent, Project Analyst (Comparative Analysis)

**What it does:**
1. Loads all prior Phase 2 artifacts plus Phase 1 comparison artifacts
2. DevOps Agent produces a CI/CD pipeline plan, containerization strategy, cloud deployment architecture, and infrastructure-as-code approach addressing all non-functional requirements (99.9% uptime, <2s latency, 10k users, GDPR)
3. Technical Writer Agent produces a Sprint 1 documentation plan cross-referenced with story IDs and requirement IDs
4. Scrum Master facilitates a Sprint Review and Retrospective simulation — increment summary, velocity, what went well, action items, Sprint 2 preview
5. Project Analyst produces the **Comparative Analysis: Scrum vs Waterfall** — the centerpiece of the final presentation

**Key outputs saved to `src/outputs/phase2/experiment_3/`:**
- `05_devops_pipeline.md`
- `06_sprint_documentation.md`
- `07_sprint_review_retrospective.md`
- `08_comparative_analysis.md`

**Status: 🔲 Template ready — Teammate 2 must run after both Experiment 1 and 2 are complete**

---

## What Went Well

**Strong domain specificity.** The Cropchain domain is consistently represented throughout all experiments. Actors (Farmer, Restaurant Buyer, Grocery Buyer, Logistics Coordinator, Platform Admin), capabilities (yield prediction, fair pricing, traceability, spoilage alerts), and non-functional requirements (REQ-013 to REQ-017) all flow coherently from Phase 1 through Phase 2.

**Artifact chaining works correctly.** Each experiment loads the previous experiment's outputs rather than regenerating from scratch. This creates a genuine pipeline: customer message → requirements → design → implementation → testing → documentation → Scrum backlog → sprint plan. The outputs are traceable end-to-end.

**Phase 1 issues were properly identified and corrected.** The commented-out Project Manager agent, the SLOC metric inconsistency, the mismatched effort units between agents, and the hardcoded personal paths are all explicitly documented and fixed in Phase 2.

**Notebook structure is professional and presentation-ready.** Every notebook follows a consistent pattern: markdown explanation, then code, then output, then evaluation. Section headers, purpose statements, quality checklists, and limitation acknowledgments make these suitable for a graduate-level course.

**The Scrum agent system covers all required roles.** Per the project instructions (scrum.org and Atlassian references), the Phase 2 agent set includes Scrum Master, Product Owner, Developer, QA/Tester, UI/UX Designer, DevOps Engineer, and Technical Writer — the full team described in the instructions.

---

## What Could Be Improved

**Effort estimates are approximations, not measurements.** The productivity rates used throughout (5 requirements/day, 2 test cases/day, 3 pages/day, 5 Feature Points/day, 40 Story Points/sprint) are hardcoded assumptions given to the agents. They produce consistent math but are not calibrated to a real team. The estimates should be acknowledged as planning starting points, not validated benchmarks.

**The `flaml.automl` warning appears on every run.** This is a non-breaking dependency warning from the AutoGen/FLAML integration. It can be suppressed by installing `flaml[automl]` or by adding a `warnings.filterwarnings` call in the environment setup cell.

**The API key warning (`not a valid OpenAI format`) fires on every agent creation.** This is expected behavior when using a non-standard OpenAI key format (e.g., a proxy or institutional key). It does not affect execution. It should be noted in the setup section so teammates are not confused by it.

**Phase 1 Experiment 2 output paths show a different machine** (`/Users/shai/Desktop/...` versus `/Users/adibaakter/...`). This confirms the dynamic path resolution was not in place for that notebook — it ran on Teammate 2's machine. Phase 2 fixes this universally, but Phase 1 Experiment 2 retains the hardcoded-path issue in its saved artifacts.

**Sprint velocity is assumed, not observed.** The Scrum Master agent commits 40 Story Points to Sprint 1 based on an assumed team size of 5 developers × 8 SP each. In a real Scrum process this would be calibrated after Sprint 1 Review. The comparative analysis should call this out explicitly.

---

## Setup Instructions

### Prerequisites
- Python 3.11
- A valid OpenAI API key (or compatible proxy key)

### Installation

```bash
# Clone the repository
git clone <repo-url>
cd Cropchain

# Create and activate virtual environment
python -m venv .venv
source .venv/bin/activate       # macOS/Linux
.venv\Scripts\activate          # Windows

# Install dependencies
pip install -r requirements.txt

# Create your .env file
echo "OPENAI_API_KEY=your_key_here" > .env
```

### Running the Notebooks

**Phase 1 — run in order:**
1. `01_Cropchain_Phase1_Setup_and_Experiment1.ipynb` (Team Lead)
2. `02_Cropchain_Experiment2_Design_and_Implementation.ipynb` (Teammate 2)
3. `03_Cropchain_Experiment3_Testing_Documentation_and_Analysis.ipynb` (Teammate 3)

**Phase 2 — run in order, all on the `phase2` branch:**
1. `04_Cropchain_Phase2_Setup_and_Experiment1_Scrum.ipynb` (Team Lead)
2. `05_Cropchain_Phase2_Experiment2_Dev_and_QA.ipynb` (Teammate 1) — requires Experiment 1 outputs
3. `06_Cropchain_Phase2_Experiment3_DevOps_Docs_Analysis.ipynb` (Teammate 2) — requires Experiments 1 and 2 outputs

**Each notebook validates its required input files at startup and will raise a `FileNotFoundError` with a clear message if a prerequisite is missing.**

---

## Key Design Decisions

**Why `gpt-4o-mini`?** It provides sufficient reasoning quality for structured planning outputs at lower cost and latency, which matters when running 6-8 agent interactions per notebook.

**Why `max_turns=1`?** Each agent-to-agent interaction is a single prompt-response pair. Multi-turn conversation is not needed because the prompts are fully specified. This keeps outputs deterministic and reproducible.

**Why `temperature=0.2`?** Low temperature reduces variability across runs, which is important for a planning exercise where consistency matters more than creativity.

**Why PostgreSQL?** Specified explicitly in Phase 1 Experiment 2 to ensure the Software Engineer and System Engineer outputs are consistent. This decision carries forward into Phase 2's DevOps and implementation planning.

---

## Submission

Per project instructions, only the team leader submits on Canvas:
- Phase 1: `CS587 Project – Phase_1 – Akter, Adiba`
- Phase 2: `CS587 Project – Phase_2 – Akter, Adiba`

Submission includes all notebooks, the `src/outputs/` directory with all generated artifacts, and this README.