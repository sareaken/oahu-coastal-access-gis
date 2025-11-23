# Coastal Access & Amenities Analysis of Oʻahu, Hawaiʻi

This project analyzes shoreline public access points on the island of Oʻahu using geospatial data, Python, and GIS workflows. The study integrates spatial access point geometry with detailed amenity attributes to evaluate access quality, regional distribution, and service availability across the island’s coastline.

The goal of this project is to demonstrate applied geospatial analysis skills relevant to natural resource consulting, environmental planning, and coastal management.

---

## Objectives

1. Integrate shoreline public access geospatial data with amenity attributes.  
2. Create an amenity-based quality scoring system for each access point.  
3. Analyze access density and amenity distribution across Oʻahu.  
4. Produce professional cartographic outputs and an interactive map.  
5. Provide interpretable insights regarding coastal access infrastructure.

---

## Data Sources

### 1. Shoreline Public Access Dataset (2024)  
Hawaiʻi Statewide GIS Program  
- Geometry: Shapefile set (`Shoreline_Public_Access.*`)  
- Attributes: Amenities CSV (`Shoreline_Public_Access.csv`)

### 2. Supplemental Layers
- Oʻahu coastline shapefile   

All raw datasets are stored in `/data/raw/`.

---

## Methods

### 1. Data Cleaning
- Load shoreline public access shapefile  
- Load amenity attributes from CSV  
- Standardize amenity fields  
- Merge geospatial and tabular data on a unique site identifier  
- Export cleaned dataset to `/data/processed/`

### 2. Amenity Quality Score

Each access point receives one point for each available facility:

- Restroom  
- Shower  
- Picnic facilities  
- Trash receptacle  
- Drinking water  
- Phone  
- Lifeguard presence  

**Amenity Score = Total points (0–7)**

### 3. Access Density Analysis

- Count access points per region or coastline segment  
- Generate spatial density visualizations  
- Identify high- and low-access areas  

### 4. Amenities Analysis

- Distribution of amenities across access points  
- Region-level comparisons  
- Clustering of high-score vs low-score sites  
- Identification of underserved coastline segments  

### 5. Mapping and Visualization

- Static GIS outputs using GeoPandas and Matplotlib  
- Interactive web map (Folium) with:  
  - Clickable access points  
  - Amenity popups  
  - Color-coded scores  

Maps are exported to `/outputs/maps/`.

---

## Project Outputs

### Static Maps
- Access point density map  
- Amenity score distribution map  
- Region-level access summaries  

### Interactive Map
`folium_interactive_map.html` (stored in `/outputs/maps/`)

### Analytical Figures
- Amenity frequency plots  
- Score distribution histograms  
- Regional comparison charts  

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
Data Analyst and aspiring GIS/Remote Sensing professional  


