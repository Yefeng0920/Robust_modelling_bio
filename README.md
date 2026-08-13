
# Robust modelling and inference for dependent data

### Reproducible R tutorials for dependence-aware modelling, diagnostics and statistical inference

This repository provides the reproducible code and online tutorials accompanying the manuscript:

> **Robust modelling and inference for conservation biology: flexible statistical solutions for non-normal, hierarchical, temporal, spatial, and phylogenetic data**

The repository is designed to help researchers and students move from statistical principles to practical implementation in **R**.

Two complementary tutorials are provided: one focuses on **model diagnostics**, particularly the diagnosis of residual dependence and other forms of model misspecification; the other provides a broader **code-along guide to the modelling and inferential strategies** discussed in the article.

---

## Online tutorials

### 1. Model diagnostics

**[Open the Model Diagnostics Tutorial](https://yefeng0920.github.io/Robust_modelling_bio/)**

This tutorial focuses on diagnosing whether important structure remains unexplained after fitting a statistical model.

It includes practical examples for:

- temporal residual autocorrelation;
- spatial residual autocorrelation;
- phylogenetic residual autocorrelation;
- heteroscedasticity;
- outliers;
- model misspecification; and
- distinguishing systematic ecological structure from residual dependence.

A central principle is that **autocorrelation should be diagnosed in model residuals rather than inferred from patterns in the raw response alone**. The tutorial illustrates how ecological trends can first be represented in the systematic component of a model and how residual diagnostics can then be used to determine whether additional dependence structures are required.

➡️ **Tutorial:**  
https://yefeng0920.github.io/Robust_modelling_bio/

---

### 2. Modelling and inference strategies

**[Open the Modelling and Inference Tutorial](https://yefeng0920.github.io/Robust_modelling_bio/Script/Expanded_tutorial.html)**

This code-along tutorial provides reproducible implementations of the major **modelling and inferential strategies** discussed in the article.

Rather than presenting statistical methods as an isolated catalogue, the tutorial begins with the scientific question and guides readers through decisions about:

- the response distribution;
- hierarchical structure;
- temporal, spatial and phylogenetic dependence;
- conditional versus population-average interpretation;
- within-unit and between-unit variation;
- model-based versus robust inference; and
- the intended scope of prediction and generalisation.

Methods illustrated include:

- linear models;
- generalised linear models;
- generalised least squares;
- linear and generalised linear mixed models;
- random intercepts and random slopes;
- temporal dependence and autoregressive models;
- spatial and spatio-temporal models;
- phylogenetic models;
- generalised estimating equations;
- fixed-effects and within-between models;
- heteroscedastic and distributional models;
- robust and cluster-robust variance estimation;
- Bayesian hierarchical models;
- dependence-aware resampling;
- blocked cross-validation; and
- sensitivity, pluralistic and multiverse analyses.

The emphasis throughout is not simply on **how to fit a model**, but on understanding **what scientific question the model answers, what assumptions it makes and how its results should be interpreted**.

➡️ **Tutorial:**  
https://yefeng0920.github.io/Robust_modelling_bio/Script/Expanded_tutorial.html

---

## How the two tutorials complement each other

| Resource | Main question | Primary focus |
|---|---|---|
| **Model Diagnostics Tutorial** | *Does important structure remain in the residuals?* | Diagnosing temporal, spatial and phylogenetic dependence, heteroscedasticity, outliers and model misspecification |
| **Modelling and Inference Tutorial** | *How should the data be modelled and inference conducted?* | Implementing dependence-aware modelling, robust inference, resampling and predictive-validation strategies |

Together, the tutorials support a workflow in which researchers first identify the **scientific question and data structure**, choose an appropriate modelling strategy, evaluate model adequacy, conduct inference that respects dependence, and assess the robustness of conclusions across defensible analytical choices.

---

## A dependence-aware workflow

The tutorials encourage researchers to work through five questions before choosing a statistical method:

1. **What is the scientific goal?**  
   Inference, explanation, prediction or exploration?

2. **What quantity should be estimated?**  
   For example, a conditional relationship, a population-average relationship, a within-unit association, a variance component or a prediction?

3. **What dependence structures are scientifically plausible?**  
   Hierarchical, temporal, spatial, phylogenetic or combinations of these?

4. **How confidently can the dependence structure be specified?**  
   Should dependence be represented explicitly in the model, or should inference be protected using robust or resampling-based approaches?

5. **To what population, place, time or taxonomic group should the results generalise?**

The guiding principle is:

> **Model choice should follow the scientific question, data-generating structure and inferential target, rather than software availability or statistical habit.**


![Uploading image.png…]()


---

## Reproducibility

All code supporting the tutorials is openly available in this repository:

**https://github.com/Yefeng0920/Robust_modelling_bio**

The tutorials are written in R/R Markdown and are intended to provide transparent, reproducible examples that readers can adapt to their own biodiversity datasets.

For the expanded modelling tutorial, the source document is:

```text
Script/Expanded_tutorial.Rmd
```

It can be rendered from the repository root using:

```r
rmarkdown::render("Script/Expanded_tutorial.Rmd")
```

Core examples are designed to be accessible to applied researchers, while computationally intensive or specialised methods are presented as optional extensions where appropriate.

---

## Intended audience

These materials are written for:

- biodiversity and conservation researchers;
- ecologists and evolutionary biologists;
- environmental scientists;
- graduate students;
- quantitative biologists; and
- researchers seeking practical guidance on dependent or non-normal data.

The tutorials assume basic familiarity with regression in R but do not assume specialist training in spatial statistics, longitudinal modelling, mixed models or robust inference.

---

## Associated manuscript

These resources accompany:

> **Robust modelling and inference for conservation biology: flexible statistical solutions for non-normal, hierarchical, temporal, spatial, and phylogenetic data**

The article develops a unified framework for analysing biodiversity data containing non-normal responses and hierarchical, temporal, spatial or phylogenetic dependence, with particular emphasis on matching the modelling and inferential strategy to the scientific question.

Full citation information will be added here following publication.

---

## Repository

**Source code and materials:**  
https://github.com/Yefeng0920/Robust_modelling_bio

**Model Diagnostics Tutorial:**  
https://yefeng0920.github.io/Robust_modelling_bio/

**Modelling and Inference Tutorial:**  
https://yefeng0920.github.io/Robust_modelling_bio/Script/Expanded_tutorial.html

---

## Feedback and contributions

We welcome feedback from researchers using these materials. If you identify an error, encounter a problem with the code, or have a suggestion for improving the tutorials, please open an issue in this GitHub repository.

---

## Authors

**Yefeng Yang · Jinming Pan · David Warton · Shinichi Nakagawa**

---

*These tutorials are intended to complement, rather than replace, the conceptual and methodological discussion in the associated article. Researchers should adapt model structures, diagnostics and inferential procedures to the biological question, sampling design and dependence structure of their own data.*
````


