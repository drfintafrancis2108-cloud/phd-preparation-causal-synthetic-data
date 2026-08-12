# Methodological Preparation for PhD Research

## Causal Inference, Synthetic Data, Privacy–Utility Trade-off and Causal Utility

This repository documents my ongoing methodological preparation for PhD research on the evaluation of anonymized and synthetic health data.

The preparation is motivated by a central methodological question:

> **Does statistical similarity between real and synthetic data necessarily imply preservation of causal information?**

The work therefore focuses on understanding how data modification, anonymization, and synthetic data generation may affect statistical properties, privacy, causal relationships, and causal estimands.

---

# Methodological Handbook

I have developed a methodological handbook as part of my preparation. It currently contains eight chapters covering the main methodological areas relevant to the proposed PhD research.

### Current chapters

1. **Causal Inference and Causal Frameworks**
   - Causal estimands
   - DAGs
   - Confounding
   - Mediation
   - Colliders
   - Identification
   - Causal estimation

2. **Causality and Machine Learning**
   - Machine learning in causal inference
   - Prediction versus causal inference
   - Causal forests
   - Tree-based approaches
   - Machine-learning-based nuisance estimation

3. **Synthetic Data**
   - Motivation for synthetic data
   - Types of synthetic data
   - Synthetic data generation
   - Applications in health research
   - Advantages and limitations

4. **Synthetic Data Generation Methods**
   - Parametric synthesis
   - CART
   - Conditional inference trees (`ctree`)
   - Random Forest
   - Bayesian Networks
   - `synthpop`
   - `bnlearn`
   - Generative approaches

5. **Simulation Studies**
   - Principles of simulation studies
   - Data-generating mechanisms
   - Confounding structures
   - Treatment and outcome generation
   - Simulation-based comparison of methods
   - Evaluation of synthetic data

6. **Privacy–Utility Trade-off**
   - Anonymization
   - Quasi-identifiers
   - Re-identification risk
   - k-anonymity
   - Privacy metrics
   - Statistical utility
   - Privacy–utility trade-off

7. **Causal Utility**
   - Statistical utility versus causal utility
   - Preservation of causal estimands
   - ATE preservation
   - Regression adjustment
   - G-computation
   - Inverse Probability of Treatment Weighting (IPTW)
   - Propensity-score distributions
   - Causal effect comparison between real and synthetic data

8. **Causal Mechanism Preservation**
   - Preservation of causal relationships
   - Treatment assignment mechanisms
   - Outcome-generating mechanisms
   - Covariate relationships
   - Causal graphs
   - Distinguishing statistical similarity from causal similarity

### 📄 Handbook

The complete handbook is available here:

**[Read the PhD Methodological Preparation Handbook](./PhD_Preparation_Handbook.pdf)**

The handbook is a living document and will be updated as my methodological preparation develops.

---

# 💻 R Implementations

The repository contains practical R implementations corresponding to the methodological concepts studied in the handbook.

Current implementations include:

### Synthetic Data Generation

- CART synthesis
- Conditional inference tree (`ctree`) synthesis
- Random Forest synthesis
- Bayesian Network synthesis using `bnlearn`
- Synthetic data generation using `synthpop`

### Statistical Utility

- Descriptive statistics
- Distributional comparisons
- Correlation comparisons
- Statistical similarity between real and synthetic datasets
- Predictive utility

### Privacy Evaluation

- Quasi-identifier identification
- Re-identification risk
- k-anonymity
- Privacy evaluation
- Utility loss
- Privacy–utility trade-off

### Causal Utility

The current causal utility implementations compare causal analyses performed on the original and synthetic datasets.

Methods include:

- Regression adjustment
- G-computation
- Inverse Probability of Treatment Weighting (IPTW)
- Propensity-score modelling
- Propensity-score distribution comparison
- Causal effect estimation
- Absolute causal error
- Relative causal error
- Comparison of causal estimands between real and synthetic data

The objective is to investigate whether synthetic data preserve the causal conclusions obtained from the original data.

---

# Research Focus

The methodological preparation is organized around the following framework:

```text
Data Generation
      ↓
Synthetic / Anonymized Data
      ↓
Statistical Utility
      ↓
Privacy
      ↓
Causal Utility
      ↓
Causal Mechanism Preservation
      ↓
Overall Privacy–Utility–Causal Utility Trade-off
