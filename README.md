# Identifying Digital Dark Zones

This project aims to identify and analyze **Digital Dark Zones**, regions with poor internet connectivity and limited economic development, using datasets from **Ookla Speedtest** and **VIIRS Nighttime Lights**.

## Datasets Used

### 1. Ookla Speedtest Data
- **Metrics**:
  - Download/upload speeds
  - Latency
  - Device counts
- **Spatial Coverage**: Global, represented in ~610.8m × 610.8m tiles.
- **Temporal Coverage**: Quarterly data from Q1 2019 to Q2 2024.
- **Focus**: Identifies areas with low internet speeds, high latency, or low device count indicating poor connectivity.

### 2. VIIRS Annual Composites
- **Metrics**:
  - Radiance values representing nighttime light activity.
- **Spatial Coverage**: Global, with ~500m resolution.
- **Temporal Coverage**: Annual data from 2012 to 2021.
- **Focus**: Can indicate economic activity or development, with dimmer regions indicating lower development.

## Focus Areas
- **Countries Analyzed**: Mongolia, Madagascar, Laos.
- **Date Range**: 1/1/2023 to 30/6/2023.

## Analysis Goals
- **Identify Digital Dark Zones**: Regions with both poor internet connectivity (as indicated by Ookla data) and low economic or developmental activity (as indicated by VIIRS nighttime radiance data).
- **Spatial & Statistical Analysis**: Analyzing and visualizing the data to identify geographic patterns and correlations between internet connectivity and development levels.

## Methodology

1. **Data Preprocessing**:
   - Cleaned and aligned Ookla Speedtest data and VIIRS nighttime light data.
   - Addressed missing data and outliers.

2. **Spatial Analysis**:
   - Used Geographic Information Systems (GIS) tools to map data for the selected countries (Mongolia, Madagascar, Laos).
   - Identified regions with both low-speed internet and low nighttime light activity.

3. **Statistical Analysis**:
   - Correlated internet speeds with nighttime light data to understand the relationship between digital access and development.
   - Performed cluster analysis to identify potential digital dark zones.

4. **Visualization**:
   - Created maps and charts to visually represent digital gaps across regions.
   - Generated time-series plots to show changes over time.

## Results

The project identified several areas in Mongolia, Madagascar, and Laos where poor connectivity and low economic activity overlap. These regions can be considered potential **Digital Dark Zones** that require targeted interventions for infrastructure development and digital access improvement.

## Tools and Technologies

- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, GeoPandas
- **GIS Tools**: QGIS, ArcGIS
- **Datasets**:
  - Ookla Speedtest Data
  - VIIRS Nighttime Lights Data

## Getting Started

To run the analysis on your local machine, follow these steps:

### Prerequisites
- Python 3.x
- Install required libraries:
  ```bash
  pip install pandas numpy matplotlib seaborn geopandas
