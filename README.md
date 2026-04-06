# 📊 Machine Learning in Tabular Data

A curated hub of modern tabular datasets, benchmark suites, and educational notebooks focusing on real-world machine learning challenges.

> Tabular data is structured data organized in a table format, representing the most common data type in real-world AI applications. Benchmark suites standardize the evaluation of machine learning models on these datasets.

#### 💡 Why tabular data benchmarks?
1. **Standardized evaluation** (Unified metrics across the industry)
2. **Real-world robustness** (Testing on shifting, imbalanced, and messy data)
3. **Reproducible research** (Preventing biased testing)
4. **Fair model comparison** (e.g., Deep Learning vs. Trees)

---

## 📑 Table of Contents
* [🎯 Supervised Learning](#-supervised-learning)
* [⏳ Survival Analysis (Time-to-Event)](#-survival-analysis-time-to-event)
* [🔄 Domain Shift](#-domain-shift)
* [📈 Spatiotemporal & Longitudinal Forecasting](#-spatiotemporal--longitudinal-forecasting)
* [🧩 Clustering](#-clustering)
* [🔍 Feature Selection](#-feature-selection)
* [🚨 Anomaly Detection](#-anomaly-detection)
* [⚖️ Class Imbalance](#️-class-imbalance)
* [🔗 Relational & Multimodal Learning](#-relational--multimodal-learning)

---

## 🎯 Supervised Learning
Evaluating models on standard classification and regression tasks to expose pure architectural disparities and predictive power.

#### 🗄️ Benchmarks (Standard & Biological Data)
* **[TabArena](https://github.com/autogluon/tabarena)** A living benchmark with an objective Elo rating system and strict hyperparameter tuning budgets (51 curated datasets). Essential for standard clinical and general tabular data. [Website](https://tabarena.ai/)
* **[TabZilla](https://github.com/naszilla/tabzilla)** Algorithmic stress test specifically featuring the 36 "hardest" datasets (filtered from 176).
* **[Grinsztajn Benchmark](https://github.com/LeoGrin/tabular-benchmark)** The classic 2022 study establishing the Neural Networks vs. Trees baseline (45 datasets).
* **[Cancer Multi-Omics Benchmark (MLOmics)](https://github.com/chenzRG/Cancer-Multi-Omics-Benchmark)** Systematic evaluation of machine learning methods for pan-cancer classification.
* **[ProteomicsML](https://github.com/compomics/ProteomicsML)** A curated repository mapping raw peptide sequences to physicochemical properties (e.g., retention times, fragmentation patterns) to test peptide embedding strategies.
* **[METS-CoV](https://github.com/yuzhimanhua/METS-CoV)** Epidemiological tabular dataset extracting medical entities and sentiments from social media to track disease metrics.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Supervised Learning on Tabular Data: From Linear Baselines to Foundation Models](./notebooks/supervised/supervisedClassic.ipynb)**
  *(Evaluates Linear Regression, LASSO, XGBoost across standard datasets and high-dimensional oncology data).*

---

## ⏳ Survival Analysis (Time-to-Event)
Traditional models fail on right-censored clinical data. This domain evaluates models optimizing highly specialized objective functions (e.g., Cox Partial Likelihood) to predict dynamic risk trajectories.

#### 🗄️ Benchmarks
* **[SurvBoard](https://github.com/Eriida/SurvBoard)** A standardized benchmarking framework explicitly designed for multi-omics cancer survival models. Integrates 28 massive datasets (TCGA, ICGC, TARGET) and evaluates pan-cancer joint training on highly censored tabular arrays.

---

## 🔄 Domain Shift
Evaluating how models handle temporal changes, feature corruption, batch effects, and out-of-distribution (OOD) scenarios.

#### 🗄️ Benchmarks (Standard & Biological Data)
* **[TableShift](https://github.com/mlfoundations/tableshift)** OOD generalization across finance and healthcare tasks. Healthcare subsets explicitly partition data by socioeconomic variables (poverty, region) to simulate real-world healthcare deployment shifts. [Website](https://tableshift.org/)
* **[LAMPP (Live Assessment of Metagenomics for Phenotype Prediction)](https://github.com/borenstein-lab/LAMPP)** Evaluates host phenotype prediction from gut metagenomic tables. Tests model generalization by enforcing Leave-One-Dataset-Out (LODO) validation across multinational cohorts to prevent batch-effect memorization.
* **[ADORE (Acute aquatic Dataset for Objective Risk Evaluation)](#)** Ecotoxicological benchmark predicting aquatic toxicity. Enforces structural domain shifts by partitioning testing data using chemical Murcko scaffolds.
* **[TabReD](https://github.com/yandex-research/tabred)** Time-dependent industrial benchmark for evaluating temporal robustness.
* **[scIB & scIB-E](https://github.com/theislab/scib)** The industry standard for evaluating Data Integration and Batch Effect correction across single-cell datasets.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Domain Shift & Data Integration: Handling Non-IID Tabular Data](./notebooks/domain_shift/domain_shift_masterclass.ipynb)**
  *(Demonstrates model degradation over time and strategies for batch-effect removal in biological data).*

---

## 📈 Spatiotemporal & Longitudinal Forecasting
Models applied to these tables must handle temporal distribution shifts, irregularly sampled time intervals, and spatial covariances (Non-IID rows).

#### 🗄️ Benchmarks
* **[LakeBeD-US](#)** A massive ecological benchmark tailored for tabular ML, encompassing over 500 million unique observations of water quality time series and vertical depth profiles across 21 US lakes.
* **[Microbiome Time Series Benchmarks](#)** Longitudinal tabular datasets charting highly autocorrelated shifts in dynamic microbial communities over time (e.g., infant gut colonization).

---

## 🧩 Clustering
Evaluating unsupervised learning methods to discover hidden groupings, sub-types, and topologies in data without prior labeling.

#### 🗄️ Benchmarks (Standard & Biological Data)
* **[OpenProblems in Single-Cell Analysis](https://github.com/openproblems-bio/openproblems)** A massive, living benchmark evaluating models on tasks like cell-type clustering and dimensionality reduction. [Website](https://openproblems.bio/)
* **[MIMIC-IV Pattern Discovery and Disentanglement (PDD)](#)** Discretizes numerical clinical features into event-based representations to stratify intensive care patient records into interpretable clinical clusters.
* **[scRNAseq_Benchmark](https://github.com/tabdelaal/scRNAseq_Benchmark)** Benchmarking unsupervised tools for single-cell RNA-sequencing.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Clustering Tabular Data: Uncovering Hidden Structures](./notebooks/clustering/clustering_masterclass.ipynb)**
  *(Explores K-Means, DBSCAN, and Autoencoder-based clustering for cell-type discovery).*

---

## 🔍 Feature Selection
Evaluating the identification of true signals amidst injected noise and the extreme $P \gg N$ (High-Dimensional, Low-Sample-Size) paradigm.

#### 🗄️ Benchmarks (Standard & Biological Data)
* **[DepMap Achilles Gene Essentiality](https://depmap.org/portal/)** High-throughput CRISPR/Cas9 screens where models must sift through massive expression matrices ($P \gg N$) to identify "modifier genes" that predict cellular vulnerability.
* **[CuratedMetagenomicData Benchmarks](#)** Evaluates normalization strategies (e.g., CLR) and feature selection in identifying robust microbial biomarkers amidst high technical noise.
* **[MetaboLights Clinical Feature Benchmarks (MTBLS28)](#)** Maps thousands of mass-spectrometry features against incredibly small patient sample sizes (e.g., 7,017 features vs. 88 samples).
* **[Feature Selection in Tabular DL Benchmark](https://github.com/vcherepanova/tabular-feature-selection)** Specialized environment injecting corrupted and second-order engineered features.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Feature Selection Masterclass: Filter, Wrapper, and Embedded Methods](./notebooks/feature_selection/feature_selection_masterclass.ipynb)**
  *(Features ANOVA, RFE, LASSO, and STG for identifying true signals in high-dimensional and non-linear data).*

---

## 🚨 Anomaly Detection
Evaluating algorithms on their ability to identify rare, malicious, or defective instances in tabular datasets.

#### 🗄️ Benchmarks
* **[ADBench (Healthcare & Biology Subsets)](https://github.com/Minqi824/ADBench)** An expansive tabular anomaly detection benchmark. Biological subsets feature varied degrees of contamination to evaluate algorithms classifying arrhythmias, breast cancer diagnostics, and extreme physiological outliers.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Anomaly Detection: Finding Needles in Tabular Haystacks](./notebooks/anomaly_detection/anomaly_masterclass.ipynb)**
  *(Currently under development. Will feature Isolation Forests and Autoencoders for rare event detection).*

---

## ⚖️ Class Imbalance
Evaluating models on skewed datasets where the minority class is critical but easily ignored by standard loss functions.

#### 🗄️ Benchmarks
* **[CLIMB](https://github.com/ZhiningLiu1998/imbalanced-ensemble)** Extreme class imbalance benchmark evaluating state-of-the-art algorithms across 73 datasets.
* **[Project Data Sphere (PDS) Clinical Trial Arrays](#)** Phase III oncology clinical trial tabular datasets evaluating algorithms predicting rare, severe adverse events and early treatment discontinuation.

---

## 🔗 Relational & Multimodal Learning
Evaluating models on messy enterprise databases, multi-table joins, and tables containing raw text or graph structures.

#### 🗄️ Benchmarks
* **[NxtDRP (GDSC / CCLE / CTRP)](#)** An expansive entity-relation benchmark requiring algorithms to ingest multi-omics cell-line features fused with drug molecular graphs to predict therapeutic response, exposing "specification gaming" vulnerabilities.
* **[CARTE Benchmark](https://github.com/soda-inria/carte)** Graph-based solutions for multimodal data (complex strings, raw text) and multi-table joins (51 relational datasets).
* **[PharmaFormer Tabular Integration](#)** Evaluates the transfer of knowledge learned from massive 2D cell line screens to highly complex, limited-sample 3D organoid drug response arrays.
* **[LIVE (Latent Interacting Variable Effects) Modeling](#)** Integrates microbiome multi-omics data using single-omic latent variables to predict Crohn's Disease.
* **[TALENT](https://github.com/LAMDA-Tabular/TALENT)** Massive toolkit officially integrating 35+ deep tabular processing methods.
