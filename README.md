# Project Aura: State Manifest
- **Manifest Version:** 1.1
- **Project Version:** 0.1.0
- **Last Updated:** 2025-06-27T11:58:34+04:00

---

## 1. Session Summary & Objective

**Last Session Summary:**
- We established a two-phase approach for `Module-001`. Phase 1 will be a Zero-Shot classifier to establish a baseline. Phase 2 will be a fully fine-tuned model for production.
- We researched available `CLIP` models and selected `openai/clip-vit-large-patch14` as our base model for its strong performance and documentation.
- We defined and approved a detailed technical plan for implementing the Phase 1 Zero-Shot Classifier, including the core logic and API structure using FastAPI.

**Current Objective:**
- **Code Implementation:** To write the `classifier.py` and `main.py` scripts for the **Module-001 (Phase 1 - Zero-Shot Classifier)** as per the approved technical plan.

---

## 2. Current Project State

### 2.1. System Architecture
- **Status:** Defined.
- **Details:** A modular, multi-stage microservice pipeline. (Reference: Documentation v1.0).

### 2.2. MLOps & Infrastructure
- **Code Versioning:** Git
- **Data Versioning:** DVC (To be implemented)
- **Model Versioning:** MLflow / Hugging Face Hub (To be decided)
- **CI/CD:** GitHub Actions (To be implemented)
- **Monitoring:** Evidently AI / Prometheus (To be implemented)

### 2.3. Module Status

#### Module-001: Ceremony Classification
- **Status:** `Phase 1 - In Progress`
- **Purpose:** Classifies an image into a specific wedding ritual.
- **Base Model:** `openai/clip-vit-large-patch14`
- **Fine-tuned Version:** `N/A` (Scheduled for Phase 2)
- **Dataset Used:** `N/A` (Data scraping and labeling for Phase 2 is a parallel task)

---

## 3. Decision Log

| Date       | Decision                                                                          | Rationale                                                                                                    |
| :--------- | :-------------------------------------------------------------------------------- | :----------------------------------------------------------------------------------------------------------- |
| 2025-06-27 | Approved technical plan for Module-001 (Phase 1).                                 | The plan is technically sound, uses appropriate libraries, and provides a clear path to the first working module. |
| 2025-06-27 | Selected `openai/clip-vit-large-patch14` as the base model for Ceremony Classification. | Strong performance, good documentation, and ideal for both zero-shot baseline and future fine-tuning.          |
| 2025-06-27 | Adopted the "Project State Manifest" approach for context persistence.            | To ensure project continuity and resilience against loss of chat history.                                    |
| 2025-06-27 | Finalized v1.0 of the master technical documentation structure.                   | To provide a clear, production-focused blueprint for the project.                                            |
