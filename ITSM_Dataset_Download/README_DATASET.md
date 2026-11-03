# ITSM Practice Dataset
Synthetic data for Databricks SQL, Power Query, data modeling, DAX and Power BI.

## Files
- tickets.csv: 8,000 ticket records (fact table)
- users.csv: 600 requesters
- departments.csv: 10 departments
- services.csv: 12 IT services
- technicians.csv: 30 support technicians
- assets.csv: 500 IT assets

## Relationships
- tickets.user_id -> users.user_id
- tickets.department_id -> departments.department_id
- tickets.service_id -> services.service_id
- tickets.technician_id -> technicians.technician_id
- tickets.asset_id -> assets.asset_id
- users.department_id -> departments.department_id

## Key fields
ticket_id, created_at, resolved_at, closed_at, status, priority, category, subcategory, channel, impact, urgency, response_time_hours, resolution_time_hours, sla_target_hours, sla_status, reopened_count, satisfaction_score, first_contact_resolution.

SLA practice targets: P1=4h, P2=8h, P3=24h, P4=72h. Unresolved tickets have null resolution/closure timestamps and SLA status Not Evaluated. Dates span 2025-01-01 through 2026-10-30. All data is synthetic and contains no real company or customer information.

## Suggested report pages
1. Executive Service Overview: tickets, status, SLA, response/resolution time, backlog, monthly trends.
2. Ticket Drivers & Segments: services, categories, priorities, departments, teams and asset types.
3. Insights & Recommendations: SLA gaps, reopened tickets, satisfaction and recurring issues.
