# ITSM Service Desk Analytics

## Overview
An interactive IT Service Management analytics project built with Databricks SQL and Power BI. The dashboard explores service desk ticket volume, SLA performance, resolution times, support teams, and customer satisfaction.

The project uses a synthetic dataset of 8,000 support tickets and related reference tables.

## Tools
- Databricks SQL
- Power BI
- Power Query
- DAX
- CSV

## Data Preparation
Six CSV tables were loaded into Databricks: tickets, users, departments, services, technicians, and assets. The data was reviewed and connected in Power BI using a relational model. Missing resolution and closure values were retained because they represent tickets that had not yet reached those stages.

## Dashboard
1. **Executive Service Overview** – key performance indicators, monthly ticket trend, ticket priority, SLA status, and average resolution time.
2. **Ticket Drivers & Segments** – ticket distribution by support team, department, category, channel, service group, and impact/urgency.
3. **Insights & Recommendations** – first contact resolution, customer satisfaction, reopened tickets, and SLA breach rates.

## Key Findings
- 8,000 tickets were included in the analysis.
- SLA compliance was 86.16% among evaluated tickets.
- Average resolution time was 11.86 hours.
- 17.35% of tickets were reopened.
- P1 Critical tickets had the highest SLA breach rate (36.09%).

## Skills Practiced
- Data preparation and validation
- SQL querying and exploratory analysis
- Data modeling and relationships
- DAX measures and KPI calculations
- Power BI dashboard design and visualization

## Repository Structure
```text
ITSM-Service-Desk-Analytics/
├── data/
├── sql/
├── screenshots/
├── documentation/
├── ITSM-Service-Desk-Analytics.pbix
└── README.md
```

## Author
Jesús Toledo
