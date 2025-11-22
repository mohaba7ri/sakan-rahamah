# Rahmah Housing Charity System for Mothers and Orphans

A management system for **مجمعات مساكن الرحمة الخيرية** (Rahmah Charity Housing Complexes) dedicated to supporting **mothers and their orphan children**.  
The system provides end-to-end tools to manage housing complexes, units, mothers, orphans, and staff operations through an integrated dashboard and a dedicated mobile application.

---

## Table of Contents

1. [Overview](#overview)  
2. [Key Features](#key-features)  
3. [System Modules](#system-modules)  
4. [System Architecture](#system-architecture)  
5. [Screenshots & UI Preview](#screenshots--ui-preview)  
6. [Installation & Setup](#installation--setup)  
7. [Usage Workflow](#usage-workflow)  
8. [Folder Structure](#folder-structure)  
9. [Roadmap](#roadmap)  
10. [Contributing](#contributing)  
11. [License](#license)  
12. [Contact](#contact)  

---

## Overview

The **Rahmah Housing Charity System** is designed to support charity organizations that provide housing and care for **widowed mothers and their orphan children**.

The system helps manage:

- Housing complexes and residential units  
- Mothers and orphans profiles and eligibility  
- Housing assignments (allocation and vacating units)  
- Staff working inside the complexes and their roles  
- Daily operational tasks through a mobile application  

This project aims to:

- Reduce manual work and paper-based processes  
- Improve data accuracy and follow-up  
- Provide a clear, real-time view of housing occupancy and beneficiary status  

---

## Key Features

- **Housing Complex Management**
  - Register and manage multiple housing complexes
  - Define buildings, floors, and apartment units
  - Track occupancy status for each unit (available, reserved, occupied, under maintenance)

- **Mothers & Orphans Management**
  - Create and update detailed profiles for mothers
  - Link each mother with her orphan children
  - Store important social and eligibility data
  - Track the status of each family (active, pending, suspended, etc.)

- **Housing Assignment (Allocation)**
  - Assign families (mother + orphans) to housing units
  - Record move-in and move-out dates
  - Manage waiting lists and priority rules (if applicable)

- **Staff & Roles Management**
  - Add employees working inside each complex
  - Assign roles and permissions (e.g., social worker, supervisor, security, admin)
  - Track staff responsibilities and tasks

- **Mobile Application**
  - Dedicated mobile app for staff to:
    - View assigned complexes and apartments
    - Update visit reports and family follow-ups
    - Submit requests (maintenance, updates, notes, etc.)

- **Reporting & Monitoring**
  - Overview of total complexes, families, and orphans
  - Occupancy statistics and available units
  - Activity and status summaries per complex

---

## System Modules

1. **Admin Panel**
   - Manage complexes, units, families, and users
   - Configure system settings and access control  

2. **Beneficiary Management**
   - Mothers and orphan children profiles  
   - Eligibility and status tracking  

3. **Housing & Allocation**
   - Apartment/unit registry  
   - Assignment and move-in/out management  

4. **Operations & Staff**
   - Users, roles, and permissions  
   - Staff assignment to complexes  

5. **Mobile Application**
   - On-ground operational tool for staff  
   - Visit reports, follow-up notes, and real-time updates  

---

## System Architecture

> Adjust this section according to your actual stack (e.g. Flutter, PHP, MySQL, Firebase…).

- **Frontend / Mobile App**
  - Cross-platform mobile application (Android / iOS)
  - Staff can access only the complexes and tasks assigned to them

- **Backend API**
  - RESTful API for managing data (complexes, families, assignments, users)
  - Authentication and role-based access control

- **Database**
  - Central database for all entities (complexes, mothers, orphans, staff, housing units, logs)

- **Integration**
  - Possible integration with external services (notifications, SMS, email, etc.)

---

## Screenshots & UI Preview

### 1. System Dashboard

![Main Dashboard](docs/images/dashboard.png)
<img width="1918" height="1139" alt="image" src="https://github.com/user-attachments/assets/f9aaa9e1-7e26-43f7-a48f-95c5b73ce453" />


### 2. Housing Screen

<img width="1900" height="812" alt="image" src="https://github.com/user-attachments/assets/489361f6-41f1-4e31-a317-3cabeeba61ff" />


### 3. Family Profile (Mother & Orphans)

<img width="1919" height="1125" alt="Screenshot 2025-11-22 165502" src="https://github.com/user-attachments/assets/ffa9cefb-ec06-4fbb-b72c-1eb14ccf7336" />
<img width="1919" height="941" alt="image" src="https://github.com/user-attachments/assets/840b6994-8c4c-4b48-bc5f-22ff1158994e" />



### 4. Mobile App – Staff Home

<img width="559" height="1102" alt="image" src="https://github.com/user-attachments/assets/43deed59-a09b-4e9d-a837-14485c9870e1" />

<img width="562" height="1112" alt="image" src="https://github.com/user-attachments/assets/8d985fdb-47c1-4b0d-bc47-d36ad1624538" />



> Tip: You can add more subsections for each important flow and upload images accordingly.

---

## Installation & Setup

> Adjust the steps to match your actual technology stack.

### Prerequisites

- Backend:
  - Web server (e.g., Apache)
  - Programming language runtime (e.g., PHP)
  - Database (e.g., MySQL)

- Mobile App:
  - Flutter
  - Android Studio 

