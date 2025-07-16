# Microsoft Azure Sentinel Lab

This project demonstrates a hands-on lab environment for learning and exploring Microsoft Azure Sentinel—a cloud-native Security Information and Event Management (SIEM) and Security Orchestration Automated Response (SOAR) solution and also explore threat intelligence, detection, and incident response. The lab simulates real-world detection and response scenarios using pre-recorded data and built-in artifacts.

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

### 4. **Connect Azure Activity Logs**
- Open the **Data Connectors** section in Sentinel.
- Locate and install the **Azure Activity Connector**.
- Configure the connector to pull activity logs (such as resource modifications and role assignments) from your Azure tenant.
- Confirm successful ingestion by checking the connector status and querying incoming logs.

### 5. **Threat Intelligence Integration (TAXII - Pulsedive)**
- To enrich Sentinel with real-world threat intelligence, we connected the **Threat Intelligence - TAXII data connector**.
- Used **Pulsedive**, a free and community-driven threat intelligence platform that supports TAXII.
- Configured the connector by:
  - Enabling TAXII under **Data Connectors**
  - Providing the Pulsedive TAXII server URL and collection
  - Setting up basic authentication (if required)
- Once connected, Pulsedive’s indicators of compromise (IOCs) began flowing into Sentinel’s **ThreatIntelligenceIndicator** table.
- These IOCs could then be used in:
  - **Analytics rules**
  - **Hunting queries**
  - **Incident correlation**

---
## 🔍 Features Demonstrated

- Deployment of Sentinel and core infrastructure
- Installation of Microsoft Sentinel Training Lab solution
- Role-based access with Sentinel Contributor and Responder roles
- Integration of Azure Activity logs via native data connector
- **Threat Intelligence ingestion using TAXII (Pulsedive) connector**
- Querying and investigating security events using KQL

## 🧰 Tools & Technologies Used

- **Microsoft Azure**
- **Microsoft Sentinel**
- **Log Analytics**
- **Azure Activity Logs**
- **Azure RBAC**
- **Content Hub**
- **KQL (Kusto Query Language)**
- **Threat Intelligence - TAXII (PulseDive)**

---

## 📸 Screenshots (Optional)

_Add screenshots of key steps like Sentinel deployment, Content Hub solution installation, or incidents dashboard._

---

## 📚 Learning Outcomes

- Practical understanding of deploying and managing Microsoft Sentinel.
- Hands-on experience with simulated detection data and investigation workflows.
- Familiarity with Azure security roles and permissions.

---
