---
title: Shapefiles
url: /ru/viewer/shp/
weight: 10
---

## What are Shapefiles?
Shapefiles are a popular file format for storing geospatial vector data. They represent geographic features such as points, lines, and polygons. A shapefile is not just one file, but a collection of files that work together to store the spatial data and associated attributes.

## Shapefile Components
A shapefile typically consists of the following files:

*   **.shp**: This file stores the geometry (shape) of the geographic features.
*   **.shx**: This is an index file that links the geometric data in the .shp file to the attribute data in the .dbf file.
*   **.dbf**: This file stores the attribute data for each geographic feature, in a database-like format.
*   **.prj**: This file contains information about the coordinate system used by the shapefile.

## Supported Shapefile Versions
Our viewer supports shapefiles created with versions 0.9 and later.

## Limitations
*   Shapefiles do not support topologies.
*   The maximum length for attribute names is 10 characters.
*   The maximum size of a shapefile is limited to 2GB.

## Viewing Shapefiles in the Viewer
To view a shapefile, simply drag and drop the .shp file onto the viewer or use the "Open" button to select the shapefile. The viewer will automatically load and display the data.

## Attribute Table
The viewer displays an attribute table that shows the attributes for each geographic feature. You can sort the attribute table by clicking on the column headers.

## Zooming and Panning
You can zoom in and out of the map using the mouse wheel or by dragging the map with the left mouse button.

## Identifying Features
To identify a geographic feature, click on it. A popup window will display the attributes for that feature.

## Shapefile Metadata
The viewer displays metadata about the shapefile, such as the number of features, the extent of the data, and the coordinate system.

## Troubleshooting
If you encounter any problems viewing a shapefile, please check the following:

*   Make sure that all the required files (.shp, .shx, .dbf, .prj) are in the same directory.
*   Make sure that the shapefile is not corrupted.
*   Make sure that the coordinate system is supported by the viewer.
---
