# Contributing

Thanks for your interest in contributing to **Neuro-Symbolic AI for Product Design**.  
This repository is designed as an **awesome-style survey companion** with two synchronized artifacts:

- **GitHub (this repo):** curated browsing, taxonomy figures, issues/PR workflow, release notes.
- **ORKG Comparison (canonical table):** structured, queryable, continuously updateable comparison:
  https://orkg.org/comparisons/R1569149

We welcome contributions of (i) new papers, (ii) corrections, (iii) improved categorization, and (iv) stronger evidence/notes (datasets, evaluation signals, constraints, objectives, etc.).

---

## What can I contribute?

### A) Add a new paper
You can contribute a paper to:
1) **ORKG (preferred / canonical)** — best for structured comparison and filtering  
2) **GitHub README lists** — best for discoverability and community browsing  
Ideally do **both** (ORKG first, then README).

### B) Fix or improve an existing entry
Examples:
- Wrong year/venue/DOI/arXiv link
- Incorrect integration type (I–VI)
- Missing symbolic substrate / neural function / domain tags
- Weak or unclear “Key contribution & evidence”

### C) Add figures or tooling
Examples:
- Updated taxonomy figure
- Risk/challenges visualization improvements
- Scripts/templates for consistent formatting (optional)

---

## Ground rules (quality bar)

To keep the resource usable as a survey companion:

1. **Be precise and verifiable.** Prefer DOI / official proceedings / publisher pages over blog posts.
2. **Avoid promotional language.** Write neutral summaries and evidence statements.
3. **One paper = one primary link.** Choose the best canonical link (DOI if available; else openreview; else arXiv).
4. **Don’t overfit categories.** If a paper spans multiple domains, pick the *primary* one and note the rest briefly.
5. **If unsure, open an issue.** We will help classify.

---

## How to add a paper (recommended workflow)

### Step 1 — Add/update the paper in ORKG (canonical)
1. Open the ORKG comparison:
   https://orkg.org/comparisons/R1569149
2. Add a new contribution (paper) or edit an existing one.
3. Fill the fields as completely as possible (see “Data fields” below).
4. In the “Key contribution & evidence” field, include:
   - what the method does (1–2 sentences),
   - the product-design domain context,
   - the evaluation evidence (dataset/benchmark, metrics, constraints, objectives, baselines).

**Tip:** If you’re not sure about a field, leave it blank and add a short note (e.g., “TODO: verify venue”).

### Step 2 — Update this repository (README + optional BibTeX)
Create a PR that updates:
- `README.md` (add paper in the right section/type),
- optionally `bib/` or `refs.bib` if the repo maintains a BibTeX file (if present),
- optionally `data/` if we keep CSV exports from ORKG (if present).

If you add a paper to README, also add:
- Title, year, venue
- A single canonical link (DOI / openreview / arXiv)
- The integration type section (I–VI) that matches ORKG

### Step 3 — Cross-link ORKG ↔ GitHub
In your PR description, include:
- ORKG comparison link
- Paper identifier (DOI/arXiv/openreview id)
- What changed (added / corrected / reclassified)

---

## Data fields (how to fill ORKG consistently)

Please follow these conventions:

### Integration Type (I–VI)
Use the taxonomy from the survey:
- **Type I:** Symbolic → Neural (knowledge as features/embeddings)
- **Type II:** Symbolic[Neural] (neural oracles inside symbolic reasoning)
- **Type III:** Neuro ‖ Symbolic (parallel modules + exchange/verification/shielding)
- **Type IV:** Neuro:Symbolic→Neuro (compiled rules into architecture/training)
- **Type V:** Neuro_Symbolic (constraints as differentiable losses)
- **Type VI:** Neuro[Symbolic] (differentiable symbolic layers/solvers)

If a paper fits multiple, choose the **dominant** pattern and note alternatives in evidence text.

### Domains (choose primary)
Examples: CAD synthesis, manufacturing, assembly planning, topology optimization, materials, sustainability/LCA.

### Symbolic substrate (examples)
Ontology, knowledge graph, logic, constraints, rules, planning formalisms, Petri nets, temporal logic, SAT/SMT/MILP.

### Neural function (examples)
Perception, generation, optimization, surrogate modeling, policy learning (RL), decision transformers, diffusion models.

### Key contribution & evidence (template)
Use this neutral template:

> **Contribution:** What is the method and what NS mechanism is used?  
> **Domain:** Where it applies (CAD/manufacturing/assembly/materials/etc.).  
> **Evidence:** Dataset/benchmark/simulation + metrics/baselines + constraints/objectives (if any).

Keep it short but concrete (3–6 lines).

---

## Pull request checklist

Before submitting a PR, please ensure:

- [ ] The paper is added/updated in ORKG **or** an issue explains why not yet.
- [ ] README entry is placed under the correct Type (I–VI) section.
- [ ] The paper link is canonical (DOI preferred).
- [ ] Year and venue are correct.
- [ ] Summary is neutral and evidence-based.
- [ ] PR description includes ORKG link + what changed.

---

## Reporting issues (no PR needed)

Open an issue if you:
- want help classifying a paper,
- found duplicates,
- disagree with a type assignment,
- propose new fields or a refactor of taxonomy sections.

When opening an issue, include:
- Paper title + link
- Suggested Type (if any)
- One-sentence rationale

---

## License

By contributing, you agree that your contributions will be licensed under the repository’s license (see `LICENSE`).
