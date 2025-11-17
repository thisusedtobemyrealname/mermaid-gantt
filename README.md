# mermaid-gantt

This repository contains a Mermaid Gantt chart for the NACS Agent Hierarchy Mirroring Plan.

## Gantt Chart

The Gantt chart is defined in `gantt-chart.mmd` and visualizes the project timeline with the following phases:

1. **Prerequisites**: Database inventory verification and task delegation (Nov 1-19, 2025)
2. **Environment Setup**: Tools, database structure, and sample data (Nov 17-21, 2025)
3. **Mirroring**: Migration, replication, and stored procedures (Nov 25 - Dec 3, 2025)
4. **Validation**: Testing and comparison of results (Dec 3-5, 2025)

## Viewing the Chart

To view the Gantt chart, you can:
- Use the [Mermaid Live Editor](https://mermaid.live/) and paste the contents of `gantt-chart.mmd`
- Use a Markdown viewer that supports Mermaid diagrams
- Use GitHub's native Mermaid rendering in Markdown files

## Chart Details

```mermaid
gantt
    title NACS Agent Hierarchy Mirroring Plan - Gantt Chart
    dateFormat  YYYY-MM-DD
    axisFormat  %m-%d
    todayMarker off

    section Prerequisites
    Verify DB Inventory & Data Sources:active, prereq, 2025-11-01, 16d
    Task Delegation & Reporting:crit, delegation, 2025-11-17, 3d

    section Step 2: Environment Setup
    Tools & Access Setup:setup-tools, 2025-11-17, 2d
    Database Structure in Postgres:setup-db, 2025-11-17, 4d
    Sample Data Extraction:setup-data, 2025-11-17, 3d

    section Step 3: Mirroring
    Migration & Replication:mirr-mig, 2025-11-25, 5d
    Stored Procedures Replication:mirr-proc, 2025-12-01, 2d

    section Step 4: Validation
    Run Procedure in Oracle (Result A):val-oracle, 2025-12-03, 1d
    Run Migrated Procedure in Postgres (Result B):val-postgres, 2025-12-03, 1d
    Compare Results & Sign-off:val-compare, 2025-12-04, 1d
```
