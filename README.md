# 🏥 Healthcare Patient Outcomes Analysis (MySQL)

## 📌 Project Overview

This project focuses on analyzing healthcare data using **MySQL** to understand patient diagnoses and treatment outcomes. The objective is to demonstrate strong SQL fundamentals, relational database design, and analytical querying skills relevant to a **Data Analyst role**.

---

## 🎯 Objectives

* Analyze patient health outcomes based on different diagnoses
* Practice real-world SQL queries used in healthcare analytics
* Extract meaningful insights using structured healthcare data

---

## 🗂️ Database Structure

The project uses a relational database with the following tables:

* **Patients** – Stores patient demographic details
* **Diagnoses** – Contains diagnosis information
* **Outcomes** – Records treatment outcomes for patients

Relationships are established using **primary and foreign keys** to maintain data integrity.

---

## 🛠️ Tools & Technologies

* **Database:** MySQL
* **Language:** SQL
* **Environment:** MySQL Workbench

---

## 🔍 Key SQL Concepts Used

* INNER JOIN
* GROUP BY
* WHERE clause
* ORDER BY
* Aggregate functions (COUNT)
* Data filtering and sorting

---

## 📊 Analysis Performed

* Diagnosis-wise patient count
* Outcome-wise distribution of patients
* Diagnosis vs Outcome analysis
* Identification of trends in treatment outcomes

---

## 📈 Sample Query Example

```sql
SELECT d.diagnosisname, o.outcomename, COUNT(*) AS outcomecount
FROM patients p
JOIN diagnoses d ON p.diagnosisid = d.diagnosisid
JOIN outcomes o ON p.outcomeid = o.outcomeid
GROUP BY d.diagnosisname, o.outcomename;
```

---

## 💡 Insights

* Helps identify which diagnoses have better or worse outcomes
* Supports data-driven decision-making in healthcare management
* Demonstrates real-world analytical SQL problem-solving

---

## 🚀 How to Run the Project

1. Install MySQL and MySQL Workbench
2. Import the provided `.sql` file into MySQL
3. Execute the queries to view analytical results


