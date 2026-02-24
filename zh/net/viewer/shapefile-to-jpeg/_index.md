---
title: Shapefile to JPEG Conversion
date: 2024-01-18T16:37:59+08:00
draft: false
url: /zh/viewer/shapefile-to-jpeg/
linkTitle: Shapefile 转 JPEG 转换
weight: 10

---

## Overview ##
<div class="section">
This guide explains how to convert a shapefile (.shp) to a JPEG image. This process is useful for visualizing spatial data and creating maps.
</div>

## Prerequisites ##
<div class="section">
*   **GDAL/OGR:** A powerful geospatial data abstraction library.  Make sure it's installed on your system. You can download it from [https://gdal.org/](https://gdal.org/).
*   **Command Line Interface (CLI):** Familiarity with using the command line is required.
</div>

## Conversion Process ##
<div class="section">
The core command uses `ogr2jpeg`, a utility that comes with GDAL.  Here's the general syntax:

```bash
ogr2jpeg -if zoom=10 -of JPEG shapefile.shp output.jpg
```

Let's break down this command:

*   `ogr2jpeg`: The command itself.
*   `-if zoom=10`: Sets the initial zoom level for the map. Adjust this value to control the scale of the resulting image.  Higher values mean more zoomed in.
*   `-of JPEG`: Specifies the output format as JPEG.
*   `shapefile.shp`: The path to your shapefile. Replace with the actual filename.
*   `output.jpg`: The desired name for the output JPEG file.

</div>

## Advanced Options ##
<div class="section">
`ogr2jpeg` offers many options for customization. Here are a few useful ones:

*   **Setting the Output Size:** Use `-size widthxheight` to specify the dimensions of the output image in pixels (e.g., `-size 800x600`).
*   **Controlling Color and Background:**  Use `-dpi dpi_value` to set the resolution of the output image in dots per inch. You can also use options like `-bg color` to change the background color.
*   **Defining Projection:** If your shapefile has a projection defined, `ogr2jpeg` will automatically use it. However, you can override this with `-t_srs epsg:4326` (for example) to force a specific spatial reference system.
*   **Layer Selection:**  If the shapefile contains multiple layers, you can specify which layer to convert using `-layer layer_number`.

</div>

## Example ##
<div class="section">
Let's say you have a shapefile named `cities.shp` and want to create a JPEG image with a zoom level of 12, an output size of 1024x768 pixels, and a white background.  The command would be:

```bash
ogr2jpeg -if zoom=12 -of JPEG -size 1024x768 -bg White cities.shp city_map.jpg
```

</div>

## Troubleshooting ##
<div class="section">
*   **"ogr2jpeg not found":**  Make sure GDAL is installed correctly and that the `ogr2jpeg` executable is in your system's PATH environment variable.
*   **Incorrect Projection:** If the map appears distorted, double-check the shapefile's projection and consider using the `-t_srs` option to specify a known coordinate reference system.
*   **Missing Shapefile:** Verify that the path to the shapefile is correct.

</div>

## Conclusion ##
<div class="section">
Converting shapefiles to JPEGs with `ogr2jpeg` is a straightforward process, allowing you to easily visualize and share your geospatial data. Experiment with the various options to achieve the desired results.
</div>
---
