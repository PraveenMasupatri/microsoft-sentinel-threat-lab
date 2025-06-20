# microsoft-sentinel-threat-labs
Practical lab project leveraging Microsoft Sentinel to explore threat intelligence, detection, and incident response.

# Microsoft Azure Sentinel Lab

This project demonstrates a hands-on lab environment for learning and exploring Microsoft Azure Sentinel—a cloud-native Security Information and Event Management (SIEM) and Security Orchestration Automated Response (SOAR) solution. The lab simulates real-world detection and response scenarios using pre-recorded data and built-in artifacts.

---

## 🚀 Lab Objectives

- Deploy Azure Sentinel components in a structured and secure environment.
- Simulate threat detection use cases using pre-recorded datasets.
- Explore built-in Microsoft Sentinel features including analytics rules, workbooks, and hunting queries.
- Understand role-based access control (RBAC) specific to Sentinel roles.

---

## 🏗️ Lab Setup Overview

### 1. **Resource Group and Workspace Deployment**
- Create a new **Azure Resource Group** for the lab.
- Deploy a **Log Analytics Workspace** within the same resource group.
- Enable **Microsoft Sentinel** on the deployed workspace.

### 2. **Install Microsoft Sentinel Training Lab Solution**
- Navigate to the **Content Hub** in Azure Sentinel.
- Install the **Microsoft Sentinel Training Lab** solution.
- This solution ingests pre-recorded logs and enables multiple artifacts (analytics rules, hunting queries, workbooks) to simulate detection and response scenarios.

### 3. **RBAC Role Assignments**
- Assign users to Azure Sentinel-specific roles:
  - **Sentinel Responder** – Can view incidents and take action (e.g., assign, close, comment).
  - **Sentinel Contributor** – Can manage content such as analytics rules and workbooks.

---

## 🧰 Tools & Technologies Used

- **Microsoft Azure**
- **Azure Resource Manager (ARM)**
- **Azure Log Analytics**
- **Microsoft Sentinel**
- **Azure Role-Based Access Control (RBAC)**

---

## 📸 Screenshots (Optional)

_Add screenshots of key steps like Sentinel deployment, Content Hub solution installation, or incidents dashboard._

---

## 📚 Learning Outcomes

- Practical understanding of deploying and managing Microsoft Sentinel.
- Hands-on experience with simulated detection data and investigation workflows.
- Familiarity with Azure security roles and permissions.

---
