# Rahmah Housing Charity System for Mothers and Orphans  
**(نظام مشروع مساكن الرحمة الخيرية للأمهات وأيتامهم)**

A management system for **مجمعات مساكن الرحمة الخيرية** (Rahmah Charity Housing Complexes) dedicated to supporting **mothers and their orphan children**.

The system provides end-to-end tools to manage housing complexes, residential units, mothers, orphans, and staff operations through an integrated **admin dashboard** and a **Flutter-based mobile / web / desktop application**.

---

## Table of Contents

1. [Overview](#overview)  
2. [Key Features](#key-features)  
3. [Tech Stack](#tech-stack)  
4. [System Modules](#system-modules)  
5. [System Architecture](#system-architecture)  
6. [Screenshots & UI Preview](#screenshots--ui-preview)  
7. [Installation & Setup](#installation--setup)  
   - [Backend (PHP + MySQL)](#backend-php--mysql)  
   - [Flutter App (Android / Web / Desktop)](#flutter-app-android--web--desktop)  
8. [Usage Workflow](#usage-workflow)  
9. [Folder Structure](#folder-structure)  
10. [Roadmap](#roadmap)  
11. [Contributing](#contributing)  
12. [License](#license)  
13. [Contact](#contact)  

---

## Overview

The **Rahmah Housing Charity System** is designed for charity organizations that provide housing and care for **widowed mothers and their orphan children**.

The system helps manage:

- Housing complexes and residential units  
- Mothers and orphans profiles and eligibility  
- Housing assignments (allocation and vacating units)  
- Staff working inside the housing complexes and their roles  
- Daily operational tasks through a **Flutter mobile app**  

Main goals:

- Reduce manual and paper-based processes  
- Improve data accuracy and traceability  
- Provide a real-time, clear view of occupancy status and beneficiaries  

---

## Key Features

### Housing Complex Management
- Register and manage multiple housing complexes  
- Define buildings, floors, and apartment units  
- Track unit status: **available**, **reserved**, **occupied**, **under maintenance**  

### Mothers & Orphans Management
- Create and update detailed profiles for mothers  
- Link each mother with her orphan children  
- Store important social, eligibility, and status information  
- Track each family status: **active**, **pending**, **suspended**, etc.  

### Housing Assignment (Allocation)
- Assign families (mother + orphans) to specific units  
- Record **move-in** and **move-out** dates  
- Manage waiting lists and priority rules (if applicable)  

### Staff & Roles Management
- Add employees working inside each housing complex  
- Assign roles and permissions (e.g. social worker, supervisor, security, admin)  
- Track responsibilities and tasks per staff member  

### Mobile / Web / Desktop App (Flutter)
- Built with **Flutter** to support:
  - Android
  - Web
  - Desktop (Windows / others depending on build config)
- Staff can:
  - View assigned complexes and families  
  - Submit visit reports and follow-up notes  
  - Create maintenance or update requests  

### Reporting & Monitoring
- Overview of total complexes, families, mothers, and orphans  
- Occupancy statistics and available units  
- Activity and status summaries per complex  

---

## Tech Stack

**Client Applications (Single Flutter Codebase)**  
- **Flutter**  
  - Android app (APK / AAB)  
  - Web app (deployed as static web)  
  - Desktop app (e.g. Windows build)  

**Backend API**  
- **PHP** (REST-style endpoints)  
  - Business logic for complexes, families, allocations, and users  
  - Authentication & role-based access control  

**Database**  
- **MySQL**  
  - Tables for:
    - Complexes, buildings, floors, units  
    - Mothers, orphans, families  
    - Staff, roles, permissions  
    - Housing allocations, logs, and actions  

You can extend this stack with:
- Nginx / Apache as web server  
- Optional services: email, SMS gateway, or push notifications  

---

## System Modules

1. **Admin Panel**
   - Manage complexes, units, families, and users  
   - Configure system settings and permissions  

2. **Beneficiary Management**
   - Profiles for mothers and orphan children  
   - Eligibility, social data, and status tracking  

3. **Housing & Allocation**
   - Registry of apartments/units per complex  
   - Allocation, move-in, and move-out management  

4. **Operations & Staff**
   - Users, roles, and permissions  
   - Staff assignment to specific complexes  

5. **Flutter App (Mobile / Web / Desktop)**
   - On-ground operational tool for staff  
   - Visit reports, follow-up notes, and real-time updates  

---

## System Architecture

> This is a high-level overview. Adjust details to match your exact implementation.

- **Flutter Client (Android / Web / Desktop)**
  - Communicates with the backend via HTTP/HTTPS  
  - Uses authentication tokens (e.g. JWT / session tokens)  
  - Staff see only the complexes and families assigned to them  

- **PHP Backend**
  - REST-like API endpoints (e.g. `/api/login`, `/api/complexes`, `/api/families`, `/api/allocations`)  
  - Handles authorization, validation, and core business rules  

- **MySQL Database**
  - Centralized database storing:
    - Complex structures (complex → buildings → floors → units)  
    - Mothers, orphans, and family relationships  
    - Allocations, staff, visit logs, and actions  

- **Optional Integrations**
  - Notifications (email/SMS)  
  - External reporting or donor systems  

---

## Screenshots & UI Preview

> The images below are taken from the current version of the system.

### 1. System Dashboard

![Dashboard](https://github.com/user-attachments/assets/f9aaa9e1-7e26-43f7-a48f-95c5b73ce453)

### 2. Housing Screen

![Housing Screen](https://github.com/user-attachments/assets/489361f6-41f1-4e31-a317-3cabeeba61ff)

### 3. Family Profile (Mother & Orphans)

![Family Profile – Header](https://github.com/user-attachments/assets/ffa9cefb-ec06-4fbb-b72c-1eb14ccf7336)

![Family Profile – Details](https://github.com/user-attachments/assets/840b6994-8c4c-4b48-bc5f-22ff1158994e)

### 4. Mobile App – Staff Home

![Staff Home – Complex List](https://github.com/user-attachments/assets/43deed59-a09b-4e9d-a837-14485c9870e1)

![Staff Home – Family List](https://github.com/user-attachments/assets/8d985fdb-47c1-4b0d-bc47-d36ad1624538)



## Installation & Setup

> Adapt the details (paths, URLs, database names) to your environment.

### Backend (PHP + MySQL)

1. **Clone the Repository**

```bash
git clone https://github.com/your-org/rahmah-housing-system.git
cd rahmah-housing-system
