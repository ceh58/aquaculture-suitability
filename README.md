# Habitat Suitability for Aquaculture
By [Carmen Hoyt](https://ceh58.github.io/) [@ceh58](https://github.com/ceh58)

## About
Aquaculture has the potential to match the production of wild fisheries using just a fraction of ocean space: [0.015% of the global ocean area](https://www.nature.com/articles/s41559-017-0257-9), to be precise. To make efficient use of this space, it is essential to match species of farming potential with their optimal habitat for growth. Many variables influence habitat suitability, but this analysis focused on two main factors: sea surface temperature (SST) and depth. There are 5 main Exclusive Economic Zones (EEZs) off the West Coast of the US: Washington, Oregon, Northern California, Central California, and Southern California. By creating a `suitability()` function, we can determine how much area in each EEZ is suitable for aquaculture for any species of interest.

## Skills
This analysis harnesses the following valuable skills:

- Creating functions for
- Reclassifying rasters
- Clipping raskers

## Repository Structure
```
├── .gitignore
├── README.md
├── aquaculture-suitability.Rproj
├── functions.html # Rendered document
└── functions.qmd # Quarto document detailing the analysis
```
## Data Access

All the data used in this analysis were downloaded from a pre-prepared [Google Drive](https://drive.google.com/file/d/1u-iwnPDbe6ZK7wSFVMI-PpCKaRQ3RVmg/view). It was downloaded, unzipped, and housed in a data/ folder that was not pushed to the repository due to its size. The data in the drive was originally obtained from the following sources:

**Sea Surface Temperature (SST) Data:**

SST data was originally obtained from [NOAA's Daily Global 5km Satellite Sea Surface Temperature Anomaly v3.1](https://coralreefwatch.noaa.gov/product/5km/index_5km_ssta.php) from the years 2008 to 2012 as a GeoTiff. 

**Bathymetry Data:**

Bathymetry data was originally downloaded from the [General Bathymetric Chart of the Oceans (GEBCO)](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area) as a GeoTiff.

**EEZ Data:**

EEZ boundaries were downloaded as a shapefile from [Marineregions.org](https://www.marineregions.org/eez.php).

## References

Bisby, F.A., M.A. Ruggiero, K.L. Wilson, M. Cachuela-Palacio, S.W. Kimani, Y.R. Roskov, A. Soulier-Perkins and J. van Hertum. 2005. (via [SeaLifeBase](https://www.sealifebase.ca/summary/Haliotis-rufescens.html)). 

[GEBCO](https://www.gebco.net/data_and_products/gridded_bathymetry_data/#area) Compilation Group (2024) GEBCO 2024 Grid (doi:10.5285/1c44ce99-0a0d-5f4f-e063-7086abc0ea0f)

Gentry, R. R., Froehlich, H. E., Grimm, D., Kareiva, P., Parke, M., Rust, M., Gaines, S. D., & Halpern, B. S. Mapping the global potential for marine aquaculture. Nature Ecology & Evolution, 1, 1317-1324 (2017) [https://www.nature.com/articles/s41559-017-0257-9](https://www.nature.com/articles/s41559-017-0257-9).

[MarineRegions](https://www.marineregions.org/eez.php). nd. EEZ Boundaries.

NOAA Coral Reef Watch. 2018, updated daily. Daily Global 5km Satellite Sea Surface Temperature Anomaly (Version 3.1, released August 1, 2018). College Park, Maryland, USA: [NOAA Coral Reef Watch](https://coralreefwatch.noaa.gov/product/vs/data.php).

# Acknowledgements
This analysis was adopted from [EDS223: Geospatial Analysis & Remote Sensing Homework #4](https://eds-223-geospatial.github.io/assignments/HW4.html). Thank you to Ruth Oliver [@ryoliver](https://github.com/ryoliver) for preparing the data hosted on Google Drive.
