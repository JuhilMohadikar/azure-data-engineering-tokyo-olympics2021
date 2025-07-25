# Azure Data Engineering Project – Tokyo Olympics 2021

## Introduction

A comprehensive data engineering project on **Microsoft Azure** using the **Tokyo Olympics 2021** dataset. This project showcases the implementation of an end-to-end data pipeline leveraging key Azure services including **Azure Data Factory (ADF)**, **Azure Data Lake Storage Gen2**, **Azure Databricks**, and **Azure Synapse Analytics**.

## Architecture 
![Project Architecture](Architecture.jpg)


---

## 🔧 Tools & Technologies Used

| Technology              | Purpose                                       |
|------------------------|-----------------------------------------------|
| Azure Data Factory     | Ingestion pipeline and data orchestration     |
| ADLS Gen2              | Scalable storage for raw and processed data   |
| Azure Databricks       | Data transformation using PySpark             |
| Azure Synapse Analytics| Final querying and analytics layer            |


---

## 📊 Dataset Overview
This data contains the details of over 11,000 athletes, with 47 disciplines, along with 743 Teams taking part in the 2021(2020) Tokyo Olympics.
This dataset contains the details of the Athletes, Coaches, Teams participating as well as the Entries by gender. It contains their names, countries represented, discipline, gender of competitors, name of the coaches.

- Source: [Kaggle - 2021 Olympics in Tokyo](https://www.kaggle.com/datasets)

---

## 🔄 Data Flow Architecture

1. **Data Ingestion**  
   - Raw CSV files uploaded to **ADLS Gen2** (`raw-data/` folder)

2. **Orchestration with ADF**  
   - **Azure Data Factory** pipelines used to copy data to lake

3. **Data Transformation**  
   - **Databricks Notebooks** used for cleaning, type casting and enrichment
   - Output stored in `transformed-data/` folder

4. **Analytics Layer**  
   - Cleaned data queried in **Azure Synapse Analytics** using serverless SQL pools

---

## 🚀 Key Features

- End-to-end Azure-native data pipeline
- Scalable and modular folder structure
- Reusable PySpark transformation logic
- Structured output ready for reporting

---

## 📂 How to Run This Project

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/azure-data-engineering-tokyo-olympics2021.git
