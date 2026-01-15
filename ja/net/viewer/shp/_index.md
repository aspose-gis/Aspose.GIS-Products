---
title: Shapefile Viewer
url: /ja/viewer/shp/
weight: 10
---

## Overview

The Shapefile Viewer is a web application that allows users to view and interact with shapefiles. It provides a user-friendly interface for exploring geospatial data directly in the browser.

## Features

*   **Display Shapefiles:** Load and display shapefiles containing various geometric types (points, lines, polygons).
*   **Interactive Map:** Pan, zoom, and rotate the map to explore different areas of interest.
*   **Attribute Table:** View and sort data associated with each feature in an attribute table.
*   **Feature Information:** Display detailed information about selected features.
*   **Layer Control:** Enable or disable layers to customize the displayed data.
*   **Search Functionality:** Locate specific features based on their attributes.

## Usage

1.  **Load Shapefile:** Use the "Load Shapefile" button to select a shapefile from your local machine.
2.  **Explore Data:** Pan, zoom, and rotate the map to view the data.
3.  **View Attributes:** Click on a feature to display its attributes in the attribute table.
4.  **Customize Display:** Use the layer control to enable or disable layers as needed.

## Technical Details

*   **Frontend:** React, Leaflet
*   **Backend:** Node.js, Express
*   **Data Format:** Shapefile (ESRI)

## Troubleshooting

*   **Shapefile Not Loading:** Ensure that the shapefile is not corrupted and contains valid data.
*   **Performance Issues:** Large shapefiles may take time to load and render. Try simplifying the geometry or using a smaller subset of the data.
*   **Display Errors:** Check for any errors in the browser console and ensure that all required libraries are loaded correctly.

## Support

For questions or issues, please contact us at [support email address].
---
