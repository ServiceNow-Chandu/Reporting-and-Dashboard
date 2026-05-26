# Reporting Dashboard Lite – ServiceNow

## Project Overview

Reporting Dashboard Lite is a ServiceNow reporting project built to demonstrate operational dashboards, KPI-style reporting, interactive filters, and scheduled report distribution without using Performance Analytics.

This project uses native ServiceNow Reports and Dashboards to provide visibility into Incident, Change, and Problem Management processes.

## Business Requirement

The goal of this project is to provide operational and leadership teams with clear visibility into ITSM performance using native ServiceNow reporting capabilities.

## Features Implemented

- Incident KPI reports
- Change Management reports
- Problem Management reports
- Ops Overview Dashboard
- Service Desk Daily Dashboard
- Interactive Filters
- Scheduled Report Pack
- GitHub documentation and screenshots

## Reports Created

### 1. Open Incidents by Priority
- Table: Incident
- Type: Bar Chart
- Filter: Active = True
- Group by: Priority

### 2. Incident Trend – Last 30 Days
- Table: Incident
- Type: Time Series
- Filter: Opened At = Last 30 Days
- Trend by: Opened At

### 3. MTTR Proxy Report
- Table: Incident
- Filter: Resolved incidents
- Purpose: Measures average resolution performance

### 4. Changes by State
- Table: Change Request
- Type: Donut Chart
- Group by: State

### 5. Change Success Rate
- Closed changes count
- Successful closed changes count
- Used to explain success percentage

### 6. Problems by Known Error
- Table: Problem
- Type: Bar Chart
- Group by: Known Error

## Dashboards Created

### Ops Overview Dashboard

Widgets:
- Open Incidents by Priority
- Incident Trend
- Changes by State
- Problems by Known Error
- Top Assignment Groups by Open Incidents

### Service Desk Daily Dashboard

Widgets:
- Open Incidents by Assignment Group
- Incidents Created vs Resolved
- My Group’s Open Incidents

## Interactive Filters

Interactive filters were added to improve dashboard usability.

Filters:
- Assignment Group
- Priority
- Time Range

## Scheduled Reports

A scheduled report pack named Daily Ops Snapshot was configured to send operational reports by email.

## GitHub Repository Structure

```text
09-reporting-dashboard-lite/
├── README.md
├── docs/
│   ├── report-catalog.md
│   ├── dashboard-walkthrough.md
│   └── lessons-learned.md
└── media/
    ├── ops-dashboard.png
    ├── service-desk-dashboard.png
    └── scheduled-report.png
