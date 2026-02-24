---
title: Shapefiles
linkTitle: Pliki kształtu
weight: 10
url: /pl/net/viewer/shp/
---

Shapefiles are a popular geospatial file format used to store vector data. They are commonly used in GIS software for displaying and analyzing geographic information.

## What is a Shapefile?

A shapefile (.shp) is not just one file, but a collection of files that work together to store spatial data. These files typically include:

*   **.shp:** The main file containing the geometry (points, lines, polygons).
*   **.shx:** An index file that speeds up access to the geometric data.
*   **.dbf:** A dBASE table containing attribute information associated with each feature.
*   **.prj:** A projection file defining the coordinate system of the data.

## Supported Data Types

Shapefiles can store various types of geographic features, including:

*   **Points:** Representing single locations (e.g., cities, wells).
*   **Lines:** Representing linear features (e.g., roads, rivers).
*   **Polygons:** Representing areas (e.g., lakes, countries).
*   **Multi-points, Multi-lines, and Multi-polygons:**  Representing collections of points, lines, or polygons respectively.

## Creating Shapefiles

Shapefiles are typically created using GIS software such as:

*   QGIS (open source)
*   ArcGIS (commercial)
*   GeoDa (open source)

These programs provide tools for digitizing geographic features and storing them in shapefile format.

## Reading Shapefiles

The NetCDF Viewer supports reading shapefiles. The viewer will display the geometry of the features along with any associated attribute data.

### Displaying Attributes

Attribute data from the .dbf file can be displayed in a table within the viewer. This allows users to examine and analyze the characteristics of each geographic feature.

## Limitations

*   Shapefiles are not designed for very large datasets due to limitations in the dBASE format used for attribute storage.
*   Shapefiles do not inherently support topology, which means that relationships between features (e.g., adjacency) are not explicitly stored.
*   The .dbf file uses a fixed-length field definition, which can limit the types and sizes of attributes that can be stored.

