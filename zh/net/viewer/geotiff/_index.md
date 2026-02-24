---
title: GeoTIFF Viewer
url: /zh/viewer/geotiff/
weight: 10
previous: /zh/viewer/
next: /zh/viewer/raster-tile-source/
---

## Overview

The GeoTIFF viewer allows you to visualize and interact with GeoTIFF files. It provides features for zooming, panning, measuring distances, and displaying metadata.

## Features

*   **Zooming and Panning:** Easily navigate through the GeoTIFF image using mouse wheel or touch gestures.
*   **Measurement Tools:** Measure distances and areas on the map.
*   **Metadata Display:** View information about the GeoTIFF file, such as spatial reference, data type, and pixel size.
*   **Customizable Color Palettes:** Adjust the color scheme to enhance visualization.
*   **Support for Various GeoTIFF Formats:** Compatible with a wide range of GeoTIFF formats, including those with multiple bands and overviews.

## Usage

1.  **Load GeoTIFF File:** Drag and drop a GeoTIFF file onto the viewer or use the "Open" button to select a file from your computer.
2.  **Navigate the Image:** Use the mouse wheel or touch gestures to zoom in and out, and click and drag to pan across the image.
3.  **Measure Distances/Areas:** Click the measurement tool icon and then click on the map to define points for measuring distances or areas.
4.  **View Metadata:** Click the metadata button to display information about the GeoTIFF file.

## Code Example

```java
// This is a sample code snippet demonstrating how to load a GeoTIFF image.
GeoTiffReader reader = new GeoTiffReader(new File("path/to/your/geotiff/file.tif"));
Raster raster = reader.read();
```

## Troubleshooting

*   **File Not Supported:** Ensure that the file is a valid GeoTIFF format.
*   **Performance Issues:** Large GeoTIFF files may require more processing power. Try reducing the image resolution or using an overview level.
*   **Display Errors:** Check for any errors in the metadata or data structure of the GeoTIFF file.

## Further Reading

*   [GeoTIFF Specification](https://www.awadagroup.com/geo-tiff/)
*   [GDAL/OGR](https://gdal.org/)
