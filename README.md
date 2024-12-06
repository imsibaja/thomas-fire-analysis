# Thomas Fire Scarring 2017

![thomas fire image](images/thomas-fire-ojai.jpeg)
Image credits: [spookysnoopy via Imgur](https://imgur.com/gallery/thomas-fire-ojai-california-OJdjw)


## About
This repository contains notebooks `hwk4-task2-fire-perimeter-MORRIS-SIBAJA.ipynb` and `hwk4-task2-false-color-MORRIS-SIBAJA.ipynb` whose goal are to analyze the fire scarring of the 2017 Thomas Fire in Santa Barbara and Ventura Counties.

After examining geospatial and tabular datasets, we created a border of the Thomas Fire boundary and overlayed it over a false color map of the fire scarring.
This completed map is located at the bottom of the `hwk4-task2-false-color-MORRIS-SIBAJA.ipynb` notebook.

### Highlights

- Data wrangling and exploration with `pandas` and `rioxarray`
- Geospatial data wrangling with `geopandas` and `rioxarray`
- Merging of tabular and vector data
- Creating and customizing a false color map using `matplotlib.pyplot`

### Data

#### U.S. Air Quality Index (AQI)

The U.S. Air Quality Index (AQI), developed by the EPA, communicates outdoor air quality and associated health risks through six color-coded categories, ranging from “Good” (AQI ≤ 50) to “Hazardous” (AQI > 300). AQI values up to 100 indicate satisfactory air quality, aligned with national health standards, while values above 100 signal unhealthy conditions—initially for sensitive groups and eventually for all as pollution levels rise. The color-coded system enables quick identification of air quality concerns in communities.

#### Landset 8 Satellite Collection

This dataset consists of simplified bands (red, green, blue, near-infrared, and shortwave infrared) from Landsat Collection 2 Level-2 surface reflectance data, which was atmospherically corrected and captured by NASA’s Landsat 8 satellite. It was sourced from the Microsoft Planetary Computer data catalog and preprocessed to exclude non-land areas and reduce spatial resolution for ease of computation.

### References

[CalFire Fire Perimeter Data](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program/fire-perimeters)

California Department of Forestry and Fire Protection (CAL FIRE), [calfire_all.gdb], [2024-11-17], retrieved from [CAL FIRE data portal.](https://www.fire.ca.gov/what-we-do/fire-resource-assessment-program/fire-perimeters)

[Landsat Data](https://planetarycomputer.microsoft.com/dataset/landsat-c2-l2) from Microsoft's Planetary Computer Data Catalogue,

- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 4-5 Thematic Mapper Level-2, Collection 2. U.S. Geological Survey. https://doi.org/10.5066/P9IAXOVV
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 7 Enhanced Thematic Mapper Plus Level-2, Collection 2. U.S. Geological Survey. https://doi.org/10.5066/P9C7I13B
- Earth Resources Observation and Science (EROS) Center. (2020). Landsat 8-9 Operational Land Imager / Thermal Infrared Sensor Level-2, Collection 2. U.S. Geological Survey. https://doi.org/10.5066/P9OGBGM6

Galaz García, Carmen. Assignment4 – EDS 220 - Working with Environmental Datasets. (n.d.). https://meds-eds-220.github.io/MEDS-eds-220-course/assignments/assignment4.html

M. M. Bennett, J. K. Chen, L. F. Alvarez León, and C. J. Gleason, “The politics of pixels: A review and agenda for critical remote sensing,” Progress in Human Geography, vol. 46, no. 3, pp. 729–752, Jun. 2022, doi: 10.1177/03091325221074691. Available: https://journals.sagepub.com/doi/10.1177/03091325221074691. [Accessed: Nov. 23, 2024]

### Repository organization

```
 eds220-hwk4
│   README.md
|   hwk4-task1-reflection-MORRIS-SIBAJA.md
|   hwk4-task2-fire-perimeter-MORRIS-SIBAJA.ipynb
│   hwk4-task2-false-color-MORRIS-SIBAJA.ipynb
|   .gitignore
│
└───data
|   |   landsat8-2018-01-26-sb-simplified.nc
|   |   thomas_2017.geojson
|       California_Fire_Perimeters_4280901625349411772.geojson available from link above
|
└───images
    |   thomas-fire-ojai.jpeg
```
