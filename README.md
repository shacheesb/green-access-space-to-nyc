# green-access-space-to-nyc
# How Green Is Your Block? 🌳

**An end-to-end geospatial data science project using PostGIS and Python to assess neighborhood-level access to public parks in New York City.**


##  Overview

Urban access to green space is a key indicator of community well-being, environmental equity, and livability. This project evaluates how many NYC neighborhoods are within walking distance (500 meters) of a public park.

Using open data, spatial databases, and Python, I created a reproducible pipeline to:
- Load and clean city spatial data
- Perform spatial buffer and join operations using **PostGIS**
- Visualize neighborhood accessibility using **GeoPandas** and **Matplotlib**
- Quantify underserved areas


## Tools Used

- PostgreSQL + PostGIS (spatial SQL operations)
- Python (GeoPandas, Matplotlib, SQLAlchemy, Psycopg2)
- Jupyter Notebook (full pipeline + visualization)
- NYC Open Data

## Key Insights from the Analysis
 99.97% of NYC neighborhoods have access to at least one public park within 500 meters.

 Queens has the largest total green space area (in acres), while Brooklyn has the highest number of individual park properties.

 A small number of neighborhoods (representing ~0.03% of NYC’s land area) are underserved by nearby green space.

 Population-weighted analysis showed that ~0.4% of NYC’s residents live in neighborhoods without immediate park access, highlighting equity gaps in high-density zones.

 Some neighborhoods had less than 0.5 acres of green space per 1,000 residents, falling below urban health standards.

 Identified and mapped the top 5 most populated “park deserts” in NYC, ideal candidates for future green infrastructure projects.

 Only a small portion of parks are classified as waterfront, indicating potential for new public space development along NYC’s coastlines.

 The majority of NYC’s parks are playgrounds, followed by gardens and passive green spaces.

##  Data Sources

- 🏞️ [NYC Parks Properties](https://data.cityofnewyork.us/Recreation/Parks-Properties/enfh-gkve)
- 🗺️ [2020 NYC Neighborhood Tabulation Areas](https://data.cityofnewyork.us/City-Government/2020-Neighborhood-Tabulation-Areas-NTAs-/9nt8-h7nd)


##  Results

```python
Neighborhood Access Summary:
Has Access    99.97%
No Access      0.03%


