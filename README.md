# Retail_Catchment_Income_Analysis_Charlotte
Analysis of Walmart retail catchment areas in Charlotte, NC to visualize household income distribution within driving and walking zones using QGIS, Python, and Census data. Helps retail companies optimize site planning, marketing, and customer targeting.


Project Overview:
This project analyzes the catchment areas of retail stores to understand household income distribution around each location. Using Walmart retail locations in Charlotte, NC as an example, it integrates spatial analysis, demographic data, and Python-based data cleaning to generate maps showing potential customer income levels in different travel zones.

The goal is to help retail companies optimize site planning, marketing, and product strategies based on the surrounding community demographics.

Retail Sites:
 Name       , Latitude , Longitude 
 Walmart #1 ,35.2271,-80.8431
 Walmart #2 ,35.2,-80.8
 Walmart #3 ,35.25,-80.9
 Walmart #4 ,35.23,-80.77
 Walmart #5 ,35.26,-80.83

Data Sources
1. Retail Locations – Provided as latitude and longitude.
2. Household Income Data – Extracted from U.S. Census Bureau (Mecklenburg County, NC) including:
- GEOID (Census tract identifier)
- Household income estimates
- Area information
3. Spatial Boundaries – North Carolina shapefiles filtered to Charlotte tracts.

Methodology
1. Geocoding Retail Sites
Plotted the 5 Walmart retail locations in QGIS using a retail cart symbol.
2. Creating Catchment Areas
Used Travel Time Toolbox (Esri) to generate travel-based catchment areas:
Driving: 5 minutes
Walking: 10 minutes
3. Adding Household Income Data
Cleaned Census and shapefile data using Python to produce cleaned_income_data.csv with GEOID and Income.
Uploaded this file to QGIS and joined it with the tract shapefile.
Applied graduated symbology to visualize income variations (yellow = low income, red = high income).
4. Analysis
Mapped household income for each catchment area.
Compared walking vs. driving zones to understand accessible customer demographics.

Tools Used
ARC GIS – Spatial visualization, mapping, and catchment area creation
Python – Data cleaning, filtering, and preparation
Travel Time Toolbox (Esri / GIS Group) – Driving and walking catchment area generation
Census Data & Shapefiles – Income and geographic boundary information


Results / Visualizations
Maps showing driving (5–15 min) and walking (10 min) catchment areas for each Walmart location.
Income distribution visualized using color gradients.
Example Insights:
- Identify high-income areas for premium product promotions.
- Understand local vs regional customer accessibility.
- Plan store inventory and marketing strategies based on demographics.

Business Use & Insights
- This analysis provides actionable insights for retail companies:
- Site Planning – Evaluate potential new store locations.
- Marketing Strategy – Tailor promotions by local household income.
- Inventory Optimization – Stock products according to nearby demographics.
- Accessibizity Analysis – Determine walking and driving reach for customers.
- Competitor Analysis – Compare catchment areas with competitors.
