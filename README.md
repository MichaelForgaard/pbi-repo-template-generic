# <Add Project Name>

**Description:** A template for documenting and managing Power BI and Microsoft Fabric solutions.

> 📚 **This template is used as the practical starting point in the [Power BI, PBIP, GitHub and Fabric Beginner Course](https://github.com/MichaelForgaard/powerbi-fabric-git-beginner-course).**
> If you are following the course, use this template as your working repository.

---

## 🛤️ Which Workflow Are You Using?

This template supports all three workflows from the beginner course. Choose the one that matches your setup:

| Workflow | Description | What to store in `reports/` |
|---|---|---|
| 📄 Path 1 — No-Template GitHub Setup | Browser only, no extra tools | Upload `.pbix` files manually |
| 💻 Path 2 — VS Code + GitHub + PBIP | VS Code + Git, full version history | `.pbip` folder structure |
| ☁️ Path 3 — Fabric + GitHub Integration | Microsoft Fabric + GitHub | Fabric syncs files automatically |

> 💡 Not sure which to use? See the [Comparison and Recommendation](https://github.com/MichaelForgaard/powerbi-fabric-git-beginner-course/blob/main/learning-path/comparison.md) page in the course.

---

## 💼 Using Without Microsoft Fabric

If your organisation does not have a Microsoft Fabric SKU or Premium capacity, you can still get great value from this template using **Power BI Pro** or **Premium Per User (PPU)**!

### What changes:
- ❌ Git Integration (auto-sync between Power BI and GitHub) is **not available**
- ❌ Deployment Pipelines require PPU or Premium
- ✅ GitHub still works as your **documentation and version control hub**
- ✅ All governance, README, and checklist features work exactly the same

### Your workflow (manual — Path 1):
1. Build and edit reports in **Power BI Desktop**
2. Save the `.pbix` file locally
3. Upload it to the `/reports` folder in GitHub manually via:
   - [GitHub Desktop](https://desktop.github.com/) — recommended for beginners
   - The GitHub web UI (drag and drop)
4. Update the README with report descriptions and architecture
5. Open the governance checklist issue and work through it
6. Publish from Power BI Desktop directly to your workspace

### ⚠️ Update your `.gitignore`
By default, `.pbix` files are excluded from version control (because Path 2 and 3 users use `.pbip` instead).
If you are using **Path 1** (no Fabric), remove this line from `.gitignore`:
```
*.pbix
```
This allows your `.pbix` report files to be tracked in GitHub. ✅

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
├── docs/                  # Documentation
│   ├── file-types.md      # Reference: Power BI file types (PBIX, PBIT, PBIP)
│   └── screenshots/       # Report screenshots
├── reports/               # Power BI report files (.pbix, .pbit, or .pbip structure)
│   └── templates/         # Reusable .pbit template files
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

*(Add screenshots if needed — store them in `docs/screenshots/`)*

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

This section applies to **Path 3 — Fabric + GitHub Integration**.

When connected, this means:

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

When using Power BI Git integration (Path 3):

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
1. Clone or use this template to create your repository.
2. Fill in all `<placeholder>` fields in this README.
3. Decide which workflow you are using (see **Which Workflow Are You Using?** above).
4. Update `config/workspaces.json` with your workspace IDs (if applicable).
5. Add your Power BI files to the `/reports` folder.
6. Open the governance checklist issue and work through it.

---

## 📁 Reference

- [Power BI File Types: PBIX, PBIT and PBIP](docs/file-types.md)
- [Beginner Course](https://github.com/MichaelForgaard/powerbi-fabric-git-beginner-course)
