### Tabular Data Benchmarks
A curated list of modern tabular datasets and benchmark suites focusing on real-world industrial challenges and baseline evaluations.

#### Why Tabular Data Benchmarks?
1. **Reliable evaluations:** Preventing data leakage and metric hacking.
2. **Real-world challenges:** Simulating distribution shifts, missing values, and class imbalance.
3. **The "Deep Learning vs. Trees" debate:** Providing fair comparisons between GBDTs and Neural Networks.
4. **Standardized metrics:** Using robust scoring systems like Elo ratings or normalized scores.

##### Temporal & Distribution Shifts (OOD)
* **[TabReD](https://github.com/yandex-research/tabred)** Time-dependent industrial benchmark for evaluating temporal robustness (8 massive datasets).
  * [*TabReD: Analyzing Pitfalls and Filling the gaps in Tabular Deep Learning Benchmarks* (2024)](https://arxiv.org/abs/2406.19380) Ivan Rubachev, Nikolay Kartashev, Yury Gorishniy, Artem Babenko
* **[TableShift](https://github.com/mlfoundations/tableshift)** Out-of-Distribution (OOD) generalization across finance and healthcare tasks (15 datasets). *(Includes Wild-Tab for regression)*. [Website](https://tableshift.org/)
  * [*TableShift: A Benchmark for Out-of-Distribution Generalization in Tabular Data* (2023)](https://arxiv.org/abs/2312.07577) Josh Gardner, et al.
* **[TabFSBench](https://github.com/LAMDASZ-ML/TabFSBench)** Pinpoint feature-shift scenarios simulating upstream data pipeline failures (Multiple datasets).
  * [*TabFSBench: A Comprehensive Benchmark for Feature Shift in Tabular Data* (2024)](https://icml.cc/virtual/2025/poster/44787)

##### Class Imbalance
* **[CLIMB](https://github.com/ZhiningLiu1998/imbalanced-ensemble)** Extreme class imbalance benchmark evaluating state-of-the-art CIL algorithms (73 datasets).
  * [*CLIMB: A Class Imbalanced Learning Benchmark* (2024)](https://arxiv.org/abs/2505.17451) Zhining Liu, et al.

##### Standard IID & Algorithmic Stress Tests
* **[TabArena](https://github.com/autogluon/tabarena)** A living benchmark with an objective Elo rating system and strict hyperparameter tuning budgets (51 curated datasets). [Website](https://tabarena.ai/)
  * [*TabArena: A Living Benchmark for Machine Learning on Tabular Data* (2025)](https://arxiv.org/abs/2506.16791) Nick Erickson, Lennart Purucker, Andrej Tschalzev, David Holzmüller, Prateek Mutalik Desai, David Salinas, Frank Hutter
* **[TabZilla](https://github.com/naszilla/tabzilla)** Algorithmic stress test specifically featuring the 36 "hardest" datasets (filtered from 176).
  * [*When do neural nets outperform boosted trees on tabular data?* (2023)](https://arxiv.org/abs/2305.02997) D. McElfresh, S. Khandagale, J. Valverde, V. Prasad C, G. Ramakrishnan, M. Goldblum, C. White
* **[Grinsztajn Benchmark](https://github.com/LeoGrin/tabular-benchmark)** The classic 2022 study establishing the Neural Networks vs. Trees baseline (45 datasets).
  * [*Why do tree-based models still outperform deep learning on typical tabular data?* (2022)](https://arxiv.org/abs/2207.08815) Léo Grinsztajn, Edouard Oyallon, Gaël Varoquaux

##### Feature Selection
* **[Feature Selection in Tabular DL Benchmark](https://github.com/vcherepanova/tabular-feature-selection)** Specialized environment injecting corrupted and second-order engineered features (Dozens of datasets).
  * [*A Performance-Driven Benchmark for Feature Selection in Tabular Deep Learning* (2023)](https://arxiv.org/abs/2311.05877) Valeriia Cherepanova, et al.

##### Enterprise, Multimodal & Toolkits
* **[TabBench](https://github.com/Neuralk-AI/TabBench)** E-commerce and product cataloging representation learning over proprietary enterprise data structures (Multiple commercial datasets). [Website](https://dashboard.neuralk-ai.com/)
* **[CARTE Benchmark](https://github.com/soda-inria/carte)** Graph-based solutions for multimodal data (complex strings, raw text) and multi-table joins (51 relational datasets).
  * [*Carte: Pretraining and transfer for tabular learning* (2024)](https://arxiv.org/abs/2402.16785) Myung Jun Kim, Leo Grinsztajn, Gael Varoquaux
* **[TALENT](https://github.com/LAMDA-Tabular/TALENT)** Massive toolkit officially integrating 35+ deep tabular processing methods (300+ datasets).
  * [*TALENT: A Tabular Analytics and Learning Toolbox* (2024)](https://arxiv.org/abs/2407.00956) Si-Yang Liu, Hao-Run Cai, Qi-Le Zhou, Han-Jia Ye
  
* **[LSPIN](https://github.com/jcyang34/lspin)** Locally SParse Interpretable Networks for tabular data.
  * [*Locally Sparse Neural Networks for Tabular Biomedical Data* (2025)](https://arxiv.org/abs/2502.12345) Junchen Yang, Ofir Lindenbaum, Yuval Kluger
