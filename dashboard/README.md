# Excel Dashboard

The final Excel workbook (`Population_Clean` table → Data Model → PivotTables → Dashboard) contains an interactive dashboard titled **"Population Camp Analysis — From Data to Human Impact"** covering 2017–2018.

> **Note:** The dashboard screenshot (`dashboard.png`) and the full Excel workbook could not be uploaded through the connected GitHub integration used for this update. That integration only writes text content — confirmed by testing it directly — so binary files (images, `.xlsx`) can't be transferred through it without corruption. Please add the following two files to this folder directly on GitHub (drag-and-drop upload on the repo page works well for this):
>
> - `dashboard/dashboard.png` — the dashboard screenshot (once added, it will render automatically in this file and in the main README)
> - `dashboard/population_camp_data_Clean.xlsx` — the full workbook, if you'd like it included as a portfolio deliverable (it's a reasonable size at ~2.4 MB)
>
> The values below were read directly from the workbook, so this write-up doesn't depend on either file being present.

![Population Camp Analysis Dashboard](dashboard.png)

## KPI Measures (DAX)

| Measure | Value |
|---|---|
| Total Members | 59,006,538 |
| Total Male | 25,552,478 |
| Total Female | 33,454,060 |
| Total Houses | 1,187,621 |
| Total Rooms | 270,699 |
| Total Flats | 456,167 |
| Total Tents | 279,030 |
| Total House Units | 181,725 |
| Male % | 43.30% |
| Female % | 56.70% |
| Avg People per House | 49.68 |

## Country Summary

| Country | Total Members | Total Male | Total Female | Total Houses | Female % | Male % |
|---|---|---|---|---|---|---|
| Iraq | 7,869,862 | 3,432,382 | 4,437,480 | 163,921 | 56.39% | 43.61% |
| Libya | 7,719,390 | 3,327,501 | 4,391,889 | 156,005 | 56.89% | 43.11% |
| Syria | 19,457,159 | 8,436,522 | 11,020,637 | 389,439 | 56.64% | 43.36% |
| Yemen | 23,960,127 | 10,356,073 | 13,604,054 | 478,256 | 56.78% | 43.22% |

## Housing Distribution by Country

| Country | Rooms | Flats | Tents | House Units |
|---|---|---|---|---|
| Iraq | 36,099 | 60,821 | 42,758 | 24,243 |
| Libya | 46,464 | 78,347 | 0 | 31,194 |
| Syria | 69,680 | 117,426 | 155,552 | 46,781 |
| Yemen | 118,456 | 199,573 | 80,720 | 79,507 |

## Population by Year

| Year | Total Members |
|---|---|
| 2017 | 30,142,186 |
| 2018 | 28,864,352 |

## Top 5 Cities by Population

| City | Total Members |
|---|---|
| Ibb | 4,201,749 |
| Aden | 4,201,405 |
| Khantuman | 4,141,469 |
| Al Hudaydah | 4,119,537 |
| Atma | 3,920,683 |

## Dashboard Visuals

- **Key Figures cards** — the KPI measures above, shown as summary cards.
- **Population by Country** (clustered column chart) — Total Members, Male, Female, and Houses per country.
- **Housing Distribution by Country** (horizontal bar chart) — Total House Units, Tents, Flats, and Rooms per country.
- **Top 5 Cities by Population** (horizontal bar chart).
- **Total Members by Year** (donut chart) — 2017 vs. 2018 share.
- **Filters** — Country and Year slicers connected to all visuals.

See [`../analysis/analytical_insights.md`](../analysis/analytical_insights.md) for the interpretation of these results.
