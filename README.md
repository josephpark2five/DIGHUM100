# Detroit Mapping — DIGHUM 100 Final Project
**Author:** Joseph Park • **Course:** Digital Humanities 100 (Spring 2025)  
Interactive notebook: **`detroit_mapping.ipynb`**

This project visualises how New-Deal redlining boundaries intersect with the
childhood locations and later life outcomes of low-income children in
Detroit.  The Folium map layers, at 2020 census-tract resolution, include  

1. **Low-income child density (2000)** – counts per km² by race  
2. **Mean adult-income percentile** those children reach (Opportunity Atlas)  
3. **Shannon race-diversity index** of the same child population  
4. **Majority-race indicator** (> 50 % of low-income children)  
5. **1939 HOLC grades** (Mapping Inequality)  
6. **Road network** (2024 TIGER/Line) for orientation  

## Data sources

| Dataset | Citation | Files in repo |
|---------|----------|---------------|
| **Opportunity Atlas, Module 1 – Household Income & Incarceration for Children from Low-Income Households by Census Tract, Race, and Gender** | Chetty, Raj, et al. *Opportunity Atlas Data Tables: Neighborhood Mobility Outcomes.* U.S. Census Bureau & Opportunity Insights, 2018 (rev. 2024). <https://www.census.gov/programs-surveys/ces/data/public-use-data/opportunity-atlas-data-tables.html> | `Opportunity_Atlas_Data_Tables/` |
| **HOLC Residential Security (“Redlining”) Maps, 1935-1940** | Nelson, Robert K., et al. *Mapping Inequality: Home Owners’ Loan Corporation Security Maps.* American Panorama, University of Richmond. Accessed 2025-06-30. <https://dsl.richmond.edu/panorama/redlining/> | `Mapping_Inequality/mappinginequality.json` |
| **TIGER/Line Shapefiles** | U.S. Census Bureau. *TIGER/Line Shapefiles: 2020 Census Tracts (tl_2020_26_tract.shp) and 2024 Roads (tl_2024_26163_roads.shp).* <https://www.census.gov/geographies/mapping-files/time-series/geo/tiger-line-file.html> | `2020_Census_TIGER/` |

## Quick start

```bash
git clone https://github.com/josephpark2five/DIGHUM100.git
cd DIGHUM100

# Create and activate a virtual environment
python -m venv .venv && source .venv/bin/activate

# Install dependencies
pip install -r requirements.txt   # or see the library list below

# Launch the notebook
jupyter notebook detroit_mapping.ipynb
````

### Key Python libraries

* `geopandas` ≥ 0.14
* `folium` ≥ 0.16
* `mapclassify`, `branca`, `shapely`, `pandas`, `numpy`

To freeze the exact versions you used:

```bash
pip freeze > requirements.txt
```

© 2025 Joseph Park.
This repository is for educational use under UC Berkeley course DIGHUM 100.

```
```
