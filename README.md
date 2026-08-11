# healthcare-ai-ml-pipeline
Enterprise-grade MLOps system for predicting patient visit risk and insurance claim outcomes using SQL analytics, XGBoost, FastAPI, MLflow, DVC, and Kubernetes (EKS).

## 🏥 Problem Statement & Overview

Healthcare organizations lose millions annually due to inefficient patient flow and high insurance claim denial rates. This project builds an end-to-end enterprise MLOps platform that integrates **Patient**, **Visit**, and **Billing** data to solve two core healthcare challenges:

1. **Patient Visit Risk Modeling (XGBoost Classifier):**
   - **Goal:** Predict patient risk severity (Low / Medium / High) at intake.
   - **Business Value:** Helps hospital staff manage bed capacity, allocate care resources efficiently, and reduce emergency readmissions.

2. **Claim Outcome Prediction (Revenue Cycle AI):**
   - **Goal:** Predict whether an insurance claim will be **Approved** or **Rejected** prior to submission.
   - **Business Value:** Empowers billing departments to fix flagged claims upfront, lowering rejection rates and improving revenue realization.

---

## 🛠️ Tech Stack & MLOps Architecture

- **Data Analytics & Warehousing:** PostgreSQL / SQL Analytics for ETL, relational joining, and metrics computation.
- **Data & Model Versioning:** DVC (Data Version Control) for dataset tracking and pipeline reproducibility.
- **ML Engine & Experimentation:** XGBoost models tracked with MLflow (parameters, metrics, and model registry).
- **API Serving Layer:** FastAPI asynchronous REST API for low-latency real-time inference.
- **Containerization & Deployment:** Docker containers orchestrated on AWS EKS (Elastic Kubernetes Service).
- **Governance & Monitoring:** Data drift tracking (PSI), feature schema enforcement, and explainable AI.
