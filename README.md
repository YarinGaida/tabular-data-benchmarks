# Tabular Data Benchmarks

A curated list of modern tabular datasets and benchmark suites focusing on real-world industrial challenges and baseline evaluations.

## Temporal & Distribution Shifts (OOD)
* **[TabReD](https://github.com/yandex-research/tabred)** - Time-dependent industrial datasets for evaluating temporal robustness. | [Paper](https://arxiv.org/abs/2406.19380)
* **[TableShift](https://github.com/mlfoundations/tableshift)** - Out-of-Distribution (OOD) generalization across finance and healthcare tasks. *(Includes Wild-Tab for regression).* | [Paper](https://arxiv.org/abs/2312.07577) | [Website](https://tableshift.org/)
* **[TabFSBench](https://github.com/LAMDASZ-ML/TabFSBench)** - Pinpoint feature-shift scenarios simulating upstream data pipeline failures. | [Paper](https://icml.cc/virtual/2025/poster/44787)

## Class Imbalance
* **[CLIMB](https://github.com/ZhiningLiu1998/imbalanced-ensemble)** - Extreme class imbalance benchmark (73 datasets) evaluating state-of-the-art CIL algorithms. | [Paper](https://arxiv.org/abs/2505.17451)

## Standard IID & Algorithmic Stress Tests
* **[TabArena](https://github.com/autogluon/tabarena)** - A living benchmark with an objective Elo rating system and strict hyperparameter tuning budgets. | [Paper](https://arxiv.org/abs/2506.16791) | [Website](https://tabarena.ai/)
* **[TabZilla](https://github.com/naszilla/tabzilla)** - Algorithmic stress test featuring the 36 "hardest" tabular datasets. | [Paper](https://arxiv.org/abs/2305.02997)
* *(Historical Note)* **[Grinsztajn Benchmark](https://github.com/LeoGrin/tabular-benchmark)** - The classic 2022 study establishing the Neural Networks vs. Trees baseline. | [Paper](https://arxiv.org/abs/2207.08815)

## Feature Selection
* **[Feature Selection in Tabular DL Benchmark](https://github.com/vcherepanova/tabular-feature-selection)** - Specialized environment injecting corrupted and second-order engineered features. | [Paper](https://arxiv.org/abs/2311.05877)

## Enterprise, Multimodal & Toolkits
* **[TabBench](https://github.com/Neuralk-AI/TabBench)** - E-commerce and product cataloging representation learning over proprietary enterprise data structures. | [Website](https://dashboard.neuralk-ai.com/)
* **[CARTE Benchmark](https://github.com/soda-inria/carte)** - Graph-based solutions for multimodal data (complex strings, raw text) and multi-table joins. | [Paper](https://arxiv.org/abs/2402.16785)
* **[TALENT](https://github.com/LAMDA-Tabular/TALENT)** - Massive toolkit providing over 300 datasets and officially integrating 35+ deep tabular processing methods. | [Paper](https://arxiv.org/abs/2407.00956)
