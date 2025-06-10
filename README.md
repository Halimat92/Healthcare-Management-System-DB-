

## 🏥 Healthcare Patient Record Management System (SQL Project)

### 📌 Project Summary

This project involves the creation, transformation, and advanced querying of a **relational healthcare database** designed to manage patient data, medical history, treatments, and analytical insights. The system simulates operations commonly required in healthcare record systems—supporting patient care tracking, financial management, demographic analysis, and automated monitoring.

---

### 🎯 Objectives

* Build and normalize a **multi-table SQL database** for healthcare data.
* Perform **data cleaning, transformation**, and schema optimization.
* Create **views, stored procedures, functions**, and **triggers** to enhance automation, integrity, and business logic.
* Enable **data analysis** to identify trends in treatment, cost, and patient outcomes.

---

### 🗂️ Key Features & Components

#### 🔧 Data Engineering

* **Created and normalized tables**: Patients, Conditions, Medications, Allergies, Procedures, Careplans, Immunization, Observation.
* **Data cleaning & transformation**: Used `STR_TO_DATE`, renamed columns, removed invalid fields, and enforced **referential integrity** via foreign keys.

#### 📊 Views & Queries

* `Medical_Records` view: A consolidated view combining patient info, diagnoses, treatments, and medications.
* Analysis queries:

  * Top 5 longest hospital stays.
  * Patients with chronic conditions (ongoing care).
  * Most persistent allergies.
  * Patients with highest medical expenses.
  * Average expenses by medical condition.

#### ⚙️ Stored Procedures & Functions

* `Patient_info_with_Conditions`: Returns full medical history for a specific patient ID.
* `PatientsByRace`: Retrieves patient demographics by race.
* `CalculateMinTimeInHospital`, `CalculateMaxTimeInHospital`: Custom time-based insights.
* `Balance()`: Calculates outstanding medical bills dynamically based on coverage.

#### 🧠 Event & Trigger Automation

* **Event Scheduler**: Logs daily patient reminders into a monitoring table.
* **Trigger**: Automatically deletes immunization data when a patient is removed (data privacy compliance simulation).

---

### 🛠️ Tools & Technologies

* **SQL (MySQL dialect)**
* **Stored Procedures, Functions, Triggers**
* **Automated Events**
* **Relational database design and normalization**

---

### ✅ Future Improvements

* Add user authentication and audit logging.
* Visualize insights via Streamlit or Power BI dashboard.
* Incorporate NLP models for auto-tagging patient complaints and symptoms.
* Add anomaly detection for suspicious billing activity.



