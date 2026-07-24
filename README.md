# AtliQ Grands – Hospitality Domain Dashboard (Power BI)

## Overview
AtliQ Grands is a chain of five-star hotels that has operated across major Indian cities for the past 20 years. In recent years, aggressive moves from competitors combined with gaps in internal decision-making have caused the company to steadily lose market share and revenue — particularly in its luxury and business hotel categories.

To course-correct, AtliQ Grands' management decided to bring **Business and Data Intelligence** into their revenue strategy. With no in-house analytics team, the revenue management team engaged a third-party analyst (this project) to turn their historical booking data into a decision-ready dashboard.

## Problem Statement
- Revenue and market share are declining in the luxury/business hotel segment, but leadership lacks visibility into *why* — which properties, room classes, cities, or booking channels are underperforming.
- Historical booking data exists but sits unused; there is no self-serve way for the revenue management team to track occupancy, pricing, and revenue trends over time.
- Decisions are currently reactive rather than data-driven, putting AtliQ Grands at a disadvantage against competitors who already use BI tools.

## Live Dashboard link
https://app.powerbi.com/view?r=eyJrIjoiZmVlNzdjZDQtZTk0MS00YTlmLTg0MzQtMWI1MTYxNDk0OTZjIiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9

## Objective
Build a Power BI dashboard that gives the revenue management team a single, reliable view of hotel performance — enabling them to spot underperforming properties/channels early and make faster, evidence-based pricing and revenue decisions.

##  Deliverables (Task Scope)
1. **Metrics** — build all KPIs defined in the stakeholder metric list (Revenue, RevPAR, ADR, Occupancy %, Realisation %, DSRN, DBRN, DURN).
2. **Dashboard** — replicate and build out the dashboard per the stakeholder-provided mock-up.
3. **Insights** — surface additional findings not explicitly asked for in the metric list/mock-up, to add analytical value beyond the base requirement.

4. >  Based on the Hospitality Domain project from the **Codebasics** Resume Project Challenge. Data model, base metric definitions, and mock-up dashboard were provided as part of the challenge; DAX implementation, additional KPIs, layout refinements, and insights below are my own work.

<img width="1280" height="800" alt="mock up dashboard_atliq grands" src="https://github.com/user-attachments/assets/b716d33a-5cee-4129-adbe-6a861eb7a6f3" />

## Data model

<img width="1600" height="839" alt="WhatsApp Image 2026-07-24 at 3 33 41 PM" src="https://github.com/user-attachments/assets/956868de-c8a2-4e5a-9ad8-e12440d46540" />

## Dashboard

<img width="1115" height="654" alt="Hospitality domain 7_24_2026 3_52_17 PM (2)" src="https://github.com/user-attachments/assets/7c6ae9f0-5d3e-48e2-a32c-c8e49846be7e" />

##  Dataset
- `dim_date` – calendar/date dimension (day, week, month)
- `dim_rooms` – room class (Standard, Elite, Premium, Presidential)
- `dim_hotels` – property details (property_id, property_name, city, category: Luxury/Business)
- `fact_bookings` – booking-level transactions (booking_id, property_id, check-in/out, room category, revenue_generated, revenue_realized, booking_platform, ratings, status)
- `fact_aggregated_bookings` – daily aggregated capacity & successful bookings per property (used for DSRN/DBRN calculations)

##  Tech Stack
- **Power BI Desktop** – data modeling, DAX, dashboard
- **Power Query** – data cleaning & transformation
- **DAX** – calculated measures for KPIs

- KPIs Created Using DAX:  Total Bookings | Total Revenue | Average Rating | Total Capacity | Total Successful Bookings | Occupancy % | Total Cancelled Bookings Cancellation Rate | Revenue Loss | Total Stay

## Some Important insights from the Dashboard
- Mumbai generates the highest revenue (661 M) followed by Bangalore, Hyderabad and Delhi
- Elite type rooms has the most booking and as well higher cancellation rate
- Delhi tops both in occupancy and rating followed by Hyderabad, Mumbai, Bangalore
- AtliQ Exotica performs better compared to all 7 type of properties revenue, rating,occupancy percentage and cancellation rate.
- ADR stays flat (~12K–13K) all three months while occupancy fluctuates — indicating the property isn't adjusting prices for demand. Dynamic pricing during high-demand weeks could boost RevPar without hurting occupancy.
- June had the highest cancellation rate (25.09%).
- Strengthening partnership with logtrip and journey — both leading in Realisation% at 71% — can help boost bookings, as these channels convert reservations into revenue most efficiently

## Key Learnings:

- Crafting data-driven stories through dashboards
- Understanding business needs & translating them into insights
- Optimizing visuals & using the right charts for effective communication
- Mastering DAX measures for meaningful KPIs





