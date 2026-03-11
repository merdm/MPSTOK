# MP STOK: Secure Desktop Inventory Management System

> **Note:** The source code for this project is closed-source as it is an active commercial product deployed in a private hospital. This repository documents the software architecture, module design, and business logic.

##  System Overview
MP STOK is a standalone Windows desktop application (`.exe`) designed for the isolated, high-security environment of a private healthcare facility. It operates entirely offline (local network/machine) to ensure zero dependency on external internet connections, maximizing data privacy and system reliability for critical hospital inventory.



##  Technology Stack & Architecture
* **Platform:** Windows Desktop Application (Executable)
* **Language:** C# (.NET Framework)
* **Database:** Local/Intranet Relational Database (e.g., SQLite / MS SQL LocalDB)
* **Architecture:** Monolithic Desktop Architecture with isolated UI and Data layers.

##  Core Modules & Interface Design

### 1. Dashboard (Ana Sayfa)
* Provides an at-a-glance overview of critical inventory metrics.
* Highlights low-stock alerts and recent warehouse activities to ensure immediate operational awareness.

### 2. Product Operations (Ürün İşlemleri)
* The core CRUD (Create, Read, Update, Delete) module for inventory management.
* Handles secure data entry for new medical supplies, stock deduction during consumption, and batch/expiration date tracking without race conditions.

### 3. Reporting (Raporlama)
* An automated data extraction module replacing manual Excel sheets.
* Generates structured reports on consumption rates, historical inventory levels, and procurement needs directly from the local database.

### 4. Settings & Configuration (Ayarlar)
* Role-Based Access Control (RBAC) configuration.
* Allows administrators to manage user profiles, adjust low-stock warning thresholds, and maintain database backup protocols.

## 📈 Impact & Deployment
* Successfully replaced legacy manual tracking with a robust, zero-latency local desktop application.
* Designed to run autonomously without internet access, fully complying with hospital data isolation policies.
