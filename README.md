# 🛒 Olist E-Commerce Business Intelligence & SQL Analysis

![MySQL](https://img.shields.io/badge/MySQL-8.0-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Domain](https://img.shields.io/badge/Domain-E--Commerce%20%26%20Logistics-orange?style=for-the-badge)
![Dataset](https://img.shields.io/badge/Dataset-Olist%20Kaggle%20(100k%2B)-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

---

## 📌 Executive Summary

This repository contains an end-to-end relational database implementation and business performance analysis on **100,000+ anonymized e-commerce orders** from the Brazilian marketplace **Olist**. 

Using **MySQL Server 8.0**, raw commercial data was engineered into a relational schema to extract actionable insights surrounding **financial growth, customer geography, product portfolio demand, and logistics efficiency**.

---

## 📐 Data Architecture & Schema

The relational database (`ECOMMERCE_DB`) standardizes four core operational tables linked through primary and foreign key constraints:


🛠️ Data Engineering & ETL Highlights
Cross-Platform Compatibility: Replaced default Windows line endings (\r\n) with Unix standards (\n) to prevent dataset truncation errors during high-volume ingestion.

Null Handling Pipeline: Constructed explicit @variable loading conditions via NULLIF(@var, '') to map missing dataset values directly to SQL NULL types without violating strict mode constraints.

Transactional Integrity: Engineered execution blocks with temporary foreign key bypass rules (SET FOREIGN_KEY_CHECKS = 0) to allow high-speed bulk ingestion without constraint lockouts.

📂 Repository Structure
├── data/                      # Raw CSV datasets (Kaggle Olist)
├── scripts/
│   ├── data_import.sql        # Automated table schema creation & ETL load script
│   └── business_analysis.sql  # 5 analytical business queries
├── README.md                  # Project documentation & technical walkthrough


👨‍💻 Author
Syed Ramiq Ali
