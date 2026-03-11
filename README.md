# MPSTOK
# MP STOK: Hospital Warehouse & Inventory Tracking System

> **Note:** The source code for this project is proprietary and closed-source as it is an active commercial product deployed in a large-scale private hospital. This repository serves to document the system architecture, engineering decisions, and algorithmic implementations.

## 📌 System Overview
MP STOK is a comprehensive inventory management system designed to handle the high-throughput, mission-critical supply chain of a private healthcare facility. It transitions legacy manual tracking into a centralized, automated digital infrastructure, ensuring real-time stock visibility and preventing critical medical supply shortages.



## 🛠️ Technology Stack & Architecture
* **Language:** C#
* **Framework:** .NET (Windows Presentation Foundation / Windows Forms)
* **Database:** Relational Database Management System (SQL)
* **Architecture Pattern:** Client-Server Architecture with Layered Design (UI, Business Logic, Data Access)

## ⚙️ Core Engineering Features

### 1. Concurrency and Transaction Management
Handling simultaneous inventory requests from different hospital departments (e.g., ER, Surgery, Wards) without race conditions. Implemented strict database transaction protocols to ensure data integrity during parallel stock deductions.

### 2. Algorithmic Stock Optimization
* **Low-Stock Alerting:** Developed an automated threshold algorithm that calculates consumption rates and triggers warnings before critical medical supplies run out.
* **Search & Filter Algorithms:** Optimized querying mechanisms to instantly filter through thousands of inventory items based on custom parameters (expiration date, batch number, department allocation).

### 3. Role-Based Access Control (RBAC)
Engineered a secure authentication system segregating user privileges. Administrative staff have full CRUD (Create, Read, Update, Delete) access, while standard users (nurses, technicians) operate under restricted view/consume permissions.

## 📈 Impact & Deployment
* Successfully replaced manual Excel-based tracking with a robust relational database model.
* Currently deployed and actively maintained in a high-demand hospital environment, managing continuous daily operations.
* Reduced human error in stock counts and optimized the procurement cycle through automated reporting.
