
# California Wildfire Analysis – Palisades & Eaton Fires, February 2025

##### Author: Henry Oliver
##### Date: December 12, 2025

## **Purpose**
 The purpose of this walkthrough is to utilize false color satellite imagery, social demographic data, and geospatial methods to investigate the extent and effects of the Eaton and Palisades wildfires in California in January of 2025. First, in the 'False Color Imagery and Fire Extent' section this analysis will walk through the steps necessary to display Landsay 8 satellite imagery overlayed with estimated perimeters of the 2025 LA County Palisades and Eaton Fires. Afterwards, the 'Environmental Justice Investigation' will provide the steps necessary to spatially visualize social demographic information from the California Environmental Justice Index in an effort to analyze environmental justice impacts of the LA fires. Data sources are provided throughout this document.

## **Background**
The Palisades and Eaton fires burned across parts of Los Angeles County, leaving visible scars on the landscape. Using Landsat satellite imagery, we can highlight burn areas, compare pre- and post-fire conditions, and better understand the extent and distribution of damage. Remote sensing provides an objective, large-scale view that complements on-the-ground assessments and helps support recovery planning and ecological monitoring. In explorations of the effects of these fires, it's important to take environmental justice factors into consideration. Environmental justice examines how environmental hazards and disasters impact different communities, particularly whether vulnerable or marginalized populations bear a disproportionate burden. By combining fire perimeter data with Census demographic and socio-economic information, we can assess whether certain income levels, racial groups, or other demographic characteristics were overrepresented in affected areas—critical information for equitable recovery planning and future risk mitigation.

## Repository Structure
```
.
├── fires-combined.ipynb      # Jupyter Notebook with analysis workflow
├── .gitignore          # Git ignore file
├── README.md           # Project overview and instructions
└── data/               # Folder to store datasets (currently empty, see data sources for acces information)
```

- **analysis.ipynb**: Contains all code and visualizations for the Landsat imagery and fire perimeter overlay analysis.  
- **data/**: Should be populated with the datasets referenced below before running the notebook.  

## Data Sources
- **Eaton Fire Perimeter (Shapefile)**  
  County of Los Angeles. (2025). *Eaton fire perimeter (Version 2025-02-21) [Shapefile]*. Los Angeles County GIS Hub. [Link](https://egis-lacounty.hub.arcgis.com/datasets/lacounty::palisades-and-eaton-dissolved-fire-perimeters-2025/explore?layer=0)

- **Palisades Fire Perimeter (Shapefile)**  
  County of Los Angeles. (2025). *Palisades fire perimeter (Version 2025-02-21) [Shapefile]*. Los Angeles County GIS Hub. [Link](https://egis-lacounty.hub.arcgis.com/datasets/lacounty::palisades-and-eaton-dissolved-fire-perimeters-2025/explore?layer=1&location=34.133066%2C-118.349606%2C9.60)

- **Landsat 8 Imagery of Los Angeles County (NetCDF)**  
  Microsoft Planetary Computer. (2025). *Landsat 8 imagery of Los Angeles County (February 23, 2025) [NetCDF]*. [Link](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2)

 - **California Environmental Justice Index (EJI)**
  California Environmental Protection Agency. (2025). *CalEnviroScreen 4.0 Geodatabase (May 14, 2021) [GeoDataBase]*. [Link](https://calenviroscreen-oehha.hub.arcgis.com/documents/c1b480ac4b564f26a7d8c5582cab8b60)



## Notes
- Before running the notebook, download the data from the links above and place them in the `data/` folder.  
- The analysis produces a **false-color map** showing burned areas (red) and the outlined fire perimeters, providing a visual assessment of fire impact.
- The analysis also produces a figure displaying wealth disparity in burn areas.

## References
County of Los Angeles. (2025). Eaton fire perimeter (Version 2025-02-21) [Shapefile]. Los Angeles County GIS Hub. https://egis-lacounty.hub.arcgis.com/datasets/lacounty::palisades-and-eaton-dissolved-fire-perimeters-2025/explore?layer=0

County of Los Angeles. (2025). Palisades fire perimeter (Version 2025-02-21) [Shapefile]. Los Angeles County GIS Hub. https://egis-lacounty.hub.arcgis.com/datasets/lacounty::palisades-and-eaton-dissolved-fire-perimeters-2025/explore?layer=1&location=34.133066%2C-118.349606%2C9.60

Microsoft Planetary Computer. (2025). Landsat 8 imagery of Los Angeles County (February 23, 2025) [NetCDF]. https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2

Stanford Woods Institute for the Environment. (2025, January 9). Social and economic disparities impact wildfire protection. Stanford University. https://woods.stanford.edu/news/social-and-economic-disparities-impact-wildfire-protection

California Office of Environmental Health Hazard Assessment. (n.d.). CalEnviroScreen data portal [Data portal]. ArcGIS Hub. Retrieved November 18, 2025, from https://calenviroscreen‑oehha.hub.arcgis.com/#Data