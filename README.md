# <Add Project Name>

**Description:** A template for documenting and managing Power BI and Microsoft Fabric solutions, including operational details, report structure, architecture, governance, and deployment information.

---

## ✅ Start Here: Governance Checklist

This template includes an **optional clickable governance checklist** as a GitHub Issue Template.

**How to use it:**
1. Go to **Issues**
2. Click **New issue**
3. Select **"Fabric & Power BI Governance Checklist"**
4. Scroll down and click **Create**
5. You now have a clickable list to follow.

> 💡 Recommended: Create the checklist issue at project start and keep it updated throughout development and release. Close it when the solution goes to production.

---

## 📂 Repository Structure

```text
├── .github/               # GitHub configuration (Issue templates)
│   └── ISSUE_TEMPLATE/    # Clickable issue forms (YAML)
├── config/                # Configuration files (workspace IDs etc.)
├── docs/                  # Documentation (screenshots, architecture diagrams)
├── reports/               # Power BI report files (.pbix) or PBIP structure
├── scripts/               # Deployment / automation / CI/CD scripts
└── README.md              # Main documentation
```

---

## Workspace Name
<insert Power BI workspace name here>

---

## Operational Details
- **Cost / Budget Reference:** <Cost Code or Reference>
- **Project Mandate:** <Brief note on operational scope>

---

## Ticket / Issue References
- **Ticket ID:** <insert link>
- **Change Request:** <insert link>

---

# Report Documentation

Describe the purpose of the reports in this solution and how they are organized.
Mention access control (e.g., security groups) and any relevant notes.

---

## Example Report Sections

### <Report Name>
- **Audience:** <who can access>
- **Sources:** <list data sources>
- **Description:** <short summary of what the report shows>
- **Key Measures:**
  - <measure 1>
  - <measure 2>
- **Calculated Columns:**
  - <column 1>
  - <column 2>

*(Add screenshots if needed)*

---

# Architecture

Explain how the reports are deployed (Dev/Test/Prod) and exposed to end users via Power BI App.

## Workspaces
- <link>
- <link>

## Deployment Pipeline
- <link>

## Fabric Capacity
- <Capacity Name / ID>

## Power BI App
- <link>

## CICD Workflow
Briefly describe your CI/CD approach (e.g., branch strategy, deployment pipeline usage).

---

## Architecture Diagram
![Architecture](docs/architecture.png)

---

# Git Integration and Deployment Pipelines

This repository is connected to a Power BI workspace using **Git integration**. This means:

- Your Power BI workspace is linked to this GitHub repository.
- Changes made in this repository are automatically synced to the workspace.
- Deployment pipelines in Power BI manage promotion across environments.

### Workflow:
1. **Development** → Build and edit reports in the Dev workspace.
2. **Test** → Validate reports in the Test workspace.
3. **Production** → Publish for end users in the Prod workspace.

### How to Use:
- Make changes in the `/reports` folder (Power BI files).
- Commit and push to the branch linked to your Power BI workspace.
- Use the Power BI deployment pipeline to promote changes across environments.

---

## Branch Strategy
- `main` → Production-ready code
- `dev` → Development workspace
- `test` → Testing workspace

---

# Automated vs Manual

When using Power BI Git integration:

✅ **Automated by Power BI**
- `.pbip` folder structure for reports and datasets.
- Metadata files (`report.json`, `dataset.json`) for version control.
- Sync between GitHub and Power BI workspace.
- Deployment pipeline promotions (inside Power BI).

❌ **Manual Documentation Needed**
- Operational details (cost codes, ticket references).
- Architecture overview and diagrams.
- Access control (security groups, roles).
- Data sources and refresh strategy.
- Branch strategy and contribution guidelines.

---

# Getting Started
1. Clone the repository:
   ```bash
   git clone <repo-url>
   ```
2. Fill in all `<placeholder>` fields in this README.
3. Update `config/workspaces.json` with your workspace IDs.
4. Connect your Power BI workspace via Git integration.
5. Open the governance checklist issue and work through it.