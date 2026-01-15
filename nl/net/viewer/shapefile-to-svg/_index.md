---
title: Shapefile to SVG Conversion
url: /nl/shapefile-to-svg/
linkTitle: Shapefile naar SVG conversie
weight: 10

---

## Converting Shapefiles to Scalable Vector Graphics (SVG)

This guide explains how to convert shapefiles (.shp) into scalable vector graphics (.svg) format.  SVGs are ideal for web display due to their resolution independence and small file sizes.

### Why Convert?

*   **Web Compatibility:** SVGs render perfectly on all devices and browsers without quality loss.
*   **Small File Size:** Compared to raster images (like PNG or JPG), SVGs generally have smaller file sizes, leading to faster loading times.
*   **Scalability:**  SVGs can be scaled infinitely without losing clarity.
*   **Interactivity:** SVGs support interactivity through CSS and JavaScript.

### Methods for Conversion

Several tools and libraries are available for converting shapefiles to SVG:

1.  **QGIS (Recommended):** QGIS is a free and open-source Geographic Information System (GIS) software that provides robust shapefile handling capabilities, including export to SVG.
2.  **Mapshaper:** Mapshaper is an online tool specifically designed for simplifying and converting geospatial data, including shapefiles to SVG. It's easy to use but has limitations on file size.
3.  **GDAL/OGR:** GDAL (Geospatial Data Abstraction Library) is a powerful command-line utility that can be used with its OGR component to convert between various vector formats, including shapefile and SVG.
4.  **Python Libraries (e.g., Fiona, Shapely):** Python offers libraries like Fiona for reading shapefiles and Shapely for geometric operations, which can be combined to generate SVG output.

### Using QGIS for Conversion

1.  **Installation:** Download and install QGIS from [https://www.qgis.org/](https://www.qgis.org/).
2.  **Import Shapefile:** Open the shapefile in QGIS using "Layer" -> "Add Layer" -> "Add Vector Layer."
3.  **Export to SVG:** Right-click on the layer in the Layers panel and select "Export" -> "Save Features As...". Choose "SVG" as the format. Configure options like simplification tolerance (to reduce file size) and symbology (to preserve styling). Click "OK" to export.

### Using Mapshaper Online

1.  **Access:** Go to [https://mapshaper.org/](https://mapshaper.org/).
2.  **Upload Shapefile:** Drag and drop your shapefile onto the website or use the "Choose File" button.
3.  **Simplify (Optional):** Use the simplification tools to reduce the number of vertices in your geometry, which will decrease file size.
4.  **Convert:** Click the "Simplify & Export" button. Select "SVG" as the output format and configure any desired options.
5.  **Download:** Download the generated SVG file.

### Using GDAL/OGR (Command Line)

```bash
ogr2ogr -f "SVG" output.svg input.shp
```

/* This command converts 'input.shp' to 'output.svg' using the SVG format. */

### Python Example (using Fiona and Shapely)

```python
import fiona
from shapely.geometry import shape
from lxml import etree

# Open the shapefile
shapefile = fiona.open("input.shp", "r")
collection = shapefile.rio.to_polygon()

# Create an SVG tree
svg = etree.Element("svg", {"width": "100%", "height": "100%"})

# Iterate over the features and add them to the SVG
for feature in collection:
    geom = shape(feature['geometry'])
    # ... (Add code here to convert Shapely geometry to SVG path elements)

# Write the SVG tree to a file
tree = etree.ElementTree(svg)
tree.write("output.svg", encoding="utf-8", xml_declaration=True)

shapefile.close()
```

### Considerations

*   **Simplification:**  Reducing the number of vertices in your shapefile can significantly decrease SVG file size, but it may also affect accuracy. Experiment with different simplification tolerances to find a balance between file size and quality.
*   **Symbology:** QGIS allows you to preserve symbology (colors, line widths, etc.) during export. Mapshaper has limited styling options.  Python scripting provides the most control over SVG appearance.
*   **Large Shapefiles:** For very large shapefiles, consider using GDAL/OGR or a Python script for better performance and memory management. Online tools like Mapshaper may have file size limitations.

---
