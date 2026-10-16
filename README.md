# Awesome-Automl-Hyperparameter-Tuning

## Top AutoML & Hyperparameter Tuning Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Neural Architecture Search, Bayesian Optimization & Kubernetes-Native Tuning*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **AutoML & Hyperparameter Tuning**. These tools enable data scientists and ML engineers to automate model selection, feature engineering, and hyperparameter optimization—turning manual trial-and-error into systematic, reproducible search.



**Examples** include Google Cloud Vertex AI Vizier, AWS SageMaker Autopilot, SigOpt (Intel), Ray Tune, Optuna, Weights & Biases Sweeps, DataRobot, H2O Driverless AI, Neptune.ai, and ClearML (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, distributed tuning, and open AutoML—ideal for ML engineers, data scientists, and organizations seeking transparent, vendor-independent optimization.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Google Cloud Vertex AI Vizier](https://cloud.google.com/vertex-ai)**  

  **Google's black-box hyperparameter tuning service** integrated with Vertex AI. Features **Bayesian optimization** with transfer learning across studies. Handles **multi-objective optimization** and **parallel trials** natively. **Per-node-hour pricing**—costs scale with dataset size and trial count .



- **[AWS SageMaker Autopilot](https://aws.amazon.com/sagemaker/autopilot/)**  

  **Fully managed AutoML** that automatically explores data, selects algorithms, and tunes hyperparameters. Features **transparent model explanations** and **deployment-ready artifacts**. Integrated with SageMaker Studio for end-to-end ML workflows.



- **[SigOpt (Intel)](https://sigopt.com/)**  

  **Enterprise hyperparameter optimization** with **Bayesian optimization**, **multi-metric optimization**, and **early stopping**. Features **experiment tracking** and **ensemble strategies**. Acquired by Intel for enterprise AI tuning.



- **[Weights & Biases Sweeps](https://wandb.ai/)**  

  **Experiment tracking with hyperparameter sweeps** integrated into the W&B platform. Features **Bayesian, random, and grid search**, **early termination** (Hyperband), and **visualization** of sweep results. **The most widely used experiment tracking platform** with tuning built in.



- **[DataRobot](https://www.datarobot.com/)**  

  **Enterprise AutoML platform** with **model monitoring, challenger comparison, and compliance documentation** . Features **LLM fine-tuning workflows** (2025–2026 releases). **The enterprise governance play**—justifies cost for large institutions managing regulatory risk .



- **[H2O Driverless AI](https://h2o.ai/platform/ai-cloud/make/h2o-driverless-ai/)**  

  **Automatic machine learning platform** with **feature engineering, model selection, and hyperparameter tuning**. Features **MOJO export** for deployment without cloud dependency .



- **[Neptune.ai](https://neptune.ai/)**  

  **Experiment tracking and model registry** for ML teams. Features **hyperparameter logging**, **comparison dashboards**, and **integration with major frameworks**.



- **[ClearML](https://clear. ml/)**  

  **Open-source MLOps platform** with **experiment management**, **hyperparameter optimization**, and **pipeline orchestration**. Features **auto-scaler** for cloud GPU provisioning and **model serving**.



## Open-Source GitHub Projects



- **[Katib (Kubeflow)](https://github.com/kubeflow/katib)**  

  **Kubernetes-native Hyperparameter Tuning and Neural Architecture Search** (Apache-2.0) . **The reference implementation for cloud-native AutoML** . **Architecture**: **Experiment** (single tuning run with objective, search space, search algorithm), **Suggestion** (proposed hyperparameter values), **Trial** (one iteration with worker job instance), **Worker** (process evaluating a Trial) . **Search algorithms**: **Bayesian Optimization, Random Search, Grid Search, Hyperband, Population-Based Training (PBT), and more** . **Python SDK** with `katib_client.tune()` for programmatic experiment creation . **YAML-based Experiment specification** for declarative configuration . **NAS support** (alpha) for neural architecture search . **Dashboard UI** (`katib-ui`) and **MySQL backend** (`katib-mysql`) for metrics storage . **The best choice for teams running Kubeflow or Kubernetes-native ML pipelines**—integrates with existing cluster infrastructure without additional orchestration overhead.



- **[Optuna](https://github.com/optuna/optuna)**  

  **The most widely adopted open-source hyperparameter optimization framework** (MIT) . **14,650+ GitHub stars** . **Define-by-run API**—search spaces are Python code, not static configs. **Pruning algorithms** (Median, Hyperband, ASHA, Successive Halving) for early termination of unpromising trials. **Distributed optimization** with support for parallel and distributed training. **Visualization** with Plotly-based interactive plots. **Integration with PyTorch, TensorFlow, Keras, scikit-learn, XGBoost, LightGBM, and more**. **The default choice for general HPO**—easy to learn, powerful enough for production .



- **[Ray Tune](https://github.com/ray-project/ray)**  

  **Scalable hyperparameter tuning built on Ray** (Apache-2.0) . **Multi-fidelity optimization** (ASHA, Hyperband, Population-Based Training). **Distributed execution** across clusters with automatic fault tolerance. **Integration with PyTorch, TensorFlow, XGBoost, and more**. **Best for large-scale tuning**—when you need to search thousands of configurations across multiple machines .



- **[MLJAR AutoML](https://github.com/mljar/mljar-supervised)**  

  **Tabular AutoML with reports, explanations, feature engineering, tuning, stacking, and ensembling** (Apache-2.0) . **Powered by mljar-supervised**. **Built around reports and explainability from the beginning**—gives you models, reports, explanations, and artifacts that can be reviewed later . **Best for privacy-sensitive, explainable, local business modeling** .



- **[AutoGluon](https://github.com/autogluon/autogluon)**  

  **Fast and accurate ML in 3 lines of code** (Apache-2.0) . **10,594+ GitHub stars** . **Broadest open-source coverage**—tabular, time series, multimodal, and foundation-model support . **Multi-layer stacking and automatic feature engineering**. **Best for maximum benchmark performance and broad task coverage** .



- **[FLAML](https://github.com/microsoft/FLAML)**  

  **Resource-aware AutoML and tuning** (MIT). **Fast, budget-aware model search**—excellent when compute budget and training time matter . **Lightweight and efficient** with support for classification, regression, and time series.



- **[TPOT](https://github.com/EpistasisLab/tpot)**  

  **Genetic programming for pipeline search** (LGPL-3.0) . **10,049+ GitHub stars** . **Outputs scikit-learn code** that teams can read and modify . **Competitive with H2O, weaker than Auto-sklearn** on accuracy . **Best for discovering pipeline structures** and interpretable ML pipelines .



- **[H2O AutoML](https://github.com/h2oai/h2o-3)**  

  **Distributed enterprise AutoML** with algorithm portfolios and stacked ensembles (Apache-2.0) . **Fastest open-source option**—trains models in 5–10 minutes typically . **Competitive accuracy on tabular data**. **Best for scalable tabular ML in enterprise environments** .



- **[Auto-sklearn](https://github.com/automl/auto-sklearn)**  

  **Automated machine learning with scikit-learn** (BSD-3-Clause) . **8,128+ GitHub stars** . **Bayesian optimization, meta-learning, ensemble selection**. **Often wins competitions**—5–15% better than H2O on hard problems . **Requires serious CPU** (16+ cores recommended) . **No recent major release**—latest official release from 2023 .



- **[Hyperopt](https://github.com/hyperopt/hyperopt)**  

  **Distributed asynchronous hyperparameter optimization** (BSD-3-Clause) . **7,598+ GitHub stars** . **The original Bayesian optimization library for Python**. **Tree-structured Parzen Estimator (TPE)** algorithm. **Foundation for many other tuning frameworks**.



- **[Optuna Dashboard](https://github.com/optuna/optuna-dashboard)**  

  **Real-time web dashboard for Optuna** (MIT) . **796+ GitHub stars** . **Visualize optimization history, parameter importance, and intermediate values**. **The standard companion tool for Optuna-based tuning**.



### Additional Strong Open-Source Options



- **[NNI (Microsoft)](https://github.com/microsoft/nni)** — Neural Network Intelligence (MIT) . **14,365+ GitHub stars** . **Automates feature engineering, neural architecture search, model compression, and hyperparameter tuning**.

- **[PyCaret](https://github.com/pycaret/pycaret)** — Open-source, low-code AutoML platform (MIT) . **9,836+ GitHub stars** . **PyCaret 4.0**: sklearn-native engine + React control plane .

- **[MLflow](https://github.com/mlflow/mlflow)** — Open source AI engineering platform (Apache-2.0) . **27,484+ GitHub stars** . **Experiment tracking, model registry, and deployment**.

- **[AIDE ML](https://github.com/WecoAI/aideml)** — Agent that writes, runs, debugs, and improves ML code (MIT) . **Autonomous ML engineering research**—needs careful review and compute control .

- Community **n8n** workflows for tuning job scheduling and model deployment automation.



**Frameworks for building custom systems**: Combine **Optuna** for general HPO with **Ray Tune** for distributed tuning, **Katib** for Kubernetes-native AutoML, **MLJAR AutoML** for explainable tabular modeling, and **AutoGluon** for broad task coverage—creating a fully self-hosted, enterprise-grade AutoML platform.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- AutoML and hyperparameter tuning systems handling training data must comply with data protection regulations (GDPR, CCPA, etc.) and model licensing terms.

- **Open-source AutoML is mature and production-ready.** Optuna (14K+ stars) is the default choice for general HPO . Ray Tune scales to clusters . Katib provides Kubernetes-native AutoML . AutoGluon delivers broad task coverage . **These are genuine alternatives to commercial platforms.**

- **The right tool depends on your deployment environment, not the benchmark leaderboard.** "The best model is the one your team can monitor and retrain without external help" . **Choose based on operational fit, not accuracy alone.**

- **auto-sklearn has no recent major release.** Latest official release from 2023 . **Not recommended as default for new production projects in 2026**—but historically important for legacy baselines .

- **Tabular foundation models are emerging but gradient boosting remains strong.** "Large tabular datasets, strict latency requirements, custom feature engineering, and interpretability needs still make gradient boosting very strong" .

- Self-hosted open-source solutions require proper compute provisioning, experiment tracking infrastructure, and ongoing maintenance. **AutoML is not a substitute for ML expertise**—it automates search, not problem formulation.
