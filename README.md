# Credit-Card-Fraud-Detection-using-Hybrid-Anomaly-Classical-Ensemble-with-Explainability
Anomaly-aware fraud detection system leveraging Autoencoder + XGBoost with Optuna-tuned thresholds and LIME/SHAP interpretability.

> **High-Recall, Low-False Positive Fraud Detection Pipeline using Unsupervised-Supervised Hybrid Models with Full Interpretability.**

---

## 📌 Project Overview

This project presents a **cutting-edge credit card fraud detection pipeline** built on the **Kaggle Credit Card Fraud Dataset** — a real-world, highly imbalanced dataset where only **0.172%** of the transactions are fraudulent.

To tackle this extreme class imbalance and uncover both known and novel fraud patterns, I designed a **hybrid detection system** that combines:

* **Autoencoder-based anomaly detection** (unsupervised)
* **XGBoost-based fraud classification** (supervised)
* **Optuna-based hyperparameter & ensemble weight tuning**
* **Youden’s J-based threshold calibration**
* **LIME & SHAP-based explainability tools**

This holistic system not only achieves high fraud detection performance but also provides actionable transparency to risk analysts and business teams.

---

## 🧠 What’s Inside?

📁 You’ll find everything in a **single notebook**:

> 📄 `Fraud_Detection_Autoencoder_XGBoost.ipynb`

**It covers:**

* End-to-end data preprocessing
* Model architecture design (Autoencoder + XGBoost)
* Threshold calibration
* Ensemble logic
* Extensive model evaluation
* Visual explainability using SHAP and LIME

---

## 🎯 Results

| Metric        | Value  |
| ------------- | ------ |
| **ROC AUC**   | 0.976  |
| **Precision** | 90.3%  |
| **Recall**    | 85.7%  |
| **F1 Score**  | 0.8796 |


* ✅ **Hybrid Ensemble** → **Best Performance with Explainability**

---

## 🏆 Why This Project Matters

* 💰 **Fraud Detection Saves Millions**: Catching high-value fraudulent transactions early reduces chargebacks and reputational damage.
* ⚠️ **Highly Imbalanced Data**: Only 492 frauds in 284,807 transactions—making naive classification useless.
* 🧠 **Hybrid Thinking**: Combines pattern recognition (XGBoost) and anomaly detection (Autoencoder) to capture unknown fraud patterns.
* 🧪 **Explainability**: LIME and SHAP enhance trust and help stakeholders interpret decisions clearly.
* ⚙️ **Calibration Matters**: Threshold tuning using **Youden’s J** ensures high recall with low false positives—crucial in cost-sensitive applications.

---

## 📊 Dataset

* **Name**: Kaggle Credit Card Fraud Detection Dataset (by ULB & Worldline)
* **Type**: Real, anonymized transactional data (PCA applied)
* **Details**:

  * 284,807 transactions over 2 days
  * 492 labeled as fraud (0.172%)
  * Features: `V1` to `V28` (PCA), `Amount`, `Time`, and `Class`

🔗 [Dataset Source](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)

---

## 🧠 Technical Stack

| Component           | Tools & Techniques                                                        |
| ------------------- | ------------------------------------------------------------------------- |
| Data Preprocessing  | `Pandas`, `Scikit-learn`, `MinMaxScaler`, `PCA`                           |
| Anomaly Detection   | `Autoencoder` with `Keras` – Gaussian Noise, L1, Dropout, BatchNorm       |
| Classification      | `XGBoost` – Gradient Boosted Trees                                        |
| Ensemble Tuning     | `Optuna` – for both model tuning and ensemble weight optimization         |
| Threshold Selection | `Youden’s J Statistic` – to calibrate final decision threshold            |
| Model Evaluation    | `Confusion Matrix`, `ROC`, `PR Curve`, `Precision`, `Recall`, `F1`, `AUC` |
| Explainability      | `SHAP` for global insights, `LIME` for local predictions                  |

---

## 🔍 Interpretability: SHAP & LIME

* **SHAP (SHapley Additive exPlanations)**: Used to visualize which features contributed most to fraud predictions across the dataset.
* **LIME (Local Interpretable Model-Agnostic Explanations)**: Used to understand individual decisions—useful for fraud analysts.



---

## ✅ Usage

Download the notebook and run in Jupyter Lab / Google Colab:



---

## 📌 Future Enhancements

* 🛰️ Real-time alerting engine for live fraud scoring
* 🧪 Integration of adversarial/synthetic attacks to test robustness
* 🌐 Streamlit dashboard for business team interaction
* 🧾 Add cost-sensitive learning for transaction-level decisioning

---

## 🙋‍♂️ Author

**Kheer Sagar Patel**
Graduate Research Assistant – M.Tech (CSE) @ IIITDM Jabalpur 
Specialization: AI & ML 
| B.Tech – BIT Durg



---

