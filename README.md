# Neuro-Symbolic AI for Product Design: A Survey

[![IJCAI 2026](https://img.shields.io/badge/IJCAI--2026-Survey%20Track%20(Submitted)-blue)]()
[![ORKG](https://img.shields.io/badge/ORKG-Comparison-green)](https://orkg.org/comparisons/R1569149)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> **Integrating Neurosymbolic Systems in Advanced Product Design: A Comprehensive Review**  
> Siamak Ghodsi, Gollam Rabby, Nenad Krdzavac, Felix Engel, Sven Münker, Sören Auer  
> *Submitted to IJCAI 2026 Survey Track*

This repository accompanies our survey on neurosymbolic AI methods for product design, spanning generative CAD, manufacturing optimization, assembly planning, and sustainability-driven design.

---

## 📊 Dynamic Comparison Table

A comprehensive, queryable, and continuously updated comparison of methods is available on the **[Open Research Knowledge Graph (ORKG)](https://orkg.org/comparisons/R1569149)**.

---

## 🔬 Taxonomy Overview

We organize neurosymbolic methods using [Kautz's taxonomy](https://doi.org/10.1002/aaai.12036), adapted for product design contexts:

<p align="center">
  <img src="figures/taxonomy.png" alt="Neurosymbolic Integration Types" width="800"/>
</p>

| Type | Integration Pattern | Product Design Example |
|------|-------------------|----------------------|
| **I** | Symbolic → Neural | Material selection via KG embeddings |
| **II** | Symbolic[Neural] | CAD generation with neural manufacturability oracle |
| **III** | Neuro ‖ Symbolic | Process control: RL optimizer + safety verifier |
| **IV** | Neuro:Symbolic→Neuro | Manufacturing rules compiled into network |
| **V** | Neuro_Symbolic | Topology optimization with physics-informed constraints |
| **VI** | Neuro[Symbolic] | Assembly planning with differentiable SAT solver |

---

## 📚 Neurosymbolic Methods by Integration Type

### Type I: Symbolic → Neural (Knowledge as Features)

Symbolic knowledge (ontologies, knowledge graphs, domain taxonomies) is encoded as features or embeddings that inform neural learning.

| Paper | Year | Domain | Venue & Link|
|-------|------|--------|-----|
| Periodic Graph Transformers for Crystal Material Property Prediction | 2022 | Materials | [NeurIPS](https://openreview.net/forum?id=pqCT3L-BU9T) |
| Ontology-based Knowledge Representation of Industrial Production Workflow | 2023 | Manufacturing | [J. AEI](https://doi.org/10.1016/j.aei.2023.102185) |
| A New Ontology-based Approach to Automatic Information Extraction from Speech | 2025 | Manufacturing | [J. Adv Manuf. Tech.](https://doi.org/10.1007/s00170-025-15000-4) |
| Material Property Prediction with Element Attribute Knowledge Graphs | 2024 | Materials | [ArXiv](https://doi.org/10.48550/arXiv.2411.08414) |
| An Ontology-based Product Design Framework for Manufacturability Verification | 2018 | Design | [J. Adv Manuf. Tech.](https://doi.org/10.1007/s00170-018-2099-2) |
| Fine-tuning Large Enterprise Language Models via Ontological Reasoning | 2023 | General | [IJC. Rule ML](https://doi.org/10.1007/978-3-031-45072-3_6) |
| Graph Neural Network-enabled Manufacturing Method Classification | 2022 | Manufacturing | [Computers in Industry Journal](https://doi.org/10.1016/j.compind.2022.103697) |

### Type II: Symbolic[Neural] (Neural Oracles)

Symbolic reasoning systems use neural networks as oracles for perception, generation, or sub-symbolic computation.

| Paper | Year | Domain | Venue & Link|
|-------|------|--------|-----|
| Taxonomy-Informed Neural Networks for Smart Manufacturing | 2024 | Manufacturing | [J. Proc. Comp. Sci.](https://doi.org/10.1016/j.procs.2024.01.137) |
| NeSyGeo: Neuro-Symbolic Framework for Multimodal Geometric Reasoning | 2025 | Reasoning | [ICML Workshop](https://openreview.net/pdf/cd51b8278944e5da5f6ee643efdf5c823ddb3511.pdf) |
| LLM4CAD: Multimodal LLMs for 3D CAD Generation | 2025 | CAD | [J. Comput. Inf. Sci. Eng.](https://doi.org/10.1115/1.4067085) |
| OpenECAD: Efficient Visual Language Model for Editable 3D-CAD Design | 2024 | CAD | [Computers & Graphics Journal](https://doi.org/10.1016/j.cag.2024.104048) |
| CadVLM: Bridging Language and Vision in Parametric CAD Sketches | 2024 | CAD | [ECCV](https://doi.org/10.1007/978-3-031-72897-6_21) |
| Adaptive LLM-Symbolic Reasoning via Dynamic Logical Solver Composition | 2025 | Reasoning | [ArXiv](https://doi.org/10.48550/arXiv.2510.06774) |
| Do LLMs Really Adapt to Domains? An Ontology Learning Perspective | 2024 | Ontology | [ISWC](https://doi.org/10.48550/arXiv.2407.19998) |
| End-to-End Ontology Learning with Large Language Models | 2024 | Ontology | [NeurIPS](https://dl.acm.org/doi/10.5555/3737916.3740683) |
| Voyager: An Open-Ended Embodied Agent with Large Language Models | 2024 | Control | [TMLR](https://openreview.net/forum?id=ehfRiF0R3a) |
| KRISP: Integrating Implicit and Symbolic Knowledge for VQA | 2021 | VQA | [CVPR](https://openaccess.thecvf.com/content/CVPR2021/html/Marino_KRISP_Integrating_Implicit_and_Symbolic_Knowledge_for_Open-Domain_Knowledge-Based_VQA_CVPR_2021_paper.html) |

### Type III: Neuro ‖ Symbolic (Parallel Modules)

Neural and symbolic components operate in parallel with structured information exchange, enabling verification, shielding, or explanation.

| Paper | Year | Domain | Venue & Link|
|-------|------|--------|-----|
| Advancing Sustainable Manufacturing: RL with Adaptive Reward Machine | 2024 | Manufacturing | [Sustainability Journal](https://doi.org/10.3390/su16145873) |
| ASAP: Automated Sequence Planning for Complex Robotic Assembly | 2024 | Assembly | [ICRA](https://doi.org/10.1109/ICRA57147.2024.10611595) |
| Safe RL via Shielding under Partial Observability | 2023 | Control | [AAAI](https://ojs.aaai.org/index.php/AAAI/article/view/26723) |
| Towards Robust Shielded RL: The Fear Field Framework | 2025 | Control | [J.EngAppAI](https://doi.org/10.1016/j.engappai.2025.110055) |
| End-to-End Neuro-Symbolic RL with Textual Explanations (INSIGHT) | 2024 | Control | [ICML](https://proceedings.mlr.press/v235/luo24j.html) |
| Three Pathways to Neurosymbolic RL with Interpretable Networks | 2024 | Control | [10.48550/arXiv.2402.05307](https://doi.org/10.48550/arXiv.2402.05307) |
| Detect, Understand, Act: Neuro-symbolic Hierarchical RL Framework | 2022 | Control | [Machine Learning Journal](https://doi.org/10.1007/s10994-022-06142-7) |
| Neurosymbolic RL with Formally Verified Exploration (REVEL) | 2020 | Control | [NeurIPS](https://proceedings.neurips.cc/paper/2020/hash/448d5eda79895153938a8431919f4c9f-Abstract.html) |
| Constrained Decision Transformer for Offline Safe RL | 2023 | Control | [ICML](https://proceedings.mlr.press/v202/liu23m.html) |
| The Neuro-Symbolic Concept Learner | 2019 | Perception | [ICLR](https://openreview.net/forum?id=rJgMlhRctm) |

### Type IV: Neuro:Symbolic→Neuro (Compiled Integration)

Symbolic rules are compiled into neural network architecture or training procedure.

| Paper | Year | Domain | Venue & Link|
|-------|------|--------|-----|
| SPRING: Integrating Symbolic Reasoning into Neural Generative Models | 2025 | Design | [Artificial Intelligence](https://doi.org/10.1016/j.artint.2024.104257) |
| McGAN: Manufacturing Rules Embedded in Conditional GAN | 2025 | Manufacturing | [J. AEI](https://doi.org/10.1016/j.aei.2024.103074) |

### Type V: Neuro_Symbolic (Constraints as Loss)

Symbolic constraints (physics, logic, geometry) are incorporated as differentiable loss terms.

| Paper | Year | Domain | Venue & Link|
|-------|------|--------|-----|
| Complete PINN-Based Framework for Structural Topology Optimization | 2023 | Topology | [J.CMA](https://doi.org/10.1016/j.cma.2023.116401) |
| Scientific ML Through Physics-Informed Neural Networks | 2022 | Physics | [Journal of Scientific Computing](https://doi.org/10.1007/s10915-022-01939-z) |
| DL2: Training and Querying Neural Networks with Logic | 2019 | General | [ICML](https://proceedings.mlr.press/v97/fischer19a.html) |
| A Semantic Loss Function for Deep Learning with Symbolic Knowledge | 2018 | General | [ICML](https://proceedings.mlr.press/v80/xu18h.html) |
| NeurCADRecon: CAD Surface Reconstruction with Zero Gaussian Curvature | 2024 | CAD | [ACM Transactions on Graphics](https://doi.org/10.1145/3658171) |
| Geometry-Informed Neural Networks (GINN) | 2025 | Topology | [ICLR](https://openreview.net/forum?id=zpX0teJu9Z) |

### Type VI: Neuro[Symbolic] (Differentiable Symbolic Layers)

Symbolic solvers are made differentiable and embedded as layers within neural networks.

| Paper | Year | Domain | Venue & Link|
|-------|------|--------|-----|
| OptNet: Differentiable Optimization as a Layer | 2017 | General | [ICML](https://proceedings.mlr.press/v70/amos17a.html) |
| SATNet: Differentiable Satisfiability Solver | 2019 | General | [ICML](https://proceedings.mlr.press/v97/wang19e.html) |
| Differentiable Convex Optimization Layers (CVXpyLayers) | 2019 | General | [NeurIPS](https://proceedings.neurips.cc/paper/2019/hash/9ce3c52fc54362e22053399d3181c638-Abstract.html) |
| NURBS-Diff: Differentiable Programming Module for NURBS | 2022 | CAD | [J.CAD](https://doi.org/10.1016/j.cad.2022.103199) |
| DeepProbLog: Neural Probabilistic Logic Programming | 2021 | General | [Artificial Intelligence](https://doi.org/10.1016/j.artint.2021.103504) |

---

## 📖 Background & Foundations

### Neurosymbolic AI Surveys & Foundations

Core references for understanding NS-AI integration paradigms.

| Paper | Year | Venue & Link|
|-------|------|-----|
| The Third AI Summer (Kautz Taxonomy) | 2022 | [AAAI](https://doi.org/10.1002/aaai.12036) |
| Neurosymbolic AI: the 3rd Wave | 2023 | [J.AIR](https://doi.org/10.1007/s10462-023-10448-w) |
| Neural-Symbolic Learning and Reasoning: A Survey (IOS Press) | 2021 | [FAIA](https://doi.org/10.3233/FAIA210348) |
| A Survey on Neural-Symbolic Learning Systems | 2023 | [Neural Networks Journal](https://doi.org/10.1016/j.neunet.2023.06.028) |
| Neuro-Symbolic AI in 2024: A Systematic Review | 2024 | [ArXiv](https://doi.org/10.48550/arXiv.2501.05435) |
| Neuro-Symbolic Artificial Intelligence: A Survey | 2024 | [Neural Computing and Applications](https://doi.org/10.1007/s00521-024-09960-z) |
| Neurosymbolic Reinforcement Learning and Planning: A Survey | 2023 | [IEEE TAI](https://doi.org/10.1109/TAI.2023.3311428) |
| A Roadmap Toward Neurosymbolic Approaches in AI Design | 2025 | [IEEE ACCESS](https://doi.org/10.1109/ACCESS.2025.3617771) |
| Verification and Validation of Neurosymbolic AI | 2024 | [IEEE TAI](https://doi.org/10.1109/TAI.2024.3351798) |
| Review of Neuro-Symbolic AI for Advanced Cognitive Systems | 2025 | [J.ISWA](https://doi.org/10.1016/j.iswa.2025.200541) |
| Surveying Neuro-Symbolic Approaches for Reliable AIoT | 2024 | [JRIE](https://doi.org/10.1007/s40860-024-00231-1) |
| Techniques for Inclusion of Domain-Knowledge into DNNs | 2022 | [Scientific Reports Journal](https://doi.org/10.1038/s41598-021-04590-0) |
| Neural-Symbolic Learning Systems (Book) | 2002 | [SPRINGER NATURE](https://doi.org/10.1007/978-1-4471-0211-3) |
| Fast Relational Learning using Bottom Clause Propositionalization | 2013 | [Machine Learning Journal](https://doi.org/10.1007/s10994-013-5392-1) |
| Benchmarking Neuro-Symbolic Description Logic Reasoners | 2025 | [NeSy AIJ](https://doi.org/10.1177/29498732251339943) |

### Multi-Objective Reinforcement Learning

Foundational MORL methods providing multi-objective optimization capabilities.

| Paper | Year | Venue & Link|
|-------|------|-----|
| A Practical Guide to Multi-Objective RL and Planning | 2022 | [JAAMAS](https://doi.org/10.1007/s10458-022-09552-y) |
| A Survey of Multi-Objective Sequential Decision-Making | 2013 | [JAIR](https://doi.org/10.1613/jair.3987) |
| MORL Based on Decomposition: A Taxonomy and Framework | 2024 | [JAIR](https://doi.org/10.1613/jair.1.15702) |
| Multi-Objective RL using Sets of Pareto Dominating Policies | 2014 | [JMLR](https://www.jmlr.org/papers/v15/vanmoffaert14a.html) |
| A Generalized Algorithm for MORL and Policy Adaptation | 2019 | [NeurIPS](https://proceedings.neurips.cc/paper/2019/hash/4a46fbfca3f1465a27b210f4bdfe6ab3-Abstract.html) |
| Deep Reinforcement Learning for Multiobjective Optimization | 2021 | [IEEE TCYB](https://doi.org/10.1109/TCYB.2020.2977661) |
| On Generalization Within MORL Algorithms | 2025 | [ICLR](https://openreview.net/forum?id=tuEP424UQ5) |
| Prediction-Guided MORL for Continuous Robot Control | 2020 | [ICML](https://proceedings.mlr.press/v119/xu20h.html) |
| Multi-objective Cross-task Learning for Surgical Robot Automation | 2024 | [ICRA](https://doi.org/10.1109/ICRA57147.2024.10611051) |
| On Transforming RL With Transformers | 2024 | [IEEE TPAMI](https://doi.org/10.1109/TPAMI.2024.3408271) |

### Neural CAD & Geometric Deep Learning

Pure neural approaches for CAD and geometric processing (comparison baselines).

| Paper | Year | Venue & Link|
|-------|------|-----|
| Geometric Deep Learning for Computer-Aided Design: A Survey | 2025 | [IEEE Access](https://doi.org/10.1109/ACCESS.2025.3587121) |
| GenCAD: Image-Conditioned CAD Generation with Diffusion Priors | 2025 | [TMLR](https://openreview.net/forum?id=e817c1wEZ6) |
| CADDreamer: CAD Object Generation from Single-view Images | 2025 | [CVPR](https://openaccess.thecvf.com/content/CVPR2025/html/Li_CADDreamer_CAD_Object_Generation_from_Single-view_Images_CVPR_2025_paper.html) |
| PHT-CAD: Efficient CAD Parametric Primitive Analysis | 2025 | [ArXiv](https://doi.org/10.48550/arXiv.2503.18147) |
| A Neural Network Based Approach for Product Form Design | 2002 | [Journal Design Studies](https://doi.org/10.1016/S0142-694X(01)00015-1) |
| Position: Graph Foundation Models are Already Here | 2024 | [ICML](https://doi.org/10.48550/arXiv.2402.02216) |

### Manufacturing & Design Background

Domain context for understanding product design challenges.

| Paper | Year | Venue & Link|
|-------|------|-----|
| Industrial AI in Industry 4.0: Systematic Review | 2020 | [IEEE ACCESS](https://doi.org/10.1109/ACCESS.2020.3042874) |
| Convolutional and Generative Adversarial NNs in Manufacturing | 2019 | [IJPR](https://doi.org/10.1080/00207543.2019.1662133) |
| Artificial Neural Networks in Manufacturing | 1994 | [IEEE TCPM](https://doi.org/10.1109/95.296402) |
| Disassembly Sequence Planning of Waste Auto Parts | 2021 | [JAWMA](https://doi.org/10.1080/10962247.2020.1871444) |
| The Future of Human-AI Collaboration: Hybrid Intelligence Systems | 2021 | [ArXiv](https://doi.org/10.48550/arXiv.2105.03354) |
| Accountability in AI: What It Is and How It Works | 2024 | [Journal AI & Society](https://doi.org/10.1007/s00146-023-01635-y) |
| Transformer-Based RL for Scalable Multi-UAV Area Coverage | 2024 | [IEEE TITS](https://doi.org/10.1109/TITS.2024.3358010) |

### Datasets & Benchmarks

Resources for evaluating NS-AI methods in product design contexts.

| Paper | Year | Domain | Venue & Link|
|-------|------|--------|-----|
| SketchGraphs: Relational Geometry Dataset for CAD | 2020 | CAD | [ICML Workshop](https://doi.org/10.48550/arXiv.2007.08506) |
| ABO: Dataset and Benchmarks for Real-World 3D Object Understanding | 2022 | 3D | [CVPR](https://doi.org/10.1109/CVPR52688.2022.02045) |
| ArchCAD-400K: Large-Scale CAD Drawings Dataset | 2025 | CAD | [NeurIPS](https://openreview.net/forum?id=rAGWvnpcKe) |
| UCSM: Dataset of U-shaped CAD Geometries for Deep Drawing | 2025 | Manufacturing | [J. CAD](https://doi.org/10.1016/j.cad.2025.103924) |
| HolStep: Dataset for Higher-order Logic Theorem Proving | 2017 | Logic | [ICLR](https://openreview.net/forum?id=ryuxYmvel) |
| YAHPO Gym: Multi-Objective Multi-Fidelity Benchmark | 2022 | Optimization | [AutoML](https://proceedings.mlr.press/v188/pfisterer22a.html) |
| Snorkel: Rapid Training Data Creation with Weak Supervision | 2017 | General | [VLDB](https://doi.org/10.14778/3157794.3157797) |

### Knowledge Representation Foundations

| Paper | Year | Venue & Link|
|-------|------|-----|
| Translating Embeddings for Modeling Multi-relational Data (TransE) | 2013 | [NeurIPS](https://proceedings.neurips.cc/paper/2013/hash/1cecc7a77928ca8133fa24680a88d2f9-Abstract.html) |

---

## 🎯 Key Findings

1. **Loose couplings dominate**: Types I–III are most common in practice, preserving modularity and CAD/simulation pipeline compatibility
2. **Tight integrations remain research-focused**: Types IV–VI show promise but face scalability and domain-specific differentiability challenges  
3. **Cross-domain transfer potential**: General-domain differentiable solvers (OptNet, SATNet, CVXpyLayers) offer clear pathways to design automation
4. **Evaluation gaps**: Standardized benchmarks for constraint-aware, multi-objective design are lacking

---

## ⚠️ Risks and Challenges

<p align="center">
  <img src="figures/risks_challenges.png" alt="Risks and Challenges" width="700"/>
</p>

---

## 📖 Citation

```bibtex
@inproceedings{ghodsi2026neurosymbolic,
  title     = {Integrating Neurosymbolic Systems in Advanced Product Design: A Comprehensive Review},
  author    = {Ghodsi, Siamak and Rabby, Gollam and Krdzavac, Nenad and Engel, Felix and M{\"u}nker, Sven and Auer, S{\"o}ren},
  booktitle = {Under review to the NAI Jorunal},
  year      = {2026},
  volume    = {TBD},
  pages     = {1-22}
}
```

---

## 🔗 Related Resources

- **[ORKG Comparison Table](https://orkg.org/comparisons/R1569149)** — Dynamic, queryable version of Table 2
- **[Kautz Taxonomy (AAAI 2022)](https://doi.org/10.1002/aaai.12036)** — Original six-type NS classification
- **[MORL Practical Guide](https://doi.org/10.1007/s10458-022-09552-y)** — Multi-objective RL foundations

---
## 🔁 ORKG vs GitHub: What lives where?

This project is maintained in **two complementary forms**:

- **ORKG Comparison (live, queryable):**  
  The ORKG page is the **most up-to-date structured knowledge base** behind our survey table(s). It is designed for
  filtering, querying, and reusing the comparison as machine-actionable research knowledge.

- **GitHub Repository (curated, narrative):**  
  This repository provides the **human-readable entry point** to the survey: taxonomy figures, risk visualizations,
  reading lists grouped by integration types, and documentation for how the survey is organized.

### Source of truth
- **For structured metadata and the evolving comparison table:** ORKG is the *source of truth*.  
- **For figures, taxonomy narrative, and a stable snapshot aligned with the PDF:** GitHub is the *source of truth*.

### Synchronization policy
- ORKG may contain **more papers and richer fields** than the README at any time (continuous updates).
- The README is updated in **discrete snapshots** (e.g., for major revisions, resubmissions, or periodic releases).
- The repository aims to keep the README consistent with a tagged release (or commit) corresponding to the paper version.

**ORKG link:** https://orkg.org/comparisons/R1569149

## 📄 License

This project is licensed under the MIT License.

---

## 🙏 Acknowledgments

This work was supported by the DFG Priority Programme SPP 2443 Human Decision (Grant No. 543081196) and the German Ministry of Education and Research (BMBF) for the project KISSKI AI Service Center (01IS22093C).
