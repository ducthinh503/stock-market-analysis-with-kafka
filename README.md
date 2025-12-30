# 📈 Stock Market Analysis with Kafka

## 📌 Overview
This project demonstrates an **end-to-end real-time data engineering pipeline** for stock market data using **Apache Kafka** and **AWS cloud services**.

The system simulates stock market data, streams it through Kafka, stores it in **Amazon S3**, catalogs metadata using **AWS Glue**, and enables analytical queries via **Amazon Athena**.

The main focus of this project is **data ingestion, streaming, storage, and analytics**, rather than predictive modeling.

---

## 🏗️ Architecture
<img src="docs/Architecture.jpg" alt="System Architecture" width="800"/>

### Pipeline Flow
1. Stock market data is simulated using Python.
2. Data is published to Kafka topics via a Kafka producer.
3. Kafka consumers process streaming data and store it in Amazon S3.
4. AWS Glue Crawlers create metadata tables.
5. Amazon Athena is used to query and analyze the data using SQL.

---

## 🛠️ Technology Stack

### Programming Language
- **Python**

### Streaming & Messaging
- **Apache Kafka**

### Cloud Platform (AWS)
- **EC2** – Kafka deployment  
- **Amazon S3** – Data storage  
- **AWS Glue** – Data catalog & crawler  
- **Amazon Athena** – SQL-based analytics  

### Query Language
- **SQL**

---

## 📂 Project Structure
```bash
stock-market-analysis-with-kafka/
│
├── data/           # Dataset used for simulation
├── scripts/        # Kafka producer & consumer scripts
├── docs/           # Architecture diagram and documentation
├── README.md
└── LICENSE
