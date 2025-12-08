<div align="center">

# **PAYROLL SYSTEM**  
### **for The Visa Center (Dizon Immigration Services)**  
#### *A Web-Based Payroll Records and Management Platform*

---

## 👩‍💻 **Developed By**

<table>
  <tr>
    <td align="center"><strong>Chelsea</strong></td>
    <td align="center"><strong>Ashlee</strong></td>
    <td align="center"><strong>Joane</strong></td>
    <td align="center"><strong>Sophia</strong></td>
  </tr>
</table>

*BSIT Students — Database Systems 1 Project*  
**Advisers:** Kent Vincent Sarsalejo and Keana Cerela Giron 

</div>

---

## 📌 Project Overview
The payroll process at the newly established **Davao City branch of The Visa Center (Dizon Immigration Services)** is currently performed manually using Microsoft Excel. While spreadsheets offer basic organization, they lack **automation, scalability, and accuracy**, especially as employee data grows.

This system aims to provide an **automated, secure, and centralized payroll management platform** that reduces human errors, speeds up data processing, and supports future company expansion.

---

## 🎯 Project Goals
- Replace manual Excel-based payroll handling  
- Automate salary computations and deductions  
- Minimize human error and duplicate records  
- Improve HR productivity and data processing  
- Ensure secure, centralized payroll storage  
- Support system scalability as the company expands  

---

# 🛠 Technology Stack

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.11+-blue" />
  <img src="https://img.shields.io/badge/Flask-3.1.2+-orange" />
  <img src="https://img.shields.io/badge/SQLite-Development-lightgrey" />
  <img src="https://img.shields.io/badge/PostgreSQL-Production-blueviolet" />
  <img src="https://img.shields.io/badge/MySQL-Production-blue" />
  <img src="https://img.shields.io/badge/Frontend-HTML%2FCSS%2FJavaScript-yellow" />
</p>

---

# 🧩 System Overview

| Component                | Technology                         | Hosting            | Description |
|-------------------------|-------------------------------------|--------------------|-------------|
| **Frontend**            | HTML, CSS, JavaScript               | Firewall / Local   | Handles UI, dashboards, employee forms |
| **Authentication**      | Flask / Backend Auth                | Local Server       | Manages secure login and role access |
| **Database**            | SQLite / PostgreSQL / MySQL         | Local / Firewall   | Stores payroll data, attendance, and employee info |
| **Backend / Automation**| Flask                              | Local Server       | Automates deductions, salary computation, and report generation |
| **Storage (Optional)**  | Local File Storage                  | Local Server       | Stores payslips, reports, and exported files |

---

# ⚙️ Core Features (Workflow-Based)

### **1. Initial Setup**
- Install system → Create first admin user → Login as admin  

### **2. Employee Onboarding (HR)**
- Add employee → System creates user account + employee record  
- Auto-creates leave balances (Vacation, Sick, Personal)  
- Set work schedule (start/end times, hours per day)  
- Set leave entitlements  

### **3. Daily Operations**
- Employee clocks in/out → Creates attendance log  
- HR can manually log attendance if needed  
- HR manages holidays (affects payroll calculations)  

### **4. Leave Management**
- Employee files leave request → Status: Pending  
- HR approves/rejects → System auto-calculates working days  
- Database triggers deduct leave balance if approved  
- Excludes weekends and holidays automatically  

### **5. Payroll Processing (Monthly)**
- HR runs payroll → Enters pay period dates  
- System calculates each active employee:  
  - Time & Attendance: Regular hours, Overtime, Late minutes  
  - Base salary (prorated if < 160 hours)  
  - Overtime pay (1.25× rate)  
  - Statutory deductions (SSS, PhilHealth, Pag-IBIG)  
  - Withholding tax (BIR TRAIN Law)  
  - Net pay  
- Creates payslip for each employee  
- HR reviews summary → Employees can view payslips  

### **6. Employee Self-Service**
- View dashboard (clock status, leave balances)  
- Clock in/out  
- View payslips  
- File leave requests  
- View leave history  

---

# ⭐ Additional System Features
- Automatic leave balance management via database triggers  
- Working days calculation excludes weekends & holidays  
- Payroll calculations include T&A integration  
- Audit logging for all admin actions  
- Role-based access control (Admin, Payroll_Admin, Employee)  
- Complete workflow document saved as **WORKFLOW.md**  

---

# 📌 Conclusion
This Web-Based Payroll System modernizes the payroll operations of the **Davao City branch of The Visa Center (Dizon Immigration Services)**. By replacing manual spreadsheets with an automated and secure system, it enhances accuracy, reduces processing time, and improves HR efficiency.

Built with **Python 3.11+, Flask 3.1.2+, SQLite (development) or PostgreSQL/MySQL (production), HTML, CSS, and JavaScript**, the system ensures a **secure, scalable, and efficient payroll workflow**.
