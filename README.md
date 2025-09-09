# High resolution PM₂.₅ Air Quality Analysis with Google Earth Engine &amp; Xarray
## Overview
This project demonstrates how to analyze air pollution (PM₂.₅) using global datasets, Google Earth Engine (GEE), and Python. It extracts daily, monthly, and annual averages of PM₂.₅ concentrations for a selected region of interest (ROI), and visualizes spatial and temporal variations.

By integrating Earth Engine ImageCollections with xarray, the workflow allows flexible statistical analysis, time series extraction, and geospatial plotting, useful for environmental monitoring, health impact studies, and policy support.

## Tools & Libraries

Python: xarray, pandas, matplotlib, numpy

Geospatial:
Google Earth Engine (GEE) – dataset access & processing

geemap – interactive map visualization and ROI selection

xee – bridge between Earth Engine collections and xarray

Environment: Google Colab / Jupyter Notebook

## Data Sources

- GHAP Global PM₂.₅ Dataset
- Daily PM₂.₅: projects/sat-io/open-datasets/GHAP/GHAP_D1K_PM25
- Monthly PM₂.₅: projects/sat-io/open-datasets/GHAP/GHAP_M1K_PM25

- Temporal coverage: 2017–2023

- Spatial resolution: ~1 km

daily_pm25.csv → Time series of daily average PM₂.₅ in Western Province, Sri Lanka
<img width="534" height="405" alt="image" src="https://github.com/user-attachments/assets/0927b9d8-6af8-45e3-a186-b53ceed63bd8" />

Grid of monthly mean concentration maps
<img width="1207" height="889" alt="image" src="https://github.com/user-attachments/assets/dc2dc834-955e-490b-9985-4431aef4f5e1" />

Plots of annual variations
<img width="928" height="590" alt="image" src="https://github.com/user-attachments/assets/f4c89804-13bd-4dff-b6fd-ddb3869ec4a1" />

## Example Use Cases
1. Tracking urban air quality over time
2. Comparing seasonal air pollution trends
3. Supporting environmental policy and health research
4. Linking PM₂.₅ exposure with satellite-based indicators (NDVI, population, etc.)

## Notes
- Scaling factor 0.1 applied to dataset values (as per GHAP documentation).
- Colab recommended with GPU/TPU for efficiency when handling large datasets.
