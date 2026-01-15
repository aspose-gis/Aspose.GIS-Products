---
title: GeoJSON to SVG Conversion
linkTitle: Konversi GeoJSON ke SVG
weight: 10
url: /id/geojson-to-svg/
description: Learn how to convert GeoJSON data into SVG format for interactive mapping applications. Pelajari cara mengonversi data GeoJSON menjadi format SVG untuk aplikasi pemetaan interaktif.
aliases: [geojson2svg, geojson svg]
---

## Introduction

GeoJSON is a standard format for encoding geographic data. SVG (Scalable Vector Graphics) is an XML-based vector image format. Converting GeoJSON to SVG allows you to display and interact with geographic data in web browsers and other applications.

## Prerequisites

*   Basic understanding of GeoJSON and SVG formats.
    Pemahaman dasar tentang format GeoJSON dan SVG.
*   A GeoJSON file containing the geographic data you want to convert.
    Berkas GeoJSON yang berisi data geografis yang ingin Anda konversi.
*   Programming environment with necessary libraries (e.g., Python with `geopandas` and `svgwrite`).
    Lingkungan pemrograman dengan pustaka yang diperlukan (misalnya, Python dengan `geopandas` dan `svgwrite`).

## Conversion Methods

There are several ways to convert GeoJSON to SVG:

### 1. Using Python with Geopandas and Svgwrite

This method uses the `geopandas` library for reading GeoJSON data and the `svgwrite` library for creating SVG files.

```python
import geopandas as gpd
import svgwrite

# Load GeoJSON file
gdf = gpd.read_file("your_geojson_file.geojson")

# Create an SVG drawing
dwg = svgwrite.Drawing('output.svg', profile='tiny')

# Iterate over features in the GeoDataFrame and draw them on the SVG canvas
for _, feature in gdf.iterrows():
    geometry = feature['geometry']
    if geometry.geom_type == 'Polygon':
        polygon = dwg.polygon(points=list(geometry.exterior.coords), fill='blue', stroke='black')
        dwg.add(polygon)
    elif geometry.geom_type == 'LineString':
        line = dwg.line(points=list(geometry.coords), stroke='red', stroke_width=2)
        dwg.add(line)
    elif geometry.geom_type == 'Point':
        circle = dwg.circle(center=geometry.coords[0], r=5, fill='green', stroke='black')
        dwg.add(circle)

# Save the SVG file
dwg.save()
```

*Replace `"your_geojson_file.geojson"` with the actual path to your GeoJSON file.*

### 2. Using Online Converters

Several online tools can convert GeoJSON to SVG without requiring any programming knowledge. Some popular options include:

*   [Mapshaper](https://mapshaper.org/)
*   [GeoJSON.io](https://geojson.io/)

These converters typically provide a user-friendly interface for uploading your GeoJSON file and customizing the output SVG.

### 3. Using Command-Line Tools

Tools like `ogr2ogr` (part of the GDAL library) can also be used to convert GeoJSON to SVG from the command line.

```bash
ogr2ogr -f "SVG" output.svg input.geojson
```

## Customization Options

When converting GeoJSON to SVG, you have several options for customizing the appearance of the resulting image:

*   **Colors:** Change the fill and stroke colors of polygons, lines, and points.
    Warna: Ubah warna isian dan garis tepi poligon, garis, dan titik.
*   **Stroke Width:** Adjust the thickness of line features.
    Lebar Garis Tepi: Sesuaikan ketebalan fitur garis.
*   **Scaling:** Scale the SVG image to fit a specific area or resolution.
    Penskalaan: Penskalaan gambar SVG agar sesuai dengan area atau resolusi tertentu.
*   **Simplification:** Simplify complex geometries to reduce file size and improve rendering performance.
    Penyederhanaan: Sederhanakan geometri yang kompleks untuk mengurangi ukuran berkas dan meningkatkan kinerja render.

## Conclusion

Converting GeoJSON to SVG is a powerful technique for visualizing geographic data in web applications and other environments. By using the methods described above, you can easily convert your GeoJSON files into interactive SVG maps.

## Resources

*   [GeoJSON Specification](https://geojson.org/rfc/)
    Spesifikasi GeoJSON
*   [SVG Specification](https://www.w3.org/TR/svg/)
    Spesifikasi SVG
*   [geopandas Documentation](https://geopandas.org/en/stable/)
    Dokumentasi geopandas
*   [svgwrite Documentation](http://svgwrite.readthedocs.io/en/latest/)
    Dokumentasi svgwrite

---
