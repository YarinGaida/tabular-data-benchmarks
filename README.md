# Tabular Data Benchmarks & Algorithms

A curated hub of modern tabular datasets, benchmark suites, and educational notebooks focusing on real-world machine learning challenges.

> Tabular data is structured data organized in a table format, representing the most common data type in real-world AI applications. Benchmark suites standardize the evaluation of machine learning models on these datasets.

#### Why tabular data benchmarks?
1. Standardized evaluation (Unified metrics across the industry)
2. Real-world robustness (Testing on shifting, imbalanced, and messy data)
3. Reproducible research (Preventing biased testing)
4. Fair model comparison (e.g., Deep Learning vs. Trees)

---

## Standard IID & Algorithmic Stress Tests
Evaluating models under standard conditions to expose pure architectural disparities.

#### Benchmarks
* **[TabArena](https://github.com/autogluon/tabarena)** A living benchmark with an objective Elo rating system and strict hyperparameter tuning budgets (51 curated datasets). [Website](https://tabarena.ai/)
  * [*TabArena: A Living Benchmark for Machine Learning on Tabular Data* (2025)](https://arxiv.org/abs/2506.16791) Nick Erickson, et al.
* **[TabZilla](https://github.com/naszilla/tabzilla)** Algorithmic stress test specifically featuring the 36 "hardest" datasets (filtered from 176).
  * [*When do neural nets outperform boosted trees on tabular data?* (2023)](https://arxiv.org/abs/2305.02997) D. McElfresh, et al.
* **[Grinsztajn Benchmark](https://github.com/LeoGrin/tabular-benchmark)** The classic 2022 study establishing the Neural Networks vs. Trees baseline (45 datasets).
  * [*Why do tree-based models still outperform deep learning on typical tabular data?* (2022)](https://arxiv.org/abs/2207.08815) Léo Grinsztajn, et al.

#### Algorithms & Educational Notebooks
**Classic Methods**
* **Logistic Regression** - `[View Notebook Example](./notebooks/supervised/logistic_regression.ipynb)`
* **Gradient Boosted Trees (XGBoost/LightGBM)** - `[View Notebook Example](./notebooks/supervised/xgboost_example.ipynb)`

**Deep Learning Methods**
* **Multi-Layer Perceptron (MLP)** - `[View Notebook Example](./notebooks/deep/mlp_example.ipynb)`
* **TabPFN** - `[View Notebook Example](./notebooks/deep/tabpfn_example.ipynb)`

---

## Feature Selection
Evaluating the identification of true signals amidst injected noise.

#### Benchmarks
* **[Feature Selection in Tabular DL Benchmark](https://github.com/vcherepanova/tabular-feature-selection)** Specialized environment injecting corrupted and second-order engineered features (Dozens of datasets).
  * [*A Performance-Driven Benchmark for Feature Selection in Tabular Deep Learning* (2023)](https://arxiv.org/abs/2311.05877) Valeriia Cherepanova, et al.

#### Algorithms & Educational Notebooks
**Filter Methods**
* **ANOVA F-test** - `[View Notebook Example](./notebooks/feature_selection/anova_filter.ipynb)`

**Wrapper Methods**
* **Recursive Feature Elimination (RFE)** - `[View Notebook Example](./notebooks/feature_selection/rfe_wrapper.ipynb)`

**Embedded / Deep Methods**
* **LSPIN** - `[View Notebook Example](./notebooks/feature_selection/lspin_demo.ipynb)`

---

## Temporal & Distribution Shifts (OOD)
#### Benchmarks
* **[TabReD](https://github.com/yandex-research/tabred)** Time-dependent industrial benchmark for evaluating temporal robustness (8 massive datasets).
  * [*TabReD: Analyzing Pitfalls and Filling the gaps in Tabular Deep Learning Benchmarks* (2024)](https://arxiv.org/abs/2406.19380) Ivan Rubachev, et al.
* **[TableShift](https://github.com/mlfoundations/tableshift)** Out-of-Distribution (OOD) generalization across finance and healthcare tasks (15 datasets). *(Includes Wild-Tab for regression)*. [Website](https://tableshift.org/)
  * [*TableShift: A Benchmark for Out-of-Distribution Generalization in Tabular Data* (2023)](https://arxiv.org/abs/2312.07577) Josh Gardner, et al.
* **[TabFSBench](https://github.com/LAMDASZ-ML/TabFSBench)** Pinpoint feature-shift scenarios simulating upstream data pipeline failures (Multiple datasets).
  * [*TabFSBench: A Comprehensive Benchmark for Feature Shift in Tabular Data* (2024)](https://icml.cc/virtual/2025/poster/44787)

---

## Class Imbalance
#### Benchmarks
* **[CLIMB](https://github.com/ZhiningLiu1998/imbalanced-ensemble)** Extreme class imbalance benchmark evaluating state-of-the-art CIL algorithms (73 datasets).
  * [*CLIMB: A Class Imbalanced Learning Benchmark* (2024)](https://arxiv.org/abs/2505.17451) Zhining Liu, et al.

---

## Biological & Scientific Data (Omics & scRNA-seq)
#### Benchmarks
* **[scRNAseq_Benchmark](https://github.com/tabdelaal/scRNAseq_Benchmark)** Benchmarking classification tools for single-cell RNA-sequencing tabular data.
  * [*A comparison of automatic cell identification methods for single-cell RNA sequencing data* (2019)](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1795-z)
* **[Cancer Multi-Omics Benchmark](https://github.com/BiomedicalMachineLearning/MultiOmicsBenchmark)** Systematic evaluation of machine learning methods for multi-omics biomarker discovery.

#### Algorithms & Educational Notebooks
* *(Coming soon: Tutorials for biological tabular processing)*

---

## Enterprise, Multimodal & Toolkits
#### Benchmarks
* **[TabBench](https://github.com/Neuralk-AI/TabBench)** E-commerce and product cataloging representation learning over proprietary enterprise data structures (Multiple commercial datasets). [Website](https://dashboard.neuralk-ai.com/)
* **[CARTE Benchmark](https://github.com/soda-inria/carte)** Graph-based solutions for multimodal data (complex strings, raw text) and multi-table joins (51 relational datasets).
  * [*Carte: Pretraining and transfer for tabular learning* (2024)](https://arxiv.org/abs/2402.16785) Myung Jun Kim, et al.
* **[TALENT](https://github.com/LAMDA-Tabular/TALENT)** Massive toolkit officially integrating 35+ deep tabular processing methods (300+ datasets).
  * [*TALENT: A Tabular Analytics and Learning Toolbox* (2024)](https://arxiv.org/abs/2407.00956) Si-Yang Liu, et al.
