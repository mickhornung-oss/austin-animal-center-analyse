# Austin Animal Center — Data Modeling & Analysis

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Power BI](https://img.shields.io/badge/tool-Power%20BI-F2C811.svg)
![Records](https://img.shields.io/badge/records-79%2C000%2B-blue.svg)

End-to-end data modeling and business intelligence analysis of 79,000+ animal shelter records (Austin Animal Center, 2013–2018). Raw, flat data transformed into a star schema with actionable process optimization insights.

> **Deutsch:** End-to-End Datenmodellierung und Analyse von 79.000+ Tierheim-Datensaetzen mit Sternschema und Power-BI-Dashboard.

## Data Architecture

Built a star schema from a flat, unstructured source dataset:

| Table | Description |
|---|---|
| `fact_events_clean.csv` | All events: intakes, outcomes, adoptions, euthanasias |
| `dim_animal.csv` | Animal metadata (species, breed, age, condition) |
| `dim_date` | Time dimension for seasonal analysis |

## Key Business Findings

**1. Adoption Seasonality**
Adoption rates follow a clear seasonal pattern — peak in summer, drop in winter. Staffing and capacity planning should account for this cycle.

**2. Euthanasia is a Capacity Problem, Not an Intake Problem**
88% of animals arrive in healthy condition. Yet 4% of all euthanasias affect healthy animals. The driver is shelter capacity, not animal health on arrival.

**3. Measurable Improvement Over Time**
Euthanasia rate declined steadily from over 10% to under 8% across the observation period — demonstrating that policy changes have quantifiable impact.

## Tech Stack

- **Power BI** — interactive dashboard and data model
- **Star Schema** — fact + dimension table design
- **CSV** — clean, reproducible data layer

## Files

| File | Description |
|---|---|
| `Abschluss Austin.pbix` | Power BI report (open in Power BI Desktop) |
| `fact_events_clean.csv` | Cleaned fact table |
| `dim_animal.csv` | Animal dimension table |
| `data_dictionary.csv` | Field definitions |

## Open in Power BI

1. Clone the repository
2. Open `Abschluss Austin.pbix` in Power BI Desktop
3. CSV files are pre-referenced and load automatically
