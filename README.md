# Coastal Access & Amenities Analysis of Oʻahu, Hawaiʻi

## Overview

This project presents a geospatial analysis of **shoreline public access points and amenities on the island of Oʻahu**, using Python-based GIS workflows. It evaluates shoreline accessibility by examining the availability and distribution of key public amenities that support safe, usable, and equitable coastal access.

By combining spatial data processing, amenity-level analysis, and interactive mapping, the project highlights regional patterns of infrastructure provision and identifies areas that are relatively well-served or under-served across Oʻahu’s coastline.

---

## Project Objectives

- Classify shoreline public access points into four primary coastal regions  
- Standardize and encode amenity data for quantitative analysis  
- Create a composite **amenity score (0–7)** for each access point  
- Compare amenity availability across coastline regions  
- Produce clear static visualizations and interactive web maps  
- Demonstrate applied geospatial analysis and spatial reasoning skills  

---

## Data Sources

### Shoreline Public Access Dataset (2024)  
**Hawaiʻi Statewide GIS Program**

- Geometry: ESRI Shapefile (`Shoreline_Public_Access.*`)
- Attributes: Public amenity indicators  

All raw datasets are stored in `/data/raw/`.

---

## Methods

### 1. Spatial Preparation & Regional Classification
- Load shoreline public access shapefile
- Reproject to WGS84 for mapping consistency
- Assign access points to one of four coastal regions:
  - North Shore  
  - Windward Coast  
  - South Shore  
  - Leeward Coast  
- Apply targeted manual overrides to improve geographic accuracy

---

### 2. Amenity Encoding & Scoring
Each amenity is encoded as a binary indicator (0/1):

- Restroom  
- Showers  
- Picnic facilities  
- Trash receptacles  
- Drinking water  
- Phone  
- Lifeguard presence  

**Amenity Score = Sum of available amenities (0–7)**

---

### 3. Exploratory & Regional Analysis
- Evaluate island-wide amenity availability
- Analyze distribution of amenity scores across access points
- Compare mean amenity availability by coastal region
- Identify patterns of well-served vs under-served shoreline areas

---

### 4. Mapping & Visualization
- Static plots using Matplotlib:
  - Amenity frequency charts
  - Amenity score distribution histograms
  - Regional comparison visualizations
  - Amenity availability heatmap by coastline
- Interactive Folium maps featuring:
  - Region-based thematic mapping
  - Amenity score–based thematic mapping
  - Hover tooltips and detailed popups per access point

Maps are exported to `/outputs/maps/`.

---

## Project Outputs

### Interactive Maps
- `shoreline_access_by_region.html`
- `shoreline_access_by_amenity_score.html`

### Analytical Figures
- Amenity availability bar charts  
- Amenity score histograms  
- Regional comparison plots  
- Amenity availability heatmap  

---

## Technologies Used

- Python  
- Pandas  
- GeoPandas  
- Shapely  
- Folium  
- Matplotlib  
- Jupyter Notebook  
- ESRI Shapefile geospatial data  

---

## Author

**Sarah E.**  
M.S. CyberGIS & Geospatial Data Science (in progress)  
Data Analyst with a focus on GIS, spatial analysis, and environmental data science  


