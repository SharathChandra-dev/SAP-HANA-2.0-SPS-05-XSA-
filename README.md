# 🚀 SAP HANA 2.0 SPS 05 (XSA) – Case Study

![SAP HANA](https://img.shields.io/badge/SAP-HANA-blue?style=for-the-badge\&logo=sap)
![XSA](https://img.shields.io/badge/XS_Advanced-XSA-success?style=for-the-badge)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen?style=for-the-badge)
![GitHub](https://img.shields.io/badge/GitHub-Repository-black?style=for-the-badge\&logo=github)

## 📖 Project Overview

This repository contains my implementation of the **SAP HANA 2.0 SPS 05 (XSA) Case Study** provided by **SAP UCC Munich**.

The project demonstrates end-to-end development in **SAP HANA XS Advanced (XSA)** using **SAP Web IDE**, including data modeling, cross-container access, calculation views, star schema modeling, and analytical reporting.

---

## 🎯 Learning Objectives

✅ Understand SAP HANA XSA Architecture
✅ Work with SAP Web IDE Development & Analysis tools
✅ Configure HDI Container access
✅ Build Calculation Views
✅ Implement Star Schema Modeling
✅ Perform Business Analytics on Sales Data

---

## 🛠️ Technologies Used

| Technology             | Description                 |
| ---------------------- | --------------------------- |
| 🔵 SAP HANA 2.0 SPS 05 | In-memory database platform |
| 🌐 SAP Web IDE         | Development environment     |
| 📦 HDI Containers      | Database containerization   |
| 🔐 HDB Grants          | Authorization management    |
| 🔗 HDB Synonyms        | Cross-container access      |
| 📊 Calculation Views   | Data modeling               |
| ⭐ Star Schema          | Analytical modeling         |

---

## 📂 Project Structure

```text
SAP-HANA-2.0-SPS-05-XSA/
│
├── db/
│   ├── src/
│   │   ├── syn/
│   │   │   ├── external.hdbgrants
│   │   │   └── synonym.hdbsynonym
│   │   │
│   │   ├── data/
│   │   │   ├── Salesorg.hdbcds
│   │   │   ├── Salesorg.hdbtabledata
│   │   │   └── Salesorg.csv
│   │   │
│   │   └── views/
│   │       ├── CUSTOMER_DIM_CV
│   │       ├── PRODUCT_DIM_CV
│   │       ├── SALES_CUBE_CV
│   │       └── SALES_RANK_CUBE_CV
│   │
│   └── mta.yaml
│
└── README.md
```

---

## ✅ Implemented Tasks

### 🔐 Task 1: Cross-Container Access

* Created Multi-Target Application (MTA)
* Added Database Module
* Configured SAP HANA Service Connection
* Implemented `.hdbgrants`
* Created `.hdbsynonym`
* Connected to external HDI Container **hdi_GBI_DEMO**

---

### 📄 Task 2: Sales Organization Table

* Created `Salesorg` table
* Imported `Salesorg.csv`
* Configured `.hdbtabledata`

---

### 👥 Task 3: Customer Dimension View

Created **CUSTOMER_DIM_CV** with:

* Customer details
* Country information
* Sales Organization mapping
* Text Joins
* Data filtering

---

### 📦 Task 4: Product Dimension View

Created **PRODUCT_DIM_CV**:

* Included product attributes
* Excluded price field
* Built reusable dimension model

---

### ⭐ Task 5: Sales Cube with Star Join

Created **SALES_CUBE_CV**:

* Fact table: Sales
* Customer Dimension
* Product Dimension
* Star Schema Modeling

#### Calculated Measure

```sql
NET_REVENUE = REVENUE - DISCOUNT
```

---

### 🏆 Task 6: Ranking View

Created **SALES_RANK_CUBE_CV**:

Filters applied:

* 🇩🇪 Country = Germany (DE)
* 📅 Year = 2011
* 📆 Month = May

Generated:

🏅 Top 3 Products by Revenue

---

### 📈 Task 7: Analytics & Reporting

Performed analysis using SAP Web IDE:

✔ Total Revenue in Germany (May 2011)

✔ Top 3 Revenue Generating Products

✔ Interactive Data Preview

---

## 🧠 Key Concepts Learned

* SAP HANA XSA Development
* HDI Container Management
* Cross-Container Access
* Data Modeling
* Calculation Views
* Star Join Implementation
* Business Intelligence & Analytics

---

## 🌟 Highlights

✨ Built enterprise-grade analytical models

✨ Implemented secure HDI access

✨ Designed star schema architecture

✨ Developed reusable calculation views

✨ Performed business analytics on sales data

---

## 👨‍💻 Author

**Sharath Chandra**

🔗 GitHub: https://github.com/SharathChandra-dev

---

## 📜 Acknowledgements

Special thanks to **SAP UCC Munich** for providing the SAP HANA Case Study and learning materials.
