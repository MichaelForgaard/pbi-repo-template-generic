# reports

This folder contains Power BI report files.

## What to Put Here

Depending on the workflow you are using (see the main README):

| Workflow | What to store here |
|---|---|
| 📄 Path 1 — No-Template GitHub Setup | Upload `.pbix` files manually via GitHub web UI or GitHub Desktop |
| 💻 Path 2 — VS Code + GitHub + PBIP | Place the `.pbip` folder structure here (e.g., `My-Report/`) |
| ☁️ Path 3 — Fabric + GitHub Integration | Fabric will automatically sync report files here |

## Templates

Store reusable `.pbit` template files in `reports/templates/`.

## Notes

- For **Path 1**: Make sure to remove `*.pbix` from `.gitignore` so your files are tracked.
- For **Path 2**: The `.pbip` folder structure contains a `report/` and `dataset/` subfolder automatically created by Power BI Desktop.
- For **Path 3**: Do not manually edit files in this folder — Fabric manages the sync.
