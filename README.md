# Site Selection Analysis for Automated Speed Enforcement Expansion in Toronto

## Overview

This project focuses on identifying suitable locations for the expansion of Automated Speed Enforcement (ASE) systems within the City of Toronto. The analysis aims to improve road safety by reducing speeding incidents, thereby enhancing overall traffic safety.

## Purpose

The goal of this project is to perform a site suitability analysis to identify optimal road segments for the deployment of new ASE devices. This is in response to the City of Toronto's initiative to improve road safety and reduce traffic-related incidents. By strategically selecting locations for ASE expansion, the project aims to decrease speeding violations and enhance safety in high-risk areas, particularly those near schools and community safety zones.

## Data Collection

The datasets used in this project were obtained from reliable sources, including the Toronto Open Data Portal and the Ontario GeoHub. Key datasets include:

1. **Automated Speed Enforcement Locations:** Provides the locations of current ASE devices within Toronto.
2. **Police Annual Statistical Report - Traffic Collisions:** Contains data on traffic collisions in Toronto from 2014 to 2023.
3. **Ontario Road Network (ORN) Segment With Address:** Details road segments in Ontario, focusing on those within Toronto.
4. **Regional Municipal Boundary:** Outlines the boundaries of Toronto, aiding in clipping and focusing the analysis.
5. **Community Safety Zone Watch Your Speed Program - Locations:** Shows locations of radar devices that monitor vehicle speeds for warning purposes.

## Methodology

### Data Preparation

1. **Coordinate Transformation:** All datasets were transformed from the default WGS 1984 coordinate system to EPSG: 26917 (NAD83 / UTM zone 17N) to ensure accurate spatial analysis.
2. **Database Setup:** A PostgreSQL database with PostGIS extension was used to store and query spatial data. Shapefiles were loaded into the database using `shp2pgsql` commands, which facilitated spatial queries.

### Analysis

The analysis involved identifying road segments within Toronto that would benefit the most from new ASE devices. Key steps included:

1. Selecting road segments intersecting with high-incident areas using spatial joins with traffic collision data.
2. Filtering road segments that are in close proximity to community safety zones.
3. Prioritizing segments without existing ASE devices but with a high number of recent (2022-2023) traffic collisions.

### Key Findings

- **Top Priority Sites for ASE Expansion:**
  1. **Jameson Avenue:** Highest collision count, proximity to an elementary school and rehabilitation center.
  2. **Kipling Avenue:** Major road junction with high traffic volume, especially near Albion Mall.
  3. **Gateway Boulevard:** Close to three schools and numerous community zones, making it a critical area for enforcement.

## Data Visualization

The project included the creation of detailed maps using QGIS. The maps highlighted current ASE locations, traffic collision hotspots, and proposed expansion areas. Insets provided a closer look at the selected road segments, emphasizing their importance for enhanced road safety.

## Conclusion

The strategic placement of new ASE devices on Jameson Avenue, Kipling Avenue, and Gateway Boulevard is expected to significantly enhance road safety in Toronto. This project demonstrates the value of spatial analysis in urban planning and traffic management, aiming to create a safer environment for all road users.

## Data Sources

- **Automated Speed Enforcement Locations** - [Open Toronto](https://open.toronto.ca/dataset/automated-speed-enforcement-locations/)
- **Traffic Collisions Data** - [Open Toronto](https://open.toronto.ca/dataset/police-annual-statistical-report-traffic-collisions/)
- **Ontario Road Network** - [Ontario GeoHub](https://geohub.lio.gov.on.ca/datasets/923cb3294384488e8a4ffbeb3b8f6cb2/explore?location=46.297972%2C-82.800492%2C5.00)
- **Toronto Municipal Boundary** - [Open Toronto](https://open.toronto.ca/dataset/regional-municipal-boundary/)
- **Community Safety Zone Radar Locations** - [Open Toronto](https://open.toronto.ca/dataset/school-safety-zone-watch-your-speed-program-locations/)

## References

- Essa Township. (n.d.). ASE Camera Locations. [Link](https://www.essatownship.on.ca/living-in-essa/automated-speed-enforcement/ase-camera-locations/)
- City of Mississauga. (2023). Automated Speed Enforcement (ASE). [Link](https://www.mississauga.ca/services-and-programs/transportation-and-streets/road-safety/automated-speed-enforcement/)
- City of Toronto. (2023). Automated Speed Enforcement. [Link](https://www.toronto.ca/services-payments/streets-parking-transportation/automated-speed-enforcement/)
