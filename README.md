### **CDC Disease Forecasting Pipeline – Data Engineering & MLOps**

This repository contains a **fully automated pipeline** for extracting, processing, and forecasting CDC disease occurrence data. The project integrates **Google Cloud SDK, Cloud Functions, BigQuery, Cloud Storage, and Prefect Cloud** to streamline ETL and MLOps processes. It generates **8-week SARIMA-based forecasts** and updates interactive dashboards in **Looker Studio**.

#### **⚠️ Note: This is a Forked and Renamed Repository**
This is **not the original repository** but retains **all commit history and contributions** from the original project.  
The original repository can be found here: **[Olivia-Peng/BA882-pipeline_G10](https://github.com/Olivia-Peng/BA882-pipeline_G10.git).**

---

## **🔹 Project Overview**
### **1️⃣ Data Engineering Pipeline**
- **Extracts CDC disease data** from `.txt` files and stores them in **Google Cloud Storage**.
- **Processes and transforms the data** into structured **Parquet** format.
- **Loads the data into BigQuery**, managing schema creation, deduplication, and validation.
- **Orchestrated with Prefect Cloud**, ensuring smooth, automated execution.

### **2️⃣ MLOps Pipeline**
- **Retrieves processed data** from BigQuery for machine learning.
- **Performs automated SARIMA hyperparameter tuning** using Google Cloud Run.
- **Trains models** dynamically based on disease codes.
- **Generates 8-week disease occurrence predictions** and logs results in BigQuery.
- **Deploys Looker Studio dashboards**, updating forecasts weekly.

---

## **📁 Project Structure**
- `/functions/` – Google Cloud Functions for ETL and MLOps automation.
- `/flows/` – Prefect Cloud workflows orchestrating pipeline execution.
- `/mlops-pipeline/` – Model training, hyperparameter tuning, and prediction scripts.
- `/deploy-scripts/` – Deployment scripts for automating cloud infrastructure setup.

---

## **🚀 Technologies Used**
✅ **Google Cloud Platform (GCP)** – Cloud Functions, BigQuery, Cloud Storage  
✅ **Prefect Cloud** – ETL orchestration  
✅ **SARIMA Forecasting** – Time series modeling  
✅ **GitHub Actions** – Version control and CI/CD  

---

## **📊 Key Features**
✔ **Automated Data Ingestion** – Weekly CDC disease extraction  
✔ **Dynamic Data Processing** – Schema validation, deduplication, and transformation  
✔ **MLOps Integration** – Continuous SARIMA training & prediction  
✔ **Scalable Architecture** – Designed for expansion to multiple diseases  

---

## **📜 Acknowledgments**
This project was originally developed as part of **BA882 – Advanced Business Analytics** at Boston University.  
Contributors: **Victor Floriano** (victor-floriano), **Olivia Peng** (Olivia-Peng), **Tiancheng Yang** (lilchengzi), **Jessica Tong** (eshentong)

For questions, feel free to reach out! ✉️

---

### **📌 Next Steps**
✅ Add usage instructions if needed  
✅ Update deployment scripts for easier setup  

---

Let me know if you'd like to tweak anything! 🚀
