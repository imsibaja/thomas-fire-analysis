# Thomas Fire Environmental Impact Analysis

## About
This repository contains notebooks `thomas-fire-analysis.ipynb` and `thomas-fire-analysis.ipynb` and a combination of the two `final-project-thomas-fire.ipynb` whose goal are to analyze the effects on AQI and fire scarring from the 2017 Thomas Fire. This was one of California’s largest wildfires, which burned over 280,000 acres across Ventura and Santa Barbara counties. This repository includes examinations the fire’s impact on air quality using AQI data from the US Environmental Protection Agency and visualizes burn severity and fire scars using false-colored Landsat multispectral geospatial data.

### Highlights

- Import and explore AQI and Landsat data to analyze the Thomas Fires
- Create time series maps to explore the impact of the wildfires on AQI
- Create true and false color images to highlight the fire’s breadth
- Visualize the false color fire scar alongside perimeter data for detailed analysis 

### Data

#### U.S. Air Quality Index (AQI)

The U.S. Air Quality Index (AQI), developed by the EPA, communicates outdoor air quality and associated health risks through six color-coded categories, ranging from “Good” (AQI ≤ 50) to “Hazardous” (AQI > 300). AQI values up to 100 indicate satisfactory air quality, aligned with national health standards, while values above 100 signal unhealthy conditions The color-coded system enables quick identification of air quality concerns in communities.

#### Landset 8 Satellite Collection

This dataset consists of simplified bands (red, green, blue, near-infrared, and shortwave infrared) from Landsat Collection 2 Level-2 surface reflectance data, which was atmospherically corrected and captured by NASA’s Landsat 8 satellite. It was sourced from the Microsoft Planetary Computer data catalog and preprocessed to exclude non-land areas and reduce spatial resolution for ease of computation.

### References

[CalFire Fire Perimeter Data](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program/fire-perimeters)

California Department of Forestry and Fire Protection (CAL FIRE), [calfire_all.gdb], [2024-11-17], retrieved from [CAL FIRE data portal.](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program/fire-perimeters)

[Landsat Data](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2) from Microsoft's Planetary Computer Data Catalogue,

- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 4-5 Thematic Mapper Level-2, Collection 2. U.S. Geological Survey. https://doi.org/10.5066/P9IAXOVV
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 7 Enhanced Thematic Mapper Plus Level-2, Collection 2. U.S. Geological Survey. https://doi.org/10.5066/P9C7I13B
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6

Galaz García, Carmen. Assignment4 – EDS 220 - Working with Environmental Datasets. (n.d.). https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/assignment2.html

Galaz García, Carmen. Assignment4 – EDS 220 - Working with Environmental Datasets. (n.d.). https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/assignment4.html


### Repository organization

```
 thomas-fire-analysis
│   README.md
|   thomas-fire-analysis.ipynb
|   thomas-fire-aqi.ipynb
│   thomas-fire-false-color.ipynb
|   .gitignore
│
└───data
|   |   landsat8-2018-01-26-sb-simplified.nc
|   |   thomas_2017.geojson
|
└───images
    |   thomas-fire-ojai.jpeg
```
