# green-access-space-to-nyc
# How Green Is Your Block? 🌳

**An end-to-end geospatial data science project using PostGIS and Python to assess neighborhood-level access to public parks in New York City.**

---

##  Overview

Urban access to green space is a key indicator of community well-being, environmental equity, and livability. This project evaluates how many NYC neighborhoods are within walking distance (500 meters) of a public park.

Using open data, spatial databases, and Python, I created a reproducible pipeline to:
- Load and clean city spatial data
- Perform spatial buffer and join operations using **PostGIS**
- Visualize neighborhood accessibility using **GeoPandas** and **Matplotlib**
- Quantify underserved areas

---

## Tools Used

- PostgreSQL + PostGIS (spatial SQL operations)
- Python (GeoPandas, Matplotlib, SQLAlchemy, Psycopg2)
- Jupyter Notebook (full pipeline + visualization)
- NYC Open Data

---

##  Data Sources

- 🏞️ [NYC Parks Properties](https://data.cityofnewyork.us/Recreation/Parks-Properties/enfh-gkve)
- 🗺️ [2020 NYC Neighborhood Tabulation Areas](https://data.cityofnewyork.us/City-Government/2020-Neighborhood-Tabulation-Areas-NTAs-/9nt8-h7nd)

---

##  Final Map

![Map of Park Access in NYC](maps/nyc_park_access.png)

🟢 = Neighborhood has park access  
🔴 = Neighborhood lacks a park within 500 meters

---

## 📊 Results

```python
Neighborhood Access Summary:
Has Access    99.97%
No Access      0.03%


