---
title: Shapefile to SVG Conversion
url: /zh/shapefile-to-svg/
weight: 10
layout: ""
---

## Converting Shapefiles to Scalable Vector Graphics (SVG)

This guide explains how to convert shapefiles (.shp) into SVG format.  SVGs are useful for web mapping and other applications where vector data needs to be displayed in a scalable and interactive way.

### Why Convert to SVG?

*   **Scalability:** SVGs are vector-based, meaning they can be scaled without losing quality.
*   **Interactivity:** SVGs can be styled with CSS and JavaScript for interactive maps.
*   **Small File Size:**  SVGs often result in smaller file sizes compared to raster formats like PNG or JPEG.

### Methods for Conversion

Several tools and libraries are available for converting shapefiles to SVG:

1.  **QGIS (Free and Open Source):** QGIS is a powerful Geographic Information System that can easily convert shapefiles to SVG.
    *   Open the shapefile in QGIS.
    *   Go to "Layer" -> "Export" -> "Save Features As...".
    *   Choose "SVG" as the format.
    *   Adjust settings as needed (e.g., simplification, attribute export).
    *   Click "OK" to save the SVG file.

2.  **Mapshaper.js (Online Tool):** Mapshaper is a web-based tool for simplifying and converting geospatial data.
    *   Upload your shapefile to [https://mapshaper.org/](https://mapshaper.org/).
    *   Adjust simplification settings as needed.  Higher simplification reduces file size but can also reduce accuracy.
    *   Choose "SVG" as the output format.
    *   Click "Simplify & Export".

3.  **ogr2ogr (Command-Line Tool):** ogr2ogr is a command-line utility that's part of the GDAL/OGR library. It’s very flexible but requires some technical knowledge.
    ```bash
    ogr2ogr -f "SVG" output.svg input.shp
    ```
    *   Replace `input.shp` with the name of your shapefile.
    *   Replace `output.svg` with the desired name for your SVG file.

4.  **Python Libraries (e.g., Fiona, Shapely):** You can use Python libraries like Fiona and Shapely to programmatically convert shapefiles to SVG. This gives you more control over the conversion process.
    ```python
    import fiona
    from shapely.geometry import shape

    with fiona.open('input.shp', 'r') as source:
        with fiona.open('output.svg', 'w', driver='ogrsvg', schema=source.schema) as sink:
            for feature in source:
                geom = shape(feature['geometry'])
                sink.write({
                    'geometry': geom,
                    'properties': feature['properties']
                })
    ```
    *   Install the necessary libraries: `pip install fiona shapely`

### Considerations

*   **Simplification:**  Shapefiles can contain a large number of vertices, resulting in very large SVG files. Simplification reduces the number of vertices while preserving the overall shape. Mapshaper and QGIS provide simplification options.
*   **Attribute Export:** Decide which attributes from your shapefile you want to include in the SVG file. Some tools allow you to specify which attributes to export.
*   **Coordinate Reference System (CRS):** Ensure that both your shapefile and the target SVG have the same CRS, or reproject the shapefile before conversion.  Incorrect CRSs can lead to inaccurate map displays.

### Troubleshooting

*   **Large File Sizes:** If the resulting SVG file is too large, try increasing the simplification level.
*   **Missing Attributes:** Double-check that you've configured the tool correctly to export the desired attributes.
*   **Display Issues:** Verify that the CRS is correct and that the SVG viewer supports the features used in the SVG (e.g., gradients, complex styling).

---
