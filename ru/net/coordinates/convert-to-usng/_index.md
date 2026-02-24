---
title: Convert to USNG
url: /ru/coordinates/convert-to-usng/
linkTitle: Convert to USNG
weight: 10
---

## Convert Coordinates to USNG

The Universal Transverse Mercator (UTM) coordinate system is divided into zones, each spanning 6 degrees of longitude. This can make it difficult to share coordinates across different zones or regions. The United States National Grid (USNG) was developed to address this issue by providing a nationwide coordinate system that simplifies communication and data sharing.

### What is USNG?

USNG is a grid-based coordinate system used primarily in the United States. It's derived from the UTM system but provides a more user-friendly format for representing locations within the country.  Instead of latitude and longitude, USNG uses a combination of letters and numbers to identify a specific location.

### Why Convert to USNG?

*   **Simplified Communication:** USNG coordinates are easier to understand and communicate than latitude/longitude pairs, especially for those unfamiliar with map projections.
*   **Nationwide Consistency:** Provides a consistent coordinate system across the entire United States, regardless of UTM zone.
*   **Improved Data Sharing:** Facilitates data sharing between different organizations and agencies.
*   **Navigation & Location Services:** Useful for navigation apps, emergency services, and other location-based applications.

### How to Convert Coordinates to USNG

There are several ways to convert coordinates to USNG:

1.  **Online Converters:** Numerous online tools can perform the conversion automatically. Simply enter your latitude and longitude, and the converter will provide the corresponding USNG coordinate.
2.  **GIS Software:** Geographic Information System (GIS) software like QGIS or ArcGIS have built-in functionality to convert between different coordinate systems, including USNG.
3.  **Programming Libraries:** Programming libraries in languages like Python (e.g., `pyproj`) allow you to perform the conversion programmatically.

### Understanding USNG Coordinates

A USNG coordinate consists of two parts:

*   **Zone Designator:** A letter representing a 100 km x 100 km zone within the national grid.
*   **Easting and Northing:** Numbers representing the east-west and north-south position within the zone, respectively, in meters.

For example, `14Q 328976 4592315` represents a location in Zone 14Q, with an Easting of 328976 meters and a Northing of 4592315 meters.

### USNG vs. UTM

| Feature | USNG | UTM |
|---|---|---|
| **Scope** | United States | Worldwide |
| **Coordinate Format** | Zone Designator, Easting, Northing | Zone Number, Easting, Northing |
| **Ease of Use** | More user-friendly | Can be complex for non-experts |
| **Zone Size** | 100 km x 100 km | Varies depending on zone |

### Resources

*   [USNG Documentation](https://www.usng.mil/)
*   [Online USNG Converter](https://www.geodetics.com/usng-converter)

---
