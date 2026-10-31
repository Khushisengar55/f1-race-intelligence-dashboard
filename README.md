# F1 Race Intelligence Dashboard (2010–2026)

An interactive Tableau data analytics project exploring Formula 1 race performance, team strategy, driver reliability, circuit distribution, tyre compound usage and podium achievements.

## Project Overview

This project uses five supplied CSV datasets to build an analytical workflow in Tableau:
- Data inspection and quality auditing
- Conservative data cleaning and preprocessing
- Tableau worksheets and calculated fields
- Interactive dashboard with KPI cards and filters
- Nine-scene Tableau Story
- Manual performance checks
- Publication through Tableau Public

## Tableau Public

[Open the published F1 Race Intelligence Story](https://public.tableau.com/app/profile/khushi.sengar/viz/F1RaceIntelligenceDashboard2010-2026/Story1)

## Datasets

| Dataset | Rows | Columns | Description |
|---|---:|---:|---|
| circuits | 29 | 9 | Circuit metadata |
| race_results | 6,464 | 42 | Race outcomes, points, DNF and strategy |
| championship_standings | 311 | 10 | Season-level driver standings |
| lap_intelligence | 3,814 | 14 | Lap times, sectors, tyre and DRS data |
| qualifying_results | 3,130 | 16 | Qualifying positions and lap times |
| **Total** | **13,748** | | Combined records across the five files |

## Main Visualizations

1. Driver Performance Leaderboard
2. DNF Analysis by Team
3. Team Championship Trend
4. Tyre Compound Usage
5. Circuit Type Distribution
6. Grand Prix Participation by Country
7. Top 10 Driver Performance
8. Team Performance Ranking
9. Driver Podium Finishes

The dashboard also includes KPI views for total races, drivers, teams and DNFs.

## Tableau Story

The Story contains nine scenes:
1. F1 Race Intelligence – Overview
2. Global Grand Prix Distribution
3. Driver Reliability & DNF Analysis
4. Top Driver Championship Leaderboard
5. Team Championship Performance
6. Team Championship Trajectory (2010–2026)
7. Tyre Compound Strategy Analysis
8. Race Distribution by Circuit Type
9. Driver Podium Achievements

## Performance Checks

Manual checks performed on the published workbook:
- Dashboard load time observed: approximately 5 seconds
- Dashboard visualizations rendered correctly
- DNF Reason filter changed displayed data
- Top N parameter changed the displayed list (10 to 5)
- All nine Story scenes opened and loaded

These are user-observed manual checks, not automated benchmark results.

## Data Quality Notes and Limitations

- The supplied files contain 13,748 records in total.
- The race results include 396 DNF records. Missing finish positions for DNF rows were retained.
- Repeated `(race_id, driver)` combinations were flagged for review rather than silently deleted.
- The qualifying dataset contains placeholder driver/team labels; those records should not be treated as verified real-world driver/team results.
- No driver nationality field is supplied. Country participation refers to Grand Prix host countries, not driver nationality.
- The supplied historical data may be synthetic or modified. It should not be represented as authoritative official Formula 1 historical data without independent validation.

## Tools and Technologies

- Tableau Desktop / Tableau Public
- CSV datasets
- Excel for audit reporting
- Data preparation and validation with Python

## Author

Khushi Sengar

---

This repository is intended for educational and portfolio demonstration. Please review dataset provenance and licensing before redistribution.
