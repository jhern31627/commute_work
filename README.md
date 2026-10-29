# U.S. Commute & Demographic Analytics

## Project Overview
This project evaluates how socioeconomic factors—specifically median household income and population density—influence U.S. commuter transit choices. By analyzing county- and city-level commute data across multiple transport modes (Work-from-Home, carpooling, public transit, drive-alone, and non-vehicular travel), the analysis establishes demographic benchmarks to guide regional transportation planning and remote-work policy strategy.

---

## Technical Stack & Tools
* **Database & Querying:** SQL (CTEs, Subqueries, Window Functions: `PERCENTILE_CONT`, `DENSE_RANK`)
* **Data Processing & Statistical Modeling:** Microsoft Excel (Correlation Matrices, Linear Regression Models, Pivot Tables)
* **Visualization & Reporting:** Power BI (Custom Bookmarks, Visual Filters, Relational Modeling)

---

## Data Pipeline & Modeling
1. **Data Ingestion & Cleansing:** Standardized raw census and demographic datasets; parsed 5-digit `GEOID` codes into a 4-digit `GEOID_SPLIT` relational key for cross-table integration.
2. **Relational Data Modeling:** Created a dedicated state bridge table (`geoid_state`) to connect demographic files with commute statistics.
3. **Segmentation & Statistical Analysis:** Established a 6-tier income group distribution and ran correlation/regression models to evaluate the drivers of Work-From-Home (WFH) and public transit adoption relative to population density and income levels.

---

## Key Features & Insights
* **Income Tier Distribution:** Categorized regions by median household income tiers to identify adoption thresholds for remote work and non-car commuting.
* **Regression Analysis:** Modeled public transit and WFH adoption against population density to isolate structural adoption gaps.
* **Interactive Dashboard:** Designed a multi-page Power BI dashboard featuring county-level filtering, state benchmarks, and modal share trends.
