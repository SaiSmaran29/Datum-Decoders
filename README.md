# 🏥 CareFlow – Patient-Centric Clinical Workflow System

CareFlow is a workflow-driven clinical coordination platform that enables real-time task routing, status tracking, and interdepartmental visibility across hospital units. The system structures clinical operations around a single longitudinal patient record and a live, event-driven care timeline.

🔗 **Live Application:** [https://careflowmed.netlify.app/]

---

## 🔁 System Execution Flow

Clinical Input → Action Creation → Workflow Processing → Department Queue → Status Update → Timeline Event → Live Dashboard Sync

---

## 🧠 System Overview

CareFlow functions as a workflow orchestration layer between hospital departments. Instead of isolated communication channels, all clinical activities are modeled as structured workflow entities and tracked through lifecycle states.

The platform emphasizes:

- Patient-centric data organization  
- Event-driven updates  
- Role-based operational dashboards  
- Cross-department task visibility  

---

## 🏗 Technical Architecture

CareFlow follows a three-tier architecture.

### 1️⃣ Presentation Layer (Frontend)

Role-based dashboards that provide:

- Authentication (Login / Signup)  
- Patient record interface  
- Care timeline visualization  
- Department task panels  
- Action creation and task controls  

**Responsibilities**
- User interaction handling  
- Real-time state display  
- Dashboard rendering  

---

### 2️⃣ Application Layer (Backend Workflow Engine)

Core system logic responsible for:

- Clinical action creation and validation  
- Workflow state transitions  
- Timeline event generation  
- Role-based access control enforcement  
- Update propagation across users  

This layer ensures that when a task status changes, the update is reflected across all relevant stakeholders.

---

### 3️⃣ Data Layer (Centralized Storage)

Persistent storage for:

- Patient entities  
- Users and roles  
- Clinical actions  
- Timeline event logs  
- Attachments and notes  

The database acts as the single source of truth for patient workflow state.

---

## 🧩 Core System Modules

### 🔐 Authentication & Authorization
- Role-Based Access Control (RBAC)  
- Segmented dashboard access  
- Protected patient data views  

### 🧾 Patient Record Module
Maintains:

- Demographics  
- Diagnoses  
- Allergies  
- Current medications  

Serves as the root entity for all clinical workflow actions.

---

### 🔁 Clinical Action Workflow Engine

All hospital operations are represented as structured clinical actions with defined attributes such as type, department, priority, and status.

**Lifecycle States**

Ordered → Acknowledged → In Progress → Completed / Cancelled

---

### ⏳ Care Timeline Module

A chronological activity stream that records:

- Status changes  
- Department updates  
- Clinical notes  
- Action completions  

Provides full visibility into patient care progression.

---

### 🏢 Department Queue System

Dynamic task views filtered by:

- User role  
- Department  
- Action status  

Acts as the operational workspace for clinical units.

---

### 🔄 Real-Time Synchronization

Whenever a clinical action is updated:

1. System state is updated  
2. Timeline event is generated  
3. Dashboards reflect changes  
4. All relevant users see updated patient status  

---

## 👥 Supported Roles

| Role | System Interaction |
|------|--------------------|
| Doctor | Creates and reviews clinical actions |
| Nurse | Executes care tasks |
| Pharmacy | Processes medication workflows |
| Lab / Imaging | Handles diagnostic requests |
| Admin | Monitors system-wide operations |

---
## Authorization Page
![login page](https://github.com/SaiSmaran29/Datum-Decoders/blob/main/Screenshot%202026-02-12%20121150.png)
![Sign up Page](https://github.com/SaiSmaran29/Datum-Decoders/blob/main/Screenshot%202026-02-12%20121210.png)
## 📸 Dashboard Preview

![CareFlow Dashboard](https://github.com/SaiSmaran29/Datum-Decoders/blob/main/Screenshot%202026-02-12%20120242.png)

## ⏳ Application Interface
![api](https://github.com/SaiSmaran29/Datum-Decoders/blob/main/Screenshot%202026-02-12%20121130.png)


## 🧪 Example Workflow

**Lab Test Execution**

Doctor creates lab test → Lab receives task → Lab marks completion → Timeline updates → Doctor dashboard reflects result

---

## 🔐 Security Model

- Role-based access enforcement  
- Segregated departmental task views  
- Action-level audit tracking  
- Controlled patient record visibility  

---

## 🚀 Future Technical Extensions

- EHR system integration  
- AI-driven task prioritization  
- Predictive clinical alerts  
- IoT-based patient monitoring  

---

## 🏁 Summary

CareFlow implements a workflow-oriented coordination architecture that transforms hospital operations from siloed communication into structured, real-time, patient-centric task orchestration.

