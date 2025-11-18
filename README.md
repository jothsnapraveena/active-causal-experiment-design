# 🧬 Active Causal Experiment Design

**Author:** Jothsna Praveena Pendyala  
**Conference:** WiML @ NeurIPS 2025 — Poster Presentation  

---

## **Overview**
This project introduces an **Active Causal Experiment Design** framework that efficiently estimates causal effects (ATE) in biological datasets.  
Instead of relying on random experiment selection, this method uses **Expected Variance Reduction (EVR)** to identify the most informative next experiment, minimizing uncertainty and cost.

---

## **Key Idea**
Traditional random sampling leads to unstable ATE estimates.  
Our framework applies an **AI-driven, iterative selection loop** that:
- Estimates ATE via linear regression  
- Bootstraps variance to measure uncertainty  
- Actively selects new samples that reduce ATE variance the most  

---

## **Datasets**
Validated across four real datasets:  

| Dataset | Type | Description |
|----------|------|-------------|
| **RummaGEO** | Transcriptomics | Drug perturbation effects on gene expression |
| **LINCS L1000** | Transcriptomics | High-throughput gene expression perturbations |
| **Cell Painting** | Morphological | Imaging-based cellular phenotype data |
| **PRISM Viability** | Functional | Drug response and cell survival assays |

---

## **Results**
Causal Acquisition converges faster and produces smoother, stable ATE estimates compared to Random Acquisition — achieving reliability with fewer experiments across diverse data modalities.

---

## **Future Work**
Extend to nonlinear causal models (Causal Forests, Doubly Robust Learners)  
and deploy in real lab pipelines for adaptive experiment guidance.

---

## **References**
[1] M. A. Hernán and J. M. Robins, *Causal Inference: What If*, Chapman & Hall/CRC, 2020.  
[2] B. Settles, *Active Learning*, 2012.  
[3] A. Subramanian et al., *Cell*, vol. 171, pp. 1437–1452.e17, 2017.  

---

### **GitHub Tagline**
> Active learning framework for efficient causal effect estimation across biological datasets
