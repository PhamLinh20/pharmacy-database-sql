# 💊 365 Pharmacy Management Database System

> A relational database analysis, schema design, and SQL implementation project developed for a retail pharmaceutical enterprise.

---

## 📌 Project Overview & Objectives
- **Target System:** 365 Pharmacy Management System (Sun Pharma Joint Stock Company)
- **Domain:** Pharmaceutical Retail & Supply Chain Operations
- **System Objectives:**
  - Standardize drug catalog management, batch numbers, stock levels, and expiration dates to prevent expired distribution and stockouts.
  - Streamline point-of-sale dispensing and order processing, linking pharmacists, customers, multi-item prescriptions, and compliant electronic invoices.
  - Establish a robust, normalized database structure to secure transaction integrity and automate historical data maintenance.

---

## 🛠️ Technologies Used
- Microsoft SQL Server (SQL)
---

## 💼 My Personal Contributions

### 1. Database Modeling & Schema Architecture
- Participated in workflow analysis and co-designed the conceptual **Entity-Relationship Diagram (ERD)** across 7 core entities (`Customer`, `Pharmacist`, `Supplier`, `Drug`, `Order`, `OrderDrug`, `Invoice`).
- Derived a **3NF-normalized Relational Schema**, defining primary keys, composite keys, and foreign key relationships to prevent redundancy and update anomalies.

### 2. SQL Implementation & Business Solutions
Directly authored, tested, and executed SQL queries and scripts addressing core business rules:
- **Conditional Stock Verification:** Utilized `CASE WHEN` to evaluate stock levels and enforce safety buffer thresholds before order confirmation.
- **Defensive Data Insertion:** Applied `WHERE NOT EXISTS` clauses to ensure safe product additions without duplicate records or primary key collision errors.
- **Automated Data Retention & Lifecycle:** Formulated queries combining `DATEADD` and `GETDATE` to purge legacy transactional invoices older than two years, maintaining system performance and storage efficiency.

