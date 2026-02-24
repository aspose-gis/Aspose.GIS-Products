---
title: Shapefile Viewer
url: /vi/viewer/shp/
weight: 10
---

## Overview ##

The Shapefile Viewer is a web application that allows users to view and interact with shapefiles directly in their browser. It provides a user-friendly interface for exploring geospatial data without the need for desktop GIS software.

## Features ##

*   **Interactive Map:** Pan, zoom, and identify features on an interactive map.
*   **Attribute Table:** View and sort feature attributes in a table format.
*   **Feature Styling:** Customize the appearance of features based on attribute values.
*   **Data Filtering:** Filter features based on attribute criteria.
*   **Metadata Display:** Access metadata information about the shapefile.

## Usage ##

1.  **Load Shapefile:** Drag and drop a shapefile (``.shp``) onto the viewer or use the "Load" button to select it from your computer.
2.  **Explore Data:** Use the map controls to navigate and zoom into areas of interest. Click on features to view their attributes in the attribute table.
3.  **Customize Appearance:** Adjust feature styles (color, size, transparency) using the styling options.
4.  **Filter Features:** Apply filters to display only features that meet specific criteria.

## Technical Details ##

*   **Supported Shapefile Versions:** The viewer supports standard shapefile versions as defined by Esri.
*   **Coordinate Reference System (CRS):** The viewer automatically detects the CRS of the shapefile.
*   **Data Format:** Shapefiles are a popular geospatial data format used to store vector data such as points, lines, and polygons.

## Troubleshooting ##

*   **Shapefile Not Loading:** Ensure that all necessary files for the shapefile (``.shp``, ``.shx``, ``.dbf``, etc.) are present in the same directory.
*   **Map Displaying Incorrectly:** Verify that the CRS is correctly detected. If not, manually specify the CRS.
*   **Performance Issues:** Large shapefiles may take time to load and render. Try filtering data or simplifying geometries to improve performance.

## Future Enhancements ##

*   **Support for other geospatial formats:** Add support for GeoJSON, KML, and other common formats.
*   **Advanced Styling Options:** Provide more granular control over feature styling.
*   **Spatial Analysis Tools:** Integrate basic spatial analysis tools such as buffering and overlaying.
*   **Online Shapefile Repository:** Allow users to upload and share shapefiles with others.

## Contact ##

For questions or feedback, please contact the development team at [email protected]

---
