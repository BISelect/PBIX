# Power BI + GitHub Workflow (PBIP Projects)

This document defines how we work collaboratively on Power BI using **Power BI Project (.pbip)** and **GitHub**.

---

## 1. Goals

- Single source of truth for Power BI reports and models
- Safe, reviewable changes (Pull Requests, code review)
- No PBIX emailing / overwriting each other’s work
- Clear rules to avoid conflicts

---

## 2. Prerequisites

Each developer must have:

- Power BI Desktop (latest version)
- Git installed and configured (`git config user.name`, `git config user.email`)
- Access to the GitHub repository

### 2.1 Enable PBIP in Power BI Desktop

1. Open **Power BI Desktop**.
2. Go to **File → Options and settings → Options → Preview features**.
3. Enable **“Power BI Project (.pbip)”**.
4. Restart Power BI Desktop.

---

## 3. Repository Structure

Example:

```text
/PowerBI
  /SalesReport
    SalesReport.pbip
    SalesReport.SemanticModel/
    SalesReport.Report/
  /FinanceReport
    FinanceReport.pbip
    FinanceReport.SemanticModel/
    FinanceReport.Report/
  /Docs
    POWERBI_GIT_WORKFLOW.md
