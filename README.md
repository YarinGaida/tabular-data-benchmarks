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
* [🔄 Domain Shift](#-domain-shift)
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
* **[Cancer Multi-Omics Benchmark (MLOmics)](https://github.com/chenzRG/Cancer-Multi-Omics-Benchmark)** Systematic evaluation of machine learning methods for pan-cancer classification and survival prediction using multimodal biological tables.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Supervised Learning on Tabular Data: From Linear Baselines to Foundation Models](./notebooks/supervised_learning/supervisedClassic.ipynb)**
  *(Evaluates LASSO, XGBoost, MLPs, and TabPFN across standard datasets and high-dimensional oncology data).*

---

## 🔄 Domain Shift
Evaluating how models handle temporal changes, feature corruption, and out-of-distribution (OOD) scenarios.

#### 🗄️ Benchmarks (Standard & Biological Data)
* **[TabReD](https://github.com/yandex-research/tabred)** Time-dependent industrial benchmark for evaluating temporal robustness (8 massive datasets).
* **[TableShift](https://github.com/mlfoundations/tableshift)** Out-of-Distribution (OOD) generalization across finance and healthcare tasks (15 datasets). [Website](https://tableshift.org/)
* **[TabFSBench](https://github.com/LAMDASZ-ML/TabFSBench)** Pinpoint feature-shift scenarios simulating upstream data pipeline failures.
* **[scIB & scIB-E](https://github.com/theislab/scib)** The industry standard for evaluating Data Integration and Batch Effect correction across single-cell datasets from different laboratories.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Domain Shift & Data Integration: Handling Non-IID Tabular Data](./notebooks/domain_shift/domain_shift_masterclass.ipynb)**
  *(Demonstrates model degradation over time and strategies for batch-effect removal in biological data).*

---

## 🧩 Clustering
Evaluating unsupervised learning methods to discover hidden groupings, sub-types, and topologies in data without prior labeling.

#### 🗄️ Benchmarks (Standard & Biological Data)
* **[OpenProblems in Single-Cell Analysis](https://github.com/openproblems-bio/openproblems)** A massive, living benchmark evaluating models on tasks like cell-type clustering, dimensionality reduction, and denoising. [Website](https://openproblems.bio/)
* **[scRNAseq_Benchmark](https://github.com/tabdelaal/scRNAseq_Benchmark)** Benchmarking unsupervised clustering and classification tools for single-cell RNA-sequencing tabular data.

#### 💻 Educational Masterclass Notebook
* 🚀 **[Clustering Tabular Data: Uncovering Hidden Structures](./notebooks/clustering/clustering_masterclass.ipynb)**
  *(Explores K-Means, DBSCAN, and Autoencoder-based clustering for cell-type discovery).*

---

## 🔍 Feature Selection
Evaluating the identification of true signals amidst injected noise and massive dimensionality.

#### 🗄️ Benchmarks (Standard Data)
* **[Feature Selection in Tabular DL Benchmark](https://github.com/vcherepanova/tabular-feature-selection)** Specialized environment injecting corrupted and second-order engineered features (Dozens of datasets).

#### 💻 Educational Masterclass Notebook
* 🚀 **[Feature Selection Masterclass: Filter, Wrapper, and Embedded Methods](./notebooks/feature_selection/feature_selection_masterclass.ipynb)**
  *(Features ANOVA, RFE, LASSO, and STG for identifying true signals in high-dimensional and non-linear data).*

---

## 🚨 Anomaly Detection
Evaluating algorithms on their ability to identify rare, malicious, or defective instances in tabular datasets (e.g., fraud detection, system failures).

#### 💻 Educational Masterclass Notebook
* 🚀 **[Anomaly Detection: Finding Needles in Tabular Haystacks](./notebooks/anomaly_detection/anomaly_masterclass.ipynb)**
  *(Currently under development. Will feature Isolation Forests and Autoencoders for rare event detection).*

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
