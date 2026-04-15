# Reliability and Safety Analysis of a Redundant Avionic System

This project presents a comprehensive safety analysis of a redundant flight control system using advanced formal methods. The study focuses on a 2-out-of-3 (2oo3) architecture, evaluating its availability and safety properties under various fault scenarios.

## 🛠 Project Scope
The analysis is divided into two main formal approaches:
1. **Probabilistic Modeling (GSPN):** Using Generalized Stochastic Petri Nets to model the evolution of 3 independent channels (Functioning, Detected Fault, Undetected Fault) and calculate system availability over time.
2. **Formal Verification (Model Checking):** Using CTL (Computation Tree Logic) to verify critical safety properties, ensuring the system never reaches a hazardous state without proper detection.

## 📈 Key Features
* **Fault Tolerance:** Evaluation of the "2-out-of-3" logic where the system remains safe if at least two channels are operational.
* **Coverage Analysis:** Impact of the fault detection probability ($c$) on the overall system safety.
* **State Classification:** Dynamic classification of the system into *Safe*, *Risk*, or *Dangerous* states based on real-time channel health.

## 🧪 Verified Properties (CTL)
* **Safety Persistence:** "If all channels start functioning, it is possible to remain in a safe state indefinitely."
* **Hazard Detection:** "Any transition to a degraded state must be correctly identified by the arbiter to avoid dangerous conditions."

## 📄 Repository Contents
* `Safety_Critical_System_Exam.pdf`: Full technical report in English.
* `Prova_di_esame_SCS.pdf`: Original exam specifications and Italian documentation.
* `Exercise1_Project`: Model files and simulation scripts.
* `Figures & Video`: Visual demonstrations and architectural diagrams.

---
*Developed for the "Safety Critical Systems" course at the University of Naples Federico II.*
