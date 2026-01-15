---
title: OSM to PNG Viewer
url: /th/osm-to-png/
weight: 10
layout: ""
---

## Overview

This tool converts OpenStreetMap data to PNG images. It allows you to specify the area of interest, zoom level, and other parameters to generate customized map images.

## Features

*   Convert OSM data to PNG images
*   Specify area of interest (bounding box)
*   Adjust zoom level for desired detail
*   Customize image output (width, height)
*   Support various tile servers (OpenStreetMap, Mapbox, etc.)

## Usage

1.  **Input Data:** Provide OpenStreetMap data in a suitable format (e.g., .osm, .pbf).
2.  **Define Area of Interest:** Specify the latitude and longitude coordinates for the top-left and bottom-right corners of the area you want to capture.
3.  **Set Zoom Level:** Choose an appropriate zoom level based on the desired detail. Higher zoom levels result in more detailed images but may take longer to generate.
4.  **Configure Output Image:** Set the width and height of the output PNG image.
5.  **Select Tile Server:** Choose a tile server to use for rendering the map data. OpenStreetMap is a good default option, but you can also use other providers like Mapbox.
6.  **Generate Image:** Click the "Generate" button to create the PNG image.

## Parameters

*   `bbox`: Bounding box coordinates (top-left latitude/longitude, bottom-right latitude/longitude).
*   `zoom`: Zoom level for the map rendering.
*   `width`: Width of the output PNG image in pixels.
*   `height`: Height of the output PNG image in pixels.
*   `tile_server`: URL of the tile server to use (e.g., "https://tile.openstreetmap.org/{z}/{x}/{y}.png").

## Example

```
// Example usage:
osmToPng(bbox=[-34.0, -58.0, -33.0, -57.0], zoom=12, width=512, height=512, tile_server="https://tile.openstreetmap.org/{z}/{x}/{y}.png");
```

## Troubleshooting

*   **Image Generation Errors:** Check the input data format and bounding box coordinates. Ensure that the specified area of interest is within the bounds of the map data.
*   **Slow Image Generation:** Reduce the zoom level or image dimensions to improve performance.
*   **Tile Server Issues:** Verify that the tile server URL is correct and accessible. Try a different tile server if necessary.

## Further Information

For more information about OpenStreetMap and tile servers, please refer to the following resources:

*   [OpenStreetMap](https://www.openstreetmap.org/)
*   [Mapbox](https://www.mapbox.com/)

---
