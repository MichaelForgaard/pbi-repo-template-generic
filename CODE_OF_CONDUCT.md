## 📋 Data Governance & Delivery – Code of Conduct (Guidelines)

This document describes the expected standards for anyone working with **Power BI**, **Microsoft Fabric**, or related data products in this repository.
It is **not a task checklist**. The actionable checklist lives as a GitHub Issue Template.

---

### 💼 Business Value & Business Case
All solutions should contribute to documented business value.
- Ensure Power BI reports and Fabric data products support the defined business case.
- Produce insights that help stakeholders make informed decisions.

---

### 📐 Data Modeling, Architecture & Data Products
Build models and data products according to approved architecture principles.
- Power BI models and Fabric tables/lakehouses must follow agreed patterns for governance, quality, and structure.
- Architecture choices should support scalability, performance, maintainability, and reuse.
- Avoid unauthorized "shadow data products" in both Power BI workspaces and Fabric lakehouses.

---

### 📜 Architecture Contract for Fabric Solutions
Use only governed sources and approved architectural components.
- Prefer approved sources in Power BI and Fabric (e.g., OneLake, Delta tables, governed data products).
- Avoid parallel extracts and uncontrolled pipelines.
- Ensure Fabric components have clear ownership and are documented.

---

### 🔒 Security & Classification
Security and classification requirements must always be respected.
- Classify all content according to your organisation's data classification policy.
- Label Power BI datasets, Fabric items, and documentation with the correct classification.
- Never publish restricted or confidential data in areas where unauthorized users may have access.
- Follow encryption requirements when handling sensitive data.

---

### 👥 Access & Sharing
Access is granted strictly by the **need-to-know** principle.
- Only provide access to people who genuinely require it.
- External sharing must be approved and compliant with contracts and regulations.
- Use security groups for both Power BI workspaces and Fabric domains/warehouses.

---

### 🧭 Data Sources
Use stable, approved, and standardized data sources.
- Use governed sources where applicable.
- Use master data and reference data where available.
- Avoid local Excel files in models and pipelines.

---

### 📊 Data Quality
Maintain and protect the quality of data used for reporting and decision-making.
- Validate that data is correct, complete, and up-to-date.
- Remove duplicates, errors, and outdated data before it reaches Power BI consumption.
- Report data quality issues to the data owner.

---

### 📝 Metadata & Documentation
All solutions must be understandable and maintainable through clear documentation.
- Describe datasets, Fabric tables, and reports (definitions, owners, purpose).
- Use meaningful names for tables, columns, measures, and pipeline steps.

---

### 💾 Storage & Lifecycle
Store and manage data responsibly across its lifecycle.
- Store data only in approved locations.
- Avoid local storage (PBIX, CSV, temporary files) unless explicitly approved.
- Follow retention, deletion, and archiving requirements.

---

### 📦 Reuse & Data Products
Build for reuse where it makes sense.
- Use governed Fabric data products when possible.
- Create semantic models in Power BI that can be reused by other teams.
- Document data product ownership.

---

### 👥 Roles & Accountability
Work with the right roles and follow the required governance framework.
- Align with the Data Lead for the data sources you use.
- Align with project stakeholders on what must be measured, tracked, and reported.
- Consider whether a Legal Risk Assessment (LRA) is required.

---

## ✅ Where to find the clickable checklist
**Issues → New Issue → "Fabric & Power BI Governance Checklist"**
