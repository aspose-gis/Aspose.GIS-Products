---
title: Shapefile to PNG Viewer
url: /pl/viewer/shapefile-to-png/
linkTitle: Przeglądarka Shapefile do PNG
weight: 10

---

## Overview ##

This viewer allows you to convert shapefiles (.shp) into Portable Network Graphics (.png) images. It's a simple tool for visualizing geospatial data without needing complex GIS software.

## Features ##

*   **Simple Interface:** Easy-to-use controls for panning, zooming, and identifying features.
*   **Shapefile Rendering:** Displays shapefiles with associated attributes.
*   **PNG Export:** Converts the current view to a PNG image.
*   **Attribute Display:** Shows attribute data for selected features.

## Usage ##

1.  **Load Shapefile:** Drag and drop your .shp file onto the viewer or use the "Open" button.
2.  **Navigate:** Use the mouse wheel to zoom, click and drag to pan.
3.  **Identify Features:** Click on a feature to view its attributes in the table below.
4.  **Export PNG:** Adjust the view as needed and click the "Export PNG" button.

## Technical Details ##

*   **Frontend:** JavaScript, HTML, CSS
*   **Libraries:** Leaflet (for map rendering), GeoJSON (for shapefile parsing)
*   **Backend:** (Optional) A backend server can be used to handle large shapefiles or perform more complex processing.

## Troubleshooting ##

*   **Shapefile Not Loading:** Ensure the .shp file is valid and all associated files (.dbf, .shx, .prj) are in the same directory.
*   **Rendering Issues:** Some shapefiles may contain invalid geometries that cause rendering problems. Try simplifying the geometry in a GIS software before loading.

## Contact ##

For questions or feedback, please contact [support@example.com](mailto:support@example.com).

---
