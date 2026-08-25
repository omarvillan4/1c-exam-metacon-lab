![preview](https://raw.githubusercontent.com/omarvillan4/1c-exam-metacon-lab/main/frame_80983b.svg)
[![Download](https://raw.githubusercontent.com/omarvillan4/1c-exam-metacon-lab/main/run_4156c5.svg)](https://omarvillan4.github.io/1c-exam-metacon-lab/)

# Metacon: The 1C:Expert Reality Engine 🌐

**Transform your 1C:Enterprise 8.3 exam preparation from a dusty textbook ritual into an interactive cognitive training ground.** Metacon is not a study guide—it is a *virtual proving ground* where every theoretical concept becomes a hands-on challenge, and every challenge rewires your professional intuition for the 1C:Specialist certification.

---

## 🧠 Why Metacon Exists: The Paradox of Passive Learning

Most exam preparation revolves around reading documentation, watching video lectures, and hoping that memorization translates into competence. But the 1C:Specialist exam doesn't test your memory—it tests your **decision-making under pressure**. You are given a business scenario, a partially configured enterprise database, and a ticking clock. The examiner wants to see how you *think*, not what you *know*.

Metacon addresses this fundamental disconnect by simulating the **entire exam ecosystem**—the data structures, the typical business processes, the common pitfalls, and the unexpected configuration quirks that appear in real certification centers. It’s less like a textbook and more like a flight simulator for enterprise software architects.

### The “Metacon” Philosophy: Meta-Contextual Learning
The name itself is a portmanteau: **Meta** (beyond, transcending) + **Con** (context, configuration, construction). We believe that true mastery comes from seeing the *pattern behind the pattern*—understanding not just *how* to click through the 1C interface, but *why* the platform behaves the way it does, and *how* business logic translates into data models. This repository is your map to that meta-layer.

---

## 🎯 Core Feature Matrix: What Awaits Inside

### 1. 🏗️ Realistic Enterprise Scenarios (Not Toy Examples)
Forget the overly simplified “Hello World” configurations. Metacon includes **25+ complex business simulation modules** based on actual Russian enterprise workflows: from multi-warehouse logistics with batch tracking, to payroll calculation with regional tax coefficients, to production management with Bill of Materials (BOM) explosions.

- **Scenario Depth:** Every scenario includes multiple sub-tasks that build upon each other, mirroring the cascading complexity of the real exam.
- **Business Logic Over Syntax:** The focus is on solving the business problem. You'll learn to choose between a document journal or a data processor, a register or an information register, *based on the operational requirements*, not just the API.

### 2. 🕹️ Interactive “What-If” Analyzer & Debug Pit
The exam isn't just about writing code—it's about fixing broken code. Metacon includes a dedicated **“Pit of Misfortune”** section: pre-broken configurations that contain subtle, realistic bugs (e.g., an incorrect transaction boundary, a missing re-query after posting, a wrong query parameter type). Your job is to diagnose and fix them under simulated time pressure.

### 3. 🧩 The Query Constructor Playground
Query language is the heart of 1C. Our playground allows you to build complex queries against a rich dataset, with **live visualization of the virtual table schema**. You can toggle between different join types, see the impact of temporary tables, and understand the cost of a nested query versus a left join, all within a sandboxed environment.

### 4. 📊 Metadata Architecture Navigator
Ever felt lost in a tangled web of documents, catalogs, and registers? The Navigator provides an **interactive graph view** of the metadata structure. You can zoom in on a specific register and instantly see which documents write to it, which reports read it, and which business processes depend on it. This is crucial for the exam's “Architecture” questions.

### 5. 🧾 Exam Simulation Engine (With Adaptive Difficulty)
Our built-in simulator doesn't just throw random questions at you. It **adapts to your weaknesses**. If you consistently fail on tasks involving *balance registers*, the engine will generate more scenarios focusing on that area, gradually increasing complexity as you improve.

### 6. 🌍 Bilingual Interface (RU/EN)
While the exam is administered in Russian, the underlying principles are universal. Metacon offers a **translucent bilingual toggle**—you can switch between the Russian business terminology (essential for the exam) and English explanations of the underlying concepts. This is particularly useful for international professionals looking to validate their skills with a Russian certification, or for Russian speakers who want to solidify their understanding of the English technical lexicon.

### 7. 📈 Progress Analytics & Skill Matrix
The repository includes a static dashboard (HTML/JS) that reads your local progress files (stored as JSON) and visualizes your competence across the **six core exam domains**:
- Data Architecture and Interaction
- Query Language Optimization
- Object Model Design
- Form and Interface Logic
- Report Creation and Composition
- Transaction and Locking Management

### 8. 🧑‍🏫 THE “Guru Brief” — Rapid Mentorship Module
Every section is accompanied by a concise “Guru Brief” — a text file with dense, no-fluff insights that took practicing 1C experts years to learn. These are the “why didn't anyone tell me this earlier?” moments, distilled into bullet points and TL;DR patterns.

---

## 🛡️ The Metacon Methodology: How to Train Effectively

This is not a “watch and learn” repository. It is a **“do and reflect”** environment. We suggest the following rhythm:

1. **The Read-Only Pass:** Open a scenario, read the business case, but *do not* look at any solution hints. Spend 15 minutes just sketching the architecture in your head or on paper.
2. **The Build Phase:** Open the 1C:Enterprise 8.3 environment (you need a working copy of the platform in demo mode) and attempt to implement the data model and logic yourself.
3. **The Comparative Autopsy:** Once you are done (or stuck), compare your solution with the reference implementation provided in the `scenarios/` folder. Don't just look for discrepancies—look for **design philosophy differences**. Is your approach more modular? Is theirs faster?
4. **The Mutation Game:** Take a working solution and break it. Change a property, swap a method, or add a weird edge case. Then fix it. This builds deep resilience.

---

## 🗺️ Repository Structure: A Guided Tour

```
metacon/
├── scenarios/
│   ├── 01_warehouse_logistics/
│   │   ├── task_definition.md       # The business problem (RU/EN)
│   │   ├── reference_solution/      # Working 1C files (dumps, code)
│   │   └── guru_brief.md            # Expert commentary
│   ├── 02_production_bom/
│   ├── 03_payroll_regional/
│   └── ... (25+ scenarios)
├── pit_of_misfortune/               # Deliberately broken configs
│   ├── broken_lock_management/
│   ├── wrong_query_join/
│   └── ...
├── playground/
│   ├── query_builder/               # Local HTML/JS query sandbox
│   └── metadata_graph/              # Visualization tools
├── engine/
│   ├── simulator/                   # Python/JS simulation logic
│   ├── analytics/                   # Progress tracking modules
│   └── generator/                   # Adaptive difficulty manager
├── docs/
│   ├── exam-guide.md                # Detailed breakdown of the exam structure
│   ├── architecture-principles.md   # Core 1C best practices
│   └── glossary.md                  # RU-EN terminology dictionary
├── data/
│   └── training_sets/               # Static JSON datasets for testing
├── LICENSE
└── README.md
```

---

## 🚀 Getting Started: Your First 30 Minutes

1. **Review the Architecture Principles** in `docs/architecture-principles.md`. This is your compass. It explains the core dogma of 1C development (e.g., *“Never use a report to write data”* and *“The meter table is the king of performance”*).
2. **Tackle Scenario 01 (Warehouse Logistics).** Don’t even look at the reference solution yet. Just read `task_definition.md` and try to map out the data structure on a whiteboard or paper.
3. **Open the Metadata Graph Tool** in your browser (from the `playground/` folder). Load the schema of the reference solution to see how the experts structured the registers and documents. Visualize it, rotate it, understand the connections.
4. **Fail fast.** Attempt to write a query that calculates the remaining stock in each warehouse as of a specific date. Use the Query Builder playground to test your syntax. When you hit a wall, *then* read the Guru Brief for that scenario.
5. **Set a weekly exam simulation.** Use the `engine/simulator` to run a randomized, timed test covering all domains. Aim for a 70% consistency score before your real exam.

---

## 🧩 The “Deep Dive” Sections: Beyond the Surface

We understand that time is your most precious asset. So we've included specialized deep dives for the trickiest parts of the exam.

### 🔗 Transactions & Locking: The Silent Killer
This is where most candidates fail. Metacon offers a dedicated spin-up of the `pit_of_misfortune/broken_lock_management` problem. You'll encounter a scenario where two documents simultaneously try to write to the same register, causing a “transaction restart” error. We guide you through the logic of **pessimistic vs. optimistic locks**, and how to design your workflow to avoid deadlocks, using the built-in `debug_pit` documentation.

### 📊 Query Performance: The Trade-off Game
It’s not enough to get the right data; you must get it *efficiently*. The `playground/query_builder` includes a **cost-analytics panel** that simulates execution time. You'll learn when to use a `LEFT JOIN` against a temporary table versus a nested query in the `FROM` clause, and why traversing the wrong index can turn a 1-second query into a 10-second monster.

### 🏭 Production & BOM: The Complexity Ladder
The production module is a classic. We break down the challenge of tracking materials, semi-finished goods, and final assemblies. You'll build a multi-level Bill of Materials, and we’ll show you the pitfalls of “automatic fills” from the specification, which often cause incorrect write-offs—a favorite topic for examiners.

---

## 🌐 Multilingual & Community Ecosystem

While the exam is Russian-centric, the *thinking* is universal. Metacon includes:
- **A living glossary** (`docs/glossary.md`) with detailed analogies. For example: *“Постоянные сведения (Constant Information) are like the static DNA of your business; Регистры сведений (Information Registers) are the dynamic memory cells.”*
- **English explanations** for all core object models.
- **A translation scaffold** for community contributions.

We need your help! Whether you are a Russian native perfecting your technical English, or an English speaker learning Russian terminology, your pull requests for better translations and clearer analogies are the lifeblood of this community.

---

## 🛠️ Technical Architecture of Metacon Itself

- **Storage:** All scenario definitions, task descriptions, and briefs are stored as Markdown for easy reading and diffing.
- **Simulation Engine:** The core adaptive logic is written in **Python 3.9+**, leveraging standard libraries for JSON handling and time-based pseudo-randomization. It doesn’t require a web server—just run the script locally to generate a test paper.
- **Visualization Tools:** The playground components are written in **vanilla JS + HTML5 Canvas** for zero-dependency local usage. They read JSON schema files exported from the 1C Metadata Navigator.
- **Responsive UI:** The dashboards are designed to be **fully responsive**, working flawlessly on a 4K monitor or a 13-inch laptop screen, because we know you might be reviewing your progress during a commute.
- **Offline-First:** Everything runs locally. There are no telemetry or analytics beacons. Your progress is your own.

### Why No Build Tools?
We deliberately avoided complex package managers to lower the barrier to entry. You can inspect every line of JSON and Python logic to *understand* how the simulation engine works. This transparency is part of the educational philosophy.

---

## 📜 License & Legal Clarity

This project is open-sourced under the **MIT License**. You are free to use, modify, and distribute this material for commercial or non-commercial purposes, provided you retain the original copyright notice.

You can read the full terms in the [LICENSE](LICENSE) file.

### 🚫 Disclaimer: The “No Magic” Clause
This repository is an educational tool designed to help candidates build deep, flexible knowledge. It is **not** a collection of actual exam questions or leaked materials. The scenarios are original compositions inspired by common business logic patterns, designed to train *methodology* rather than memory recall. The 1C:Specialist certification is a rigorous, evolving test; we are here to help you become a better engineer, not to offer shortcuts of questionable legality. Passing the exam is a matter of internalized competence, not superficial recall. All names and scenarios are fictional creations; any resemblance to actual companies or individuals is purely coincidental.

---

## 🤝 Contribution Guidelines

We embrace contributions from practitioners who have passed the exam and want to give back. Here is how to help:

1. **Scenario Submissions:** Do you have a memorable business case that taught you a crucial lesson? Fork the repo, create a new folder in `scenarios/`, and fill in the `task_definition.md` template. Include a skeleton of your reference solution, but focus on the *thinking process* in the `guru_brief.md`.
2. **Bug Fixes:** If you find a flaw in the `simulator` logic or a broken link in the `playground`, please submit a pull request with a clear description.
3. **Localization:** Help us expand the `glossary.md` or provide better translations for existing scenarios.
4. **Analytics Expansion:** Have an idea for a new performance metric to track? Open an issue to discuss it before building.

We believe that the best way to solidify your understanding of 1C is to **explain it to someone else**. Contributing to Metacon is a meta-learning experience itself—it forces you to articulate the implicit knowledge that helps you rationalize your expertise.

---

## 🧭 Final Thoughts: Your Journey to Mastery

The 1C:Specialist exam is not a wall; it's a series of gates. Each gate requires a specific key forged from understanding and practice. Metacon is your **forge**. We provide the heat (challenging scenarios), the anvil (reference solutions), and the hammer (the playgrounds), but the *striking*—the actual cognitive effort—must come from you.

We invite you to explore, to struggle productively, and to emerge on the other side not just with a certificate, but with a permanent upgrade to your architectural intuition. Welcome to the meta-context. Welcome to **Metacon**.

---

*© 2026 Metacon Contributors. Built with persistence, structured failure, and a deep respect for the 1C platform.*