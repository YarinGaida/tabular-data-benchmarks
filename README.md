# 📊 Machine Learning in Tabular Data: Benchmarks & Algorithms

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
* [🔄 Domain Shift & Data Integration](#-domain-shift--data-integration)
* [🧩 Clustering & Representation Learning](#-clustering--representation-learning)
* [🔍 Feature Selection](#-feature-selection)
* [🚨 Anomaly Detection](#-anomaly-detection)
* [⚖️ Class Imbalance](#️-class-imbalance)
* [🔗 Relational & Multimodal Learning](#-relational--multimodal-learning)

---

## 🎯 Supervised Learning
Evaluating models on standard classification and regression tasks to expose pure architectural disparities and predictive power.

#### 🗄️ Benchmarks (Standard Data)
* **[TabArena](https://github.com/autogluon/tabarena)** A living benchmark with an objective Elo rating system and strict hyperparameter tuning budgets (51 curated datasets). Essential for standard clinical and general tabular data. [Website](https://tabarena.ai/)
  * [*TabArena: A Living Benchmark for Machine Learning on Tabular Data* (2025)](https://arxiv.org/abs/2506.16791)
* **[TabZilla](https://github.com/naszilla/tabzilla)** Algorithmic stress test specifically featuring the 36 "hardest" datasets (filtered from 176).
  * [*When do neural nets outperform boosted trees on tabular data?* (2023)](https://arxiv.org/abs/2305.02997)
* **[Grinsztajn Benchmark](https://github.com/LeoGrin/tabular-benchmark)** The classic 2022 study establishing the Neural Networks vs. Trees baseline (45 datasets).
  * [*Why do tree-based models still outperform deep learning on typical tabular data?* (2022)](https://arxiv.org/abs/2207.08815)

#### 🧬 Benchmarks (High-Dimensional / Biological Data)
* **[Cancer Multi-Omics Benchmark (MLOmics)](https://github.com/chenzRG/Cancer-Multi-Omics-Benchmark)** Systematic evaluation of machine learning methods for pan-cancer classification and survival prediction using multimodal biological tables.

#### 💻 Algorithms & Educational Notebooks
**Classic Methods**
* **Logistic Regression** - `[View Notebook Example](./notebooks/supervised/logistic_regression.ipynb)`
* **Gradient Boosted Trees (XGBoost/LightGBM)** - `[View Notebook Example](./notebooks/supervised/xgboost_example.ipynb)`

**Deep Learning Methods**
* **Multi-Layer Perceptron (MLP)** - `[View Notebook Example](./notebooks/deep/mlp_example.ipynb)`
* **TabPFN** - `[View Notebook Example](./notebooks/deep/tabpfn_example.ipynb)`

---

## 🔄 Domain Shift & Data Integration
Evaluating how models handle temporal changes, feature corruption, and out-of-distribution (OOD) scenarios.

#### 🗄️ Benchmarks (Standard Data)
* **[TabReD](https://github.com/yandex-research/tabred)** Time-dependent industrial benchmark for evaluating temporal robustness (8 massive datasets).
  * [*TabReD: Analyzing Pitfalls and Filling the gaps in Tabular Deep Learning Benchmarks* (2024)](https://arxiv.org/abs/2406.19380)
* **[TableShift](https://github.com/mlfoundations/tableshift)** Out-of-Distribution (OOD) generalization across finance and healthcare tasks (15 datasets). *(Includes Wild-Tab for regression)*. [Website](https://tableshift.org/)
  * [*TableShift: A Benchmark for Out-of-Distribution Generalization in Tabular Data* (2023)](https://arxiv.org/abs/2312.07577)
* **[TabFSBench](https://github.com/LAMDASZ-ML/TabFSBench)** Pinpoint feature-shift scenarios simulating upstream data pipeline failures.

#### 🧬 Benchmarks (High-Dimensional / Biological Data)
* **[scIB & scIB-E](https://github.com/theislab/scib)** The industry standard for evaluating Data Integration and Batch Effect correction across single-cell datasets from different laboratories.

---

## 🧩 Clustering & Representation Learning
Evaluating unsupervised learning methods to discover hidden groupings, sub-types, and topologies in data without prior labeling.

#### 🧬 Benchmarks (High-Dimensional / Biological Data)
* **[OpenProblems in Single-Cell Analysis](https://github.com/openproblems-bio/openproblems)** A massive, living benchmark evaluating models on tasks like cell-type clustering, dimensionality reduction, and denoising. Includes strict resource-consumption metrics. [Website](https://openproblems.bio/)
* **[scRNAseq_Benchmark](https://github.com/tabdelaal/scRNAseq_Benchmark)** Benchmarking unsupervised clustering and classification tools for single-cell RNA-sequencing tabular data.
  * [*A comparison of automatic cell identification methods for single-cell RNA sequencing data* (2019)](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1795-z)

#### 💻 Algorithms & Educational Notebooks
* *(Coming soon: K-Means, DBSCAN, and Spectral Clustering notebooks)*

---

## 🔍 Feature Selection
Evaluating the identification of true signals amidst injected noise and massive dimensionality.

#### 🗄️ Benchmarks
* **[Feature Selection in Tabular DL Benchmark](https://github.com/vcherepanova/tabular-feature-selection)** Specialized environment injecting corrupted and second-order engineered features (Dozens of datasets).
  * [*A Performance-Driven Benchmark for Feature Selection in Tabular Deep Learning* (2023)](https://arxiv.org/abs/2311.05877)

#### 💻 Algorithms & Educational Notebooks
**Filter Methods**
* **ANOVA F-test** - `[View Notebook Example](./notebooks/feature_selection/anova_filter.ipynb)`

**Wrapper Methods**
* **Recursive Feature Elimination (RFE)** - `[View Notebook Example](./notebooks/feature_selection/rfe_wrapper.ipynb)`

**Embedded / Deep Methods**
* **LSPIN** - `[View Notebook Example](./notebooks/feature_selection/lspin_demo.ipynb)`

---

## 🚨 Anomaly Detection
Evaluating algorithms on their ability to identify rare, malicious, or defective instances in tabular datasets (e.g., fraud detection, system failures).

* *(Benchmark suites and notebooks currently under review and will be added shortly)*

---

## ⚖️ Class Imbalance
Evaluating models on skewed datasets where the minority class is critical but easily ignored by standard loss functions.

#### 🗄️ Benchmarks
* **[CLIMB](https://github.com/ZhiningLiu1998/imbalanced-ensemble)** Extreme class imbalance benchmark evaluating state-of-the-art algorithms across 73 datasets.
  * [*CLIMB: A Class Imbalanced Learning Benchmark* (2024)](https://arxiv.org/abs/2505.17451)

---

## 🔗 Relational & Multimodal Learning
Evaluating models on messy enterprise databases, multi-table joins, and tables containing raw text or graph structures.

#### 🗄️ Benchmarks
* **[CARTE Benchmark](https://github.com/soda-inria/carte)** Graph-based solutions for multimodal data (complex strings, raw text) and multi-table joins (51 relational datasets).
  * [*Carte: Pretraining and transfer for tabular learning* (2024)](https://arxiv.org/abs/2402.16785)
* **[TabBench](https://github.com/Neuralk-AI/TabBench)** E-commerce and product cataloging representation learning over proprietary enterprise data structures.
* **[TALENT](https://github.com/LAMDA-Tabular/TALENT)** Massive toolkit officially integrating 35+ deep tabular processing methods (300+ datasets).
