## **Cropchain Final Project**

**AI-Driven Multi-Agent Waterfall Planning System**

This project simulates a complete **Waterfall Software Development Lifecycle (SDLC)** using a **multi-agent AI system** powered by AutoGen and the `gpt-4o-mini` model.
Each phase of the SDLC is executed by specialized AI agents that collaborate sequentially to generate structured project planning outputs.

---

## **Project Overview**

Cropchain is an intelligent farm-to-table supply chain system designed to connect farmers, restaurants, and grocery stores through:

* Predictive crop yield analytics
* Fair pricing optimization
* Real-time logistics tracking
* End-to-end supply chain visibility

The system demonstrates how AI agents can automate and coordinate software project planning across all SDLC phases.

---

## **Team Workflow**

The project is divided into three experiments, each representing a stage in the Waterfall model:

### **Experiment 1: Requirements Phase (Team Lead-Adiba Akter)**

Agents:

* Customer Proxy
* Project Manager
* Requirements Engineer

Focus:

* Define problem scope
* Generate use cases and requirements
* Estimate effort and productivity

---

### **Experiment 2: Design & Implementation (Team Member 2 - Shai Sunnuma)**

Agents:

* System Engineer
* Software Engineer

Focus:

* Translate requirements into system architecture
* Define components, APIs, and modules
* Plan implementation strategy

---

### **Experiment 3: Testing & Documentation (Team Member 3 - Jaime Blanco)**

Agents:

* Test Engineer
* Documentation Engineer

Focus:

* Generate structured test cases
* Validate system consistency
* Produce full technical and user documentation
* Perform comparative analysis across experiments

---

## **Shared Environment Setup**

To ensure consistency across all experiments, all team members must use:

* The same virtual environment (`.venv`)
* The same dependencies (`requirements.txt`)
* The same environment variables (`.env`)
* The same model configuration: `gpt-4o-mini`

This guarantees reproducibility and consistent outputs across all phases.

---

## **Project Structure**

```id="syd23k"
src/
 ├── outputs/
 │    ├── experiment_1/
 │    ├── experiment_2/
 │    └── experiment_3/
```

Each folder contains the generated outputs corresponding to its respective SDLC phase.

---

## **Key Highlights**

* Multi-agent simulation of real-world SDLC roles
* Structured Waterfall workflow across all phases
* Clear traceability from requirements to final documentation
* AI-driven automation of planning, design, and validation

---

## **Conclusion**

This project demonstrates how AI agents can effectively model and automate the software planning lifecycle using the Waterfall approach. The system highlights the potential of GenAI in improving productivity, structure, and coordination in software engineering workflows.


## Section 12: Git Branch Strategy

Run the following commands in your terminal to set up the three-branch structure.

**Branch layout:**
- `main` — original Phase 1 code (preserved, untouched)
- `phase1-backup` — safety copy of Phase 1 
- `phase2` — active working branch for Phase 2

```bash
# 1. Make sure you are on main and everything is committed
git checkout main
git status   # should be clean

# 2. Create a safety backup of Phase 1
git checkout -b phase1-backup
git push -u origin phase1-backup

# 3. Go back to main and create the Phase 2 working branch
git checkout main
git checkout -b phase2
git push -u origin phase2

# 4. From now on, all Phase 2 work is committed to the phase2 branch
# Add your Phase 2 notebooks:
git add 04_Cropchain_Phase2_Setup_and_Experiment1_Scrum.ipynb
git commit -m "Phase 2 Exp 1: Team Lead - Scrum setup, Product Backlog, Sprint 1 Plan"
git push origin phase2
```

> **Result:** You will have 3 branches total — `main`, `phase1-backup`, `phase2`.  
> `main` and `phase1-backup` are both safe copies of Phase 1.  
> `phase2` is where all Phase 2 development happens.