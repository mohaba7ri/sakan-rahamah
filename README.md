# 🏠 Rahmah Housing Charity System for Mothers and Orphans

A management system for **مجمعات مساكن الرحمة الخيرية** (Rahmah Charity Housing Complexes) dedicated to supporting **mothers and their orphan children**.

The system provides end-to-end tools to manage housing complexes, units, mothers, orphans, and staff operations through an integrated dashboard and a dedicated mobile application.

---

## 📚 Table of Contents

1. [Overview](#-overview)  
2. [Key Features](#-key-features)  
3. [System Modules](#-system-modules)  
4. [Tech Stack](#-tech-stack)  
5. [System Architecture](#-system-architecture)  
6. [Screenshots & UI Preview](#-screenshots--ui-preview)  
7. [Installation & Setup](#-installation--setup)  
8. [Usage Workflow](#-usage-workflow)  
9. [Folder Structure](#-folder-structure)  
10. [Roadmap](#-roadmap)  
11. [Contributing](#-contributing)  
12. [License](#-license)  
13. [Contact](#-contact)  

---

## 📌 Overview

The **Rahmah Housing Charity System** is designed to support charity organizations that provide housing and care for **widowed mothers and their orphan children**.

The system helps manage:

- 🏢 Housing complexes and residential units  
- 👩‍👧‍👦 Mothers and orphans profiles and eligibility  
- 🛏️ Housing assignments (allocation and vacating units)  
- 👷 Staff working inside the complexes and their roles  
- 📱 Daily operational tasks through a mobile application  

This project aims to:

- ✅ Reduce manual work and paper-based processes  
- ✅ Improve data accuracy and follow-up  
- ✅ Provide a clear, real-time view of housing occupancy and beneficiary status  

---

## ✨ Key Features

### 🏢 Housing Complex Management
- Register and manage multiple housing complexes  
- Define buildings, floors, and apartment units  
- Track occupancy status for each unit:
  - **Available**
  - **Reserved**
  - **Occupied**
  - **Under maintenance**

### 👩‍👧‍👦 Mothers & Orphans Management
- Create and update detailed profiles for mothers  
- Link each mother with her orphan children  
- Store important social and eligibility data  
- Track the status of each family (e.g., **active**, **pending**, **suspended**)

### 🛏️ Housing Assignment (Allocation)
- Assign families (mother + orphans) to housing units  
- Record move-in and move-out dates  
- Manage waiting lists and priority rules (if applicable)

### 👷 Staff & Roles Management
- Add employees working inside each complex  
- Assign roles and permissions (social worker, supervisor, security, admin, etc.)  
- Track staff responsibilities and tasks

### 📱 Mobile Application
- Dedicated mobile app for staff to:
  - View assigned complexes and apartments  
  - Update visit reports and family follow-ups  
  - Submit requests (maintenance, updates, notes, etc.)

### 📊 Reporting & Monitoring
- Overview of total complexes, families, and orphans  
- Occupancy statistics and available units  
- Activity and status summaries per complex  

---

## 🧰 Tech Stack

**Frontend / Client Applications**

- 🎯 **Flutter**
  - Android mobile app
  - Web admin/dashboard
  - Desktop support (Windows / others if needed)

**Backend**

- 🐘 **PHP** (REST API layer)
  - Handles business logic (families, complexes, allocations, staff)
  - Authentication & authorization
  - Validation and security

**Database**

- 🗄️ **MySQL / MariaDB**
  - Stores complexes, buildings, units
  - Mothers and orphans data
  - Housing assignments and history
  - Users, roles, and logs

---

## 🏛 System Architecture

> High-level architecture – adjust details to match your actual implementation.

- **Flutter Clients**
  - **Mobile (Android)**: for field staff (social workers, supervisors, etc.)  
  - **Web / Desktop**: for admins and office users (dashboard, reports, configuration)

- **PHP Backend API**
  - RESTful endpoints for:
    - Complexes & housing units  
    - Mothers, orphans, families  
    - Housing allocations & status changes  
    - Staff users and permissions  
  - Authentication (e.g., token-based)  
  - Role-based access control

- **MySQL Database**
  - Centralized data storage  
  - Relational schema with foreign keys and constraints  

**Typical flow:**

1. A user (admin or staff) interacts with the **Flutter app** (mobile / web / desktop).  
2. The app sends a request to the **PHP API**.  
3. The API validates input, executes business rules, and interacts with **MySQL**.  
4. The result is returned to the client and displayed in the UI (lists, forms, dashboards).  

---

## 🖼 Screenshots & UI Preview

> All images are displayed with rounded corners using HTML so they look nicer in the README.

### 1️⃣ System Dashboard

<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/f9aaa9e1-7e26-43f7-a48f-95c5b73ce453" 
    alt="System Dashboard" 
    style="border-radius: 16px; max-width: 100%; height: auto;" 
  />
</p>

---

### 2️⃣ Housing Screen

<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/489361f6-41f1-4e31-a317-3cabeeba61ff" 
    alt="Housing Screen" 
    style="border-radius: 16px; max-width: 100%; height: auto;" 
  />
</p>

---

### 3️⃣ Family Profile (Mother & Orphans)

<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/ffa9cefb-ec06-4fbb-b72c-1eb14ccf7336" 
    alt="Family Profile - Mother and Orphans - Overview" 
    style="border-radius: 16px; max-width: 100%; height: auto;" 
  />
</p>

<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/840b6994-8c4c-4b48-bc5f-22ff1158994e" 
    alt="Family Profile - Mother and Orphans - Details" 
    style="border-radius: 16px; max-width: 100%; height: auto;" 
  />
</p>

---

### 4️⃣ Mobile App – Staff Home

<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/43deed59-a09b-4e9d-a837-14485c9870e1" 
    alt="Mobile App - Staff Home Screen" 
    style="border-radius: 24px; max-width: 280px; height: auto;" 
  />
</p>

<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/8d985fdb-47c1-4b0d-bc47-d36ad1624538" 
    alt="Mobile App - Staff Tasks / Details" 
    style="border-radius: 24px; max-width: 280px; height: auto;" 
  />
</p>

