---
title: Convert to Georeferenced Coordinates
url: /it/net/coordinates/convert-to-georef/
linkTitle: Converti in coordinate georeferenziate
weight: 10
---

## Converting Coordinates to Georeferenced Format

This guide explains how to convert coordinates from various formats into a georeferenced format.  Georeferencing associates geographic features with specific locations on the Earth, typically using latitude and longitude.

### Coordinate Formats

Several coordinate formats exist, each representing location data differently:

*   **Latitude/Longitude (Lat/Lon):** The most common format, expressed in degrees.
*   **UTM (Universal Transverse Mercator):** A projected coordinate system that divides the Earth into zones.
*   **State Plane Coordinates:**  A projected coordinate system used within specific U.S. states.
*   **MGRS (Military Grid Reference System):** A grid-based system covering the entire globe.

### Conversion Process

The conversion process generally involves these steps:

1.  **Identify the Input Coordinate Format:** Determine the format of your existing coordinates.
2.  **Select a Georeferenced Output Format:** Choose a suitable georeferenced format (Lat/Lon is often preferred).
3.  **Use Conversion Tools:** Employ software or online tools to perform the conversion.

### Software and Online Resources

Several options are available for coordinate conversions:

*   **GIS Software:** Programs like QGIS, ArcGIS, and Global Mapper offer comprehensive coordinate transformation capabilities.
*   **Online Converters:** Numerous websites provide free coordinate conversion services (search for "coordinate converter").
*   **Programming Libraries:**  Libraries in languages like Python (e.g., `pyproj`) allow programmatic conversions.

### Example: Converting UTM to Latitude/Longitude using QGIS

1.  Open QGIS.
2.  Add a layer containing your UTM coordinates (e.g., shapefile, CSV).
3.  Use the "Project > Transform Layers" tool.
4.  Select "UTM" as the source coordinate reference system (CRS).
5.  Choose "WGS 84" (EPSG:4326) as the destination CRS (this is a common Lat/Lon format).
6.  Click "Apply".

### Considerations

*   **Datum:** Ensure that both input and output coordinates use compatible datums (e.g., WGS 84, NAD27, NAD83). Datum transformations are crucial for accurate results.
*   **Zone:** For UTM conversions, specify the correct zone number.
*   **Accuracy:** Coordinate conversion introduces potential errors.  Understand the limitations of your tools and data.

### Further Reading

*   [Coordinate Systems and Datums](https://en.wikipedia.org/wiki/Coordinate_system)
*   [UTM Coordinates](https://en.wikipedia.org/wiki/Universal_Transverse_Mercator_coordinate_system)
---
