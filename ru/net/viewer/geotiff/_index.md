---
title: GeoTIFF Viewer
linkTitle: Просмотрщик GeoTIFF
weight: 10
url: /ru/net/viewer/geotiff/
description: View and interact with GeoTIFF files in your browser.
---

## Overview

The GeoTIFF viewer allows you to visualize and interact with GeoTIFF (Geographic TIFF) raster data directly within a web browser. It provides features for zooming, panning, measuring distances, and accessing metadata associated with the GeoTIFF file.

## Features

*   **Zooming and Panning:** Navigate through the image by zooming in and out, and panning across the view.
*   **Metadata Display:** View essential information about the GeoTIFF file, such as spatial reference system, data type, and pixel size.
*   **Measurement Tools:** Measure distances and areas on the map using interactive tools.
*   **Image Information:** Get pixel values at specific locations on the image.
*   **Customizable Appearance:** Adjust color schemes and other visual settings to enhance readability.

## Usage

1.  **Load GeoTIFF File:** Provide a URL or local file path to load a GeoTIFF file into the viewer.
2.  **Interact with the Map:** Use mouse controls (scroll wheel for zoom, click and drag for pan) to explore the image.
3.  **Access Metadata:** Click on the "Metadata" button to view information about the GeoTIFF file.
4.  **Use Measurement Tools:** Select a measurement tool from the toolbar and click on the map to define points or areas.

## Code Example

```javascript
// Initialize the viewer with a URL to a GeoTIFF file
const viewer = new GeoTIFFViewer('geotiff-container', '/java/');

viewer.on('ready', () => {
    console.log('GeoTIFF Viewer is ready.');
});

viewer.on('error', (error) => {
    console.error('Error loading GeoTIFF:', error);
});
```

## Troubleshooting

*   **File Loading Errors:** Ensure the URL or file path to the GeoTIFF file is correct and accessible.
*   **Rendering Issues:** Verify that your browser supports WebGL, which is required for rendering large raster datasets.
*   **Metadata Display Problems:** Check if the GeoTIFF file contains valid metadata information.

## Support

For questions or assistance, please contact our support team at [support email address].

---
