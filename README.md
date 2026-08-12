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

1. Causal Inference and Causal Frameworks
Topics include:

Causal questions and causal estimands
Directed Acyclic Graphs (DAGs)
Confounding
Mediation
Colliders
Backdoor paths
Identification
Causal assumptions
Causal estimation

2. Methods for Causal Estimation
Topics include:

Regression adjustment
Stratification
Matching
Propensity scores
Inverse Probability of Treatment Weighting (IPTW)
G-computation
Doubly robust estimation
Targeted Maximum Likelihood Estimation (TMLE)

3. Machine Learning for Causal Inference
Topics include:

Prediction versus causal inference
Machine learning in causal inference
Tree-based approaches
Causal forests
Machine-learning-based nuisance estimation
Relationship between prediction and causal effect estimation

4. Synthetic Data Generation
Topics include:

Motivation for synthetic data
Synthetic data generation
Parametric approaches
CART
Conditional inference trees (ctree)
Random Forest
Bayesian Networks
synthpop
bnlearn
Generative approaches

5. Simulation Studies
Topics include:

Principles of simulation studies
Data-generating mechanisms
Covariates
Treatment assignment
Outcomes
Confounding structures
Simulation-based methodological evaluation
Comparing real and synthetic data under controlled conditions

6. Causal Utility and Causal Mechanism Preservation
Topics include:

Statistical utility versus causal utility
Preservation of causal estimands
ATE preservation
Regression adjustment
G-computation
IPTW
Propensity-score distributions
Causal effect comparison
Treatment-assignment mechanisms
Outcome-generating mechanisms
Preservation of causal relationships
Distinguishing statistical similarity from causal similarity

7. Privacy–Utility Trade-off in Synthetic and Anonymized Data
Topics include:

Privacy and data protection
Anonymization
Quasi-identifiers
Re-identification risk
k-anonymity
Privacy metrics
Statistical utility
Information loss
Privacy–utility trade-offs

8. Anonymization of Datasets
Topics include:

Data anonymization
Identification of quasi-identifiers
Generalization
Suppression
Re-identification risk
Privacy-preserving data publishing
Evaluation of anonymized data
# R Implementations

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

The reporsitory structure

├── README.md
│
├── PhD_Preparation_Handbook.pdf
│
├── Chapter 1_ Causal Inference.pdf
├── Chapter 2_ Methods for Causal Estimation.pdf
├── Chapter3_ Machine Learning for causal Inference.docx
├── Chapter 4_ Synthetic Data Generation.pdf
├── Chapter 5_ ML for Casual Inference .pdf
├── Chapter 6_ Causal utility and causal mechanism preservation.pdf
├── Chapter 7_ Privacy Utility trade off in Synthetic and anonymized datasets.pdf
├── Chapter 8_ Anonymization of datasets .pdf
│
├── causal_1.Rmd
├── causal_2.Rmd
├── causal_3.Rmd
│
├── syn_1.Rmd
├── syn_2.Rmd
│
├── Simulation_Bayesian.Rmd
├── Bayesian_learning.Rmd
│
└── privacy utility.Rmd
