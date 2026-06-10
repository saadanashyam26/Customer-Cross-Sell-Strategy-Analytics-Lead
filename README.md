# Portfolio Feature: Insurance Cross-Sell Optimization Analytics

**An Enterprise-Scale Predictive Modeling & Behavioral Segmentation Framework**

---

## 🎯 The Business Challenge
Acquiring new customers is significantly more expensive than cross-selling secondary services to an existing client base. This project addresses a major revenue-expansion challenge within the insurance sector: identifying which existing health insurance policyholders have the highest propensity to purchase vehicle insurance coverage. 

By analyzing behavioral patterns, risk profiles, and demographic variables across a massive customer database, this framework replaces generic marketing outreach with targeted, predictive campaigns—minimizing marketing waste while maximizing cross-selling conversion rates.

---

## 🛠️ Data Infrastructure & Scaling
* **Dataset Scale:** Engineered and processed an enterprise relational database comprising **300,000+ consumer records** containing highly skewed numeric and categorical features.
* **Big Data Execution:** Leveraged **PySpark Distributed DataFrames** to handle intensive computational loads, applying `StringIndexer` for categorical feature encoding and `StandardScaler` for robust numerical scaling.
* **Pipeline Automation:** Built automated preprocessing validation pipelines to systematically clean, normalize, and transform raw demographic variables into model-ready analytical inputs.

---

## 🧠 Model Architecture & Technical Strategy

The analytical engine executes a dual-layer strategy using unsupervised machine learning for behavioral positioning and supervised learning for conversion prediction:

### 1. Behavioral Customer Profiling (K-Means Clustering)
* Applied **Principal Component Analysis (PCA)** to reduce multidimensional customer vectors into visualizable components while maintaining structural variance.
* Implemented **K-Means Clustering** optimized via the **Silhouette Score** to mathematically partition the consumer base into 5 distinct behavioral profiles (Premium Buyers, Cost-Conscious, Risk-Averse, First-Time Buyers, and Loyalists) to drive personalized campaign structures.

### 2. Predictive Analytics Engine (XGBoost Classifier)
* **Class Imbalance Handling:** Addressed extreme target variable class imbalances using Synthetic Minority Over-sampling Technique (**SMOTE**) to prevent algorithmic bias.
* **Predictive Modeling:** Deployed an **XGBoost Classifier** to map and predict purchase intent, generating exceptional performance quantified via optimized **AUC-ROC** metrics.
* **Statistical Associations:** Utilized correlation matrices and feature importance metrics to isolate key revenue-driving triggers.
