# Data Files Overview

This repository contains various geospatial datasets and related files for traffic enforcement, stationary sign locations, and municipal boundaries. The files are mainly provided in shapefile format, accompanied by additional metadata files.

## Automated Speed Enforcement Locations

These files represent the locations where automated speed enforcement is in effect.

- **Automated Speed Enforcement Locations - 4326.cpg**: Encoding information for the shapefile.
- **Automated Speed Enforcement Locations - 4326.dbf**: Database file containing attribute data for each shape.
- **Automated Speed Enforcement Locations - 4326.prj**: Projection information for the shapefile, specifying the coordinate reference system.
- **Automated Speed Enforcement Locations - 4326.shp**: The shapefile format that stores geometric information.
- **Automated Speed Enforcement Locations - 4326.shx**: Index file that speeds up access to geometric data.
- **Automated Speed Enforcement Locations fields.csv**: A CSV file listing the fields and descriptions used in the shapefile.

## Stationary Sign Locations

These files contain data about stationary sign locations, likely used for traffic management or informational purposes.

- **Stationary Sign locations - 4326.cpg**: Encoding information for the shapefile.
- **Stationary Sign locations - 4326.dbf**: Database file containing attribute data for each shape.
- **Stationary Sign locations - 4326.prj**: Projection information for the shapefile, specifying the coordinate reference system.
- **Stationary Sign locations - 4326.shp**: The shapefile format that stores geometric information.
- **Stationary Sign locations - 4326.shx**: Index file that speeds up access to geometric data.
- **Stationary Sign locations fields.csv**: A CSV file listing the fields and descriptions used in the shapefile.

## Traffic Collisions

This file provides encoding information for traffic collision data, which may be in a different format, but the `.cpg` file suggests it could be related to a shapefile dataset.

- **Traffic Collisions - 4326.cpg**: Encoding information for the associated shapefile or geospatial data.

## Ontario Road Network

This file provides encoding information for the Ontario Road Network data.

- **Ontario_Road_Network_(ORN)_Segment_With_Address.cpg**: Encoding information for the Ontario Road Network segment shapefile with address information.

## Municipal Boundaries Data

These files provide information about municipal boundaries in a specific projection format.

- **citygcs.regional_mun_wgs84_metadata.pdf**: Metadata document in PDF format, containing information about the dataset.
- **citygcs_regional_mun_wgs84.dbf**: Database file containing attribute data for each shape.
- **citygcs_regional_mun_wgs84.prj**: Projection information for the shapefile, specifying the coordinate reference system.
- **citygcs_regional_mun_wgs84.sbn**: Spatial index file to improve performance with large datasets.
- **citygcs_regional_mun_wgs84.sbx**: Additional spatial index information.
- **citygcs_regional_mun_wgs84.shp**: The shapefile format that stores geometric information.
- **citygcs_regional_mun_wgs84.shp.xml**: Metadata file in XML format.
- **citygcs_regional_mun_wgs84.shx**: Index file that speeds up access to geometric data.

## Additional Documentation

- **Regional_municipality readme file.txt**: A text file containing additional information or instructions related to the regional municipality dataset.

## Notes

- The coordinate reference system (CRS) used for these datasets is typically WGS 84 (EPSG:4326), which is a standard for representing geospatial data.
- The `.cpg` files specify the character encoding used in the `.dbf` files.
- For more detailed information about the fields and their definitions, refer to the respective `.csv` files provided with the datasets.

