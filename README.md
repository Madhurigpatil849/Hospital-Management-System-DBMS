# Hospital-Management-System-DBMS
# 🏥 Hospital Management System (DBMS Project)

## 📖 Overview
The **Hospital Management System (HMS)** is a **database-driven project** designed to streamline the **administrative, medical, legal, and financial** aspects of a healthcare institution.  
It facilitates **efficient handling of patient records, OPD, birth records, billing, staff management, and inventory**, ensuring faster workflows, accurate data, and better healthcare delivery.  

---

## 🚀 Project Highlights
🔍 Centralized **Patient Record Management**  
👶 **Birth Record Management** with legal compliance  
💊 **OPD & Diagnostics**: Track visits, diagnoses, prescriptions, and lab reports  
💳 **Billing & Finance Automation** for OPD and in-patient services  
📦 **Inventory Management** of medicines, drugs, and hospital supplies  
👨‍⚕️ **Doctor & Staff Scheduling** for efficient operations  
📈 **SQL Queries**: CRUD, Joins, Views, Aggregates, Grouping, Indexes  

---

## 🎯 Objectives
- Automate **birth record registration** and ensure compliance with legal standards  
- Manage **OPD records** efficiently for fast access to medical history  
- Enhance **patient experience** with reduced wait times and secure record handling  
- Provide **analytics** for hospital trends and operational efficiency  
- Secure sensitive medical data with **encryption and role-based access**  

---

## ⚡ Problem Statement
Hospitals relying on manual or outdated systems face:  
- ❌ Data inaccuracies & inefficiency in workflows  
- ❌ Delay in patient care and compliance with legal documentation  
- ❌ Loss or damage of physical records  
- ❌ Security & privacy risks for sensitive patient data  

✅ The **HMS project** provides a **centralized digital solution** to ensure **accuracy, efficiency, and secure management** of hospital records.  

---

## 🛠️ Technologies Used
- **Database:** MySQL  
- **SQL Concepts:** DDL, DML, Joins, Views, Aggregates, Indexes  
- **Diagrams:** ER Diagram, Schema Diagram  
- **Tools:** MySQL Workbench / Draw.io  

---

## 🧩 System Design
### 🔹 ER Diagram  
### 🔹 Schema Diagram  

---

## 🗄️ Database Structure
Tables implemented in HMS:  
- Patient  
- Doctor  
- Birth Record  
- OPD Records  
- Medicines  
- Appointment  
- Bills  

---

## 🧠 Sample SQL Queries 

### 🔹 Basic Commands  
```sql
CREATE TABLE BirthRecords (...);
INSERT INTO BirthRecords VALUES (...);
SELECT * FROM Appointment WHERE doctor_id = 2;
ALTER TABLE BirthRecords DROP COLUMN baby_name;

🔹 Modifying Commands
DELETE FROM OPDRecords WHERE diagnosis = 'Influenza';
UPDATE Patient SET contact_no='9876543210' WHERE patient_id=1;
ALTER TABLE Patient ADD bloodgroup VARCHAR(5);
ALTER TABLE Doctor RENAME COLUMN name TO doctor_name;

🔹 Conditions & Aggregates
SELECT * FROM Patient WHERE birth_date BETWEEN '1990-01-01' AND '1995-12-31';
SELECT gender, AVG(weight) FROM BirthRecords GROUP BY gender;
SELECT SUM(amount) FROM Bills;

🔹 Joins & Views
SELECT p.patient_name, b.birth_date 
FROM Patient p INNER JOIN BirthRecords b ON p.patient_id=b.patient_id;

CREATE VIEW PatientBirth AS 
SELECT p.patient_name, b.birth_date FROM Patient p JOIN BirthRecords b;

🔹 Index
CREATE INDEX idx_patient_name ON Patient(patient_name);

📊 Advantages
✅ Improved efficiency & reduced paperwork
✅ Centralized and secure database
✅ Faster record retrieval for doctors & staff
✅ Cost savings via automation
✅ Enhanced patient care & hospital coordination

⚠️ Disadvantages
⚠️ High initial cost of setup & training
⚠️ Risk of technical issues/downtime
⚠️ Data breach risks without strong security
⚠️ Ongoing maintenance costs

🔮 Future Scope
Web/Mobile app integration for real-time access

Cloud deployment for scalability

Role-based authentication for better data security

Advanced dashboards for patient trends & hospital analytics

Integration with labs & pharmacies

👩‍💻 Team Members
47 – Madhuri G. Patil

49 – Durva P. Patkar

57 – Vaishnavi Rawate

Guided by: Mrs. Kumud Wasnik

📚 References
ResearchGate – HMS Project

Scribd – HMS Report

Slideshare – HMS Project

