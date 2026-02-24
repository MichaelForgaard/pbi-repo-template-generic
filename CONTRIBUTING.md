# Contributing Guide

This repository is a Power BI and Microsoft Fabric project connected to Power BI workspaces via Git integration.

## Branch Strategy

| Branch | Environment | Power BI Workspace |
|--------|-------------|-------------------|
| main   | Production  | Prod workspace    |
| test   | Test        | Test workspace    |
| dev    | Development | Dev workspace     |

## Working with pbip Files

Commit the full pbip folder structure when using Git integration. Do not commit pbix files unless Git integration is not in use. Power BI will automatically sync the workspace when changes are pushed to the linked branch.

## Deployment Pipeline

Use the Power BI Deployment Pipeline to promote content from Dev to Test to Prod. Do not manually publish from Power BI Desktop to the Prod workspace.

## Pull Request Process

1. Create a branch from dev for your changes.
2. Fill in all placeholder fields in README.md before raising a PR.
3. All changes must go through a Pull Request. No direct pushes to main.

## Pre-PR Checklist

- All placeholder fields in README filled in
- Architecture diagram added to docs/architecture.png
- Workspace names and URLs updated
- Governance checklist issue created and up to date
