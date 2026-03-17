# Awesome Tabular Machine Learning Benchmarks 📊

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)

A curated list of modern benchmarks, datasets, and suites for rigorously evaluating Machine Learning models (Neural Networks, GBDTs, AutoML) on tabular data.

## ⚡ Quick Comparison (TL;DR)

| Benchmark Suite | Datasets | Tasks | Data Profile | Current Top Baselines |
|-----------------|----------|-------|--------------|-----------------------|
| **[TabArena](#living--dynamic-benchmarks)** | 51 | Classification | Clean, Medium-sized, No Leaks | CatBoost, XGBoost |
| **[TabZilla](#deep-learning-vs-tree-models)** | 36 | Class. / Reg. | Highly Difficult, Mixed features | CatBoost, TabPFN |
| **[Grinsztajn](#deep-learning-vs-tree-models)** | 45 | Class. / Reg. | Medium-sized, No missing values | XGBoost, Random Forest |
| **[OpenML-CC18](#foundational--automl-suites)**| 72 | Classification | Highly Diverse, Foundational | AutoGluon, Random Forest|
| **[AMLB](#foundational--automl-suites)** | 100+ | Class. / Reg. | Raw, Missing values, Categorical | AutoGluon, H2O AutoML |

---

## 🚀 Quick Start: The Unified DataLoader

Stop writing custom data preparation scripts for every benchmark. Use our lab's unified dataloader to fetch, clean, and format datasets instantly:

```python
from lab_tabular_tools import BenchmarkLoader

# Load any dataset from any benchmark ready for training
X_train, X_test, y_train, y_test = BenchmarkLoader.load(
    benchmark="TabZilla", 
    dataset_name="credit-g",
    return_format="pandas" # Supports 'pandas', 'numpy', or 'torch'
)
```
*(Note: The full DataLoader code repository is coming soon!)*

---

## 📖 Detailed Benchmark List

### Living & Dynamic Benchmarks

* **[TabArena](https://github.com/autogluon/tabarena)** | [Website](https://tabarena.ai/)
  * **Paper:** [TabArena: A Living Benchmark for Tabular Data](https://arxiv.org/abs/2506.16791)
  * **Focus:** A continuously updated Elo rating system enforcing a strict, identical hyperparameter tuning budget.
  * **Data Characteristics:** 51 datasets heavily filtered for zero data leakage. Cleaned and standardized.
  * **Key Baseline:** CatBoost currently holds a strong position when tuning budgets are strictly controlled.

### Deep Learning vs. Tree Models

* **[TabZilla](https://github.com/naszilla/tabzilla)**
  * **Paper:** [When Do Neural Nets Outperform Boosted Trees on Tabular Data?](https://arxiv.org/abs/2305.02997)
  * **Focus:** Exposes the performance disparities between NNs and GBDTs. Identifies exactly where deep learning struggles or shines.
  * **Data Characteristics:** The 36 "hardest" datasets from an initial pool of 176. Contains complex features and challenging distributions.
  * **Key Baseline:** TabPFN and CatBoost show remarkable performance on this highly difficult suite.

* **[Grinsztajn Benchmark](https://github.com/LeoGrin/tabular-benchmark)**
  * **Paper:** [Why do tree-based models still outperform deep learning on typical tabular data?](https://arxiv.org/abs/2207.08815)
  * **Focus:** Rigorous testing ground to understand the architectural advantages of tree-based models over Neural Networks.
  * **Data Characteristics:** 45 medium-sized datasets. Specifically filtered to remove uninformative features and missing values.
  * **Key Baseline:** XGBoost and Random Forests consistently set the benchmark here.

### Foundational & AutoML Suites

* **[OpenML-CC18](https://www.openml.org/s/99)**
  * **Paper:** [OpenML Benchmarking Suites](https://arxiv.org/abs/1902.04289)
  * **Focus:** The "gold standard" curated classification suite. Evaluates generalizability across highly diverse domains.
  * **Data Characteristics:** 72 rigorously verified classification datasets of varying sizes and domains.
  * **Key Baseline:** Modern AutoML tools (like AutoGluon) and ensemble methods.

* **[AMLB (AutoML Benchmark)](https://github.com/openml/automlbenchmark)**
  * **Paper:** [AMLB: An Auto-ML Benchmark](https://arxiv.org/abs/2207.12560)
  * **Focus:** Targets out-of-the-box performance and robustness. Tests how models handle raw data without manual preprocessing.
  * **Data Characteristics:** Multiple suites handling raw text, missing values, and high-cardinality categoricals.
  * **Key Baseline:** Top-tier AutoML frameworks (AutoGluon, H2O, LightGBM).

---

## 🤝 Contributing
Contributions are welcome! If you know of a high-quality tabular benchmark that should be on this list, or want to add a new baseline result, please open a pull request or submit an issue.
