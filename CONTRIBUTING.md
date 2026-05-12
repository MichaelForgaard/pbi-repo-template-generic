# Contributing

Thank you for contributing to this Power BI and Microsoft Fabric solution repository.

---

## Which Workflow Are You Using?

This repository supports three workflows from the [Power BI, PBIP, GitHub and Fabric Beginner Course](https://github.com/MichaelForgaard/powerbi-fabric-git-beginner-course):

| Workflow | Description |
|---|---|
| 📄 Path 1 — No-Template GitHub Setup | Upload `.pbix` files manually via the GitHub web UI or GitHub Desktop |
| 💻 Path 2 — VS Code + GitHub + PBIP | Edit `.pbip` files locally using VS Code and Git |
| ☁️ Path 3 — Fabric + GitHub Integration | Changes are synced directly from a Microsoft Fabric workspace |

---

## Branch Strategy

| Branch | Purpose |
|---|---|
| `main` | Production-ready code |
| `dev` | Development workspace (linked via Fabric Git integration if applicable) |
| `test` | Test workspace |

Create feature branches from `dev` and open a pull request when your changes are ready to review.

---

## How to Contribute

1. Create a branch from `dev` (or `main` for documentation-only changes).
2. Make your changes in the appropriate folder (`reports/`, `docs/`, etc.).
3. Update the README if your changes affect report structure, architecture, or access.
4. Open a pull request with a clear description of what changed and why.
5. Request a review from the relevant team member.

---

## What Needs Manual Updates

Some things are **not** automated by Power BI or Fabric and must be kept up to date manually:

- `README.md` — Operational details, report descriptions, architecture
- `docs/` — Architecture diagrams, screenshots, access matrix
- `config/workspaces.json` — Workspace IDs and environment references
- Governance checklist issue — Progress tracking throughout the project
