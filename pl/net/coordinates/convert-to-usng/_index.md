---
title: Convert to USNG
url: /pl/net/coordinates/convert-to-usng/
linkTitle: Konwertuj do USNG
weight: 10
---

## Convert Coordinates to USNG

The Universal Transverse Mercator (UTM) coordinate system is divided into zones, each spanning 6 degrees of longitude. This can make it difficult to share coordinates across different zones or regions. The US National Grid (USNG) was developed to address this issue by providing a nationwide coordinate system that simplifies communication and data sharing.

### What is USNG?

USNG is a grid-based coordinate system used in the United States. It's derived from the UTM system but provides a more user-friendly format for localizing positions within the country. USNG coordinates are represented as a string of characters, including:

*   **Zone Designator:** A two-letter code representing the zone (e.g., "12N").
*   **Easting:** The easting value in 100-meter increments.
*   **Northing:** The northing value in 100-meter increments.

### Why Convert to USNG?

*   **Simplified Communication:** USNG provides a standardized way to share locations, eliminating the need to specify UTM zones.
*   **Improved Accuracy:** USNG coordinates are more precise than latitude/longitude values for local applications.
*   **Data Integration:** USNG facilitates the integration of geospatial data from different sources.

### How to Convert Coordinates to USNG

The conversion process involves several steps:

1.  **Determine the UTM Zone:** Identify the UTM zone in which your coordinates are located.
2.  **Convert to Easting and Northing:** Transform your latitude/longitude values into easting and northing values based on the identified UTM zone.
3.  **Calculate USNG Values:** Apply formulas to convert the easting and northing values into USNG format.

### Tools for Conversion

Several tools are available to assist with coordinate conversion:

*   **Online Converters:** Numerous websites offer free online converters that can perform the calculations automatically.
*   **GIS Software:** Geographic Information System (GIS) software packages, such as QGIS and ArcGIS, provide built-in functionality for coordinate transformations.
*   **Programming Libraries:** Programming libraries in languages like Python and JavaScript allow you to implement custom conversion routines.

### Example Conversion

Let's say we have the latitude/longitude coordinates 34.0522° N, 118.2437° W.  The UTM zone for this location is 11S. Using a coordinate converter, we can obtain the following easting and northing values:

*   Easting: 349689 m
*   Northing: 3765077 m

Applying the USNG conversion formulas, we get the USNG coordinate:

12S 349689 3765077

### Considerations

*   **Datum:** Ensure that your coordinates are referenced to the same datum (e.g., WGS84) as the converter you're using.
*   **Accuracy:** Coordinate conversion introduces some level of error. Be aware of the potential impact on accuracy for critical applications.
*   **Regional Variations:** USNG is primarily used in the United States. For international locations, consider alternative coordinate systems.

### Resources

*   [US National Grid (USNG)](https://www.usng.mil/)
*   [Coordinate Conversion Tools](https://www.gpsvisualizer.com/convert.jsp)
---
