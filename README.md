# Enterprise Revenue Analytics Pipeline (IDP + SQL)

## 📌 Project Overview
This project simulates an automated enterprise data engineering and analytics workflow. It extracts unorganized, messy transaction logs from a payment gateway, structures them into a relational SQL database, and prepares them for business intelligence reporting.

## 🛠️ Tech Stack & Skills
* **Intelligent Document Processing (IDP)**: Advanced GenAI prompting (Gemini) for data extraction and text standardization.
* **Database Engineering**: SQL (DDL/DML), Relational Architecture (Fact/Dimension tables), Foreign Key Constraints.
* **Analytics & Insights**: Multi-table Joins, Aggregations (`SUM`, `GROUP BY`), Data Sorting (`ORDER BY`).

## 🔄 Data Workflow Pipeline

### Phase 1: AI-Augmented Extraction
Raw, unstructured logs are parsed using structured prompt engineering to filter out failed attempts, clean text casing, and output clean CSV data.

### Phase 2: Relational Database Schema
Data is split into a Star Schema structure to ensure zero redundancy:
* `CUSTOMERS_DIM`: Customer profile data (Primary Key: `Customer_ID`)
* `TRANSACTION_FACT`: Sales transaction logs (Foreign Key: `Customer_ID`)

### Phase 3: Analytical Insights
The pipeline executes an optimized join query to deliver instant geographic revenue summaries for executive decision-making.

