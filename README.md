# Corruption-Perception-Index-Dashboard #

## Corruption Perception Index Dashboard — Concise Overview ##

This Python/Dash application visualizes both current (2024) and historical CPI data:

1. **Data Loading & Preprocessing**
   - Reads `CPI2024.csv` and `CPI-historical.csv`.
   - Drops missing values, scales numeric features, and encodes categories.

2. **Feature Engineering**
   - Computes quartile-based corruption levels.
   - Applies PCA to reduce numeric data to two components.
   - Selects top 5 features correlated with corruption levels.

3. **Static Visualizations**
   - ***Histogram***: Distribution of CPI scores.
   - ***Scatter Plot***: CPI Score vs. Rank by region.
   - ***Choropleth Map***: 2024 CPI ranking by country.
   - ***PCA Plot***: 2D projection colored by corruption quartiles.
   - All use a dark Plotly template for consistency.

4. **Historical Trends**
   - ***Line Chart***: Global average CPI over years.
   - ***Text Block***: Average change, top 5 improvers and decliners since earliest records.

5. **Animated Map**
   - ***Animated Choropleth***: Year-by-year CPI changes with slider controls.

6. **Dashboard Layout**
   - Dark-themed Bootstrap (`CYBORG`) with tabs for each section.
   - Uses `dcc.Graph`, `dash_table.DataTable`, and HTML components for text insights.

This concise structure highlights how corruption perception has evolved globally and allows interactive exploration of the data.
