&#x20;README.md

\# Spaceship Titanic High-Generalization Spatiotemporal Collaborative Prediction System



This repository provides a high-precision, production-grade solution for the classic Kaggle machine learning task, \*Spaceship Titanic\*. By deeply mining group spatiotemporal correlations, deploying unsupervised anomaly filtering, and incorporating proprietary post-processing algorithms, the system achieves ultimate generalization performance on unseen test datasets.



\---



\## 🛠️ 1. Environment Setup \& Dependencies



The system is developed and validated on the `Python 3.13` platform. Before running the Jupyter Notebook, please ensure that the following core frameworks are installed:



\### Core Dependencies (Required to run the code)

\* \*\*Pandas\*\*: Advanced multi-dimensional structured data cleansing and feature alignment.

\* \*\*NumPy\*\*: Vectorized mathematical acceleration for multi-dimensional matrices.

\* \*\*XGBoost\*\*: High-performance gradient boosting decision tree core engine.

\* \*\*Scikit-Learn\*\*: Governs unsupervised anomaly cleansing via `IsolationForest` and standard imputation transformers.



\### 🌟 Offline Optimization Tool (NOT required for running)

\* \*\*Optuna (Bayesian Optimization Framework)\*\*: This tool was heavily utilized during our \*\*offline hyperparameter search phase\*\* to discover the optimal global parameters. 

&#x20; > ⚠️ \*\*Engineering Note:\*\* To keep the production inference pipeline clean and fast, the messy training logs and Optuna dependencies have been completely decoupled. The verified optimal weights are hardcoded directly into `submission.ipynb`. Therefore, \*\*Optuna is intentionally excluded from `requirements.txt`\*\* and you do NOT need to install it to run this repository.



\### One-Click Installation Command

Run the following command in your Terminal or Anaconda Prompt to automatically configure the environment:

```bash

pip install -r requirements.txt

