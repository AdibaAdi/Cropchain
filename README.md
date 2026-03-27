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


