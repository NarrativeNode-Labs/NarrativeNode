# NarrativeNode

**A Deterministic AI Orchestration Engine for Systemic Role-Playing Games.**

> *Solving the "Hallucination Problem" in Generative RPGs through a hybrid Judge-Narrator Architecture and Iterative Fine-Tuning.*

---

## 🎯 The Core Problem: Why Current AI RPGs Fail

The primary bottleneck in Generative AI gaming is **consistency**. Standard LLM-based games suffer from "hallucinations"—where the AI forgets established lore, breaks game rules, or generates illogical outcomes in favor of creative writing.

**NarrativeNode** is not just a game engine; it is a solution to the **"Creativity vs. Consistency"** dilemma. We are building a system where infinite creative freedom meets strict, rule-based logic.

## 💡 Our Solution: The "Judge-Lead" Architecture

NarrativeNode implements a proprietary multi-agent system designed to enforce logic within an open-ended world:

### 1. The "AI Judge" System (Hallucination Firewall)
Unlike traditional systems that rely solely on a creative writer agent, NarrativeNode introduces a strict **"Judge Agent."**
* **Function:** Before any AI-generated narrative reaches the player, it passes through the Judge.
* **Logic:** The Judge analyses the generated input by the **Game Rules (Engine)** and **World State**.
* **Result:** If the generated content violates a rule (e.g., an NPC using magic in a non-magic zone), the Judge rejects it and forces a regeneration. This ensures a systematic, coherent world.

### 2. Iterative Fine-Tuning Pipeline
We do not rely on "out-of-the-box" models. Our development methodology involves a continuous cycle of **Domain-Specific Fine-Tuning**:
* Models are trained specifically on our custom datasets to understand not just "how to write," but "how to adhere to game mechanics."
* Every development phase contributes new data to refine the model's adherence to the project's unique constraints.

### 3. Constrained Player-Driven Generation
Players are empowered to shape the world using Generative AI, but strictly within the engine's boundaries.
* **Dynamic Assets:** Whether generating unique items, locations, or lore, the engine applies "Style & Logic Wrappers" to ensure player creations fit the game's tone and balance.
* **Rule Compliance:** A player can request anything, but the engine only generates what is *possible* within the simulation's logic.

---

## 🔧 Tech Stack & Architecture

* **Orchestration:** Python-based Multi-Agent System (Narrator, Judge, World Manager).
* **Logic Core:** Graph Theory for non-Euclidean location tracking (Mapless Navigation).
* **AI Integration:** Custom Fine-Tuned adapters for Claude 3.5 Sonnet / Gemini Pro.
* **Client:** Godot Engine (4.x) for UI and Visual Feedback.

## 🗺 Roadmap

- [x] **Phase 1: Proof of Concept:** Implementing the "Judge" agent logic to filter LLM hallucinations.
- [ ] **Phase 2: Fine-Tuning:** Training smaller models (SLMs) for cost-effective rule enforcement.
- [ ] **Phase 3: Cloud Infrastructure:** Deploying the multi-agent swarm on AWS/GCP for scalable inference.
- [ ] **Phase 4: Alpha Release:** Opening the "Systemic RPG" to early testers.

## 🤝 Contact & Collaboration

**NarrativeNode** is aiming to set a new standard for reliability in AI-generated media.

📧 **Contact:** narrativenode.labs@gmail.com
