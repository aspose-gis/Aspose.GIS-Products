---
title: OSM to PNG Viewer
url: /vi/net/viewer/osm-to-png/
weight: 10
description: Convert OpenStreetMap data to PNG images.
---

## Overview

This tool converts OpenStreetMap (OSM) data into static PNG images. It allows you to define the area of interest, zoom level, and other parameters to generate customized map visualizations.

## Features

*   **Area Selection:** Define the region for which you want to generate a map image using bounding box coordinates or by selecting an area on an interactive map.
*   **Zoom Level Control:** Adjust the zoom level to control the detail of the generated map.
*   **Customizable Layers:** Choose from various OpenStreetMap layers, such as roads, buildings, and land use.
*   **Output Image Format:** Generate images in PNG format with customizable resolution.
*   **Dynamic Rendering:** The tool renders the map image dynamically based on your input parameters.

## Usage

1.  **Input Data:** Provide the coordinates of the area you want to visualize. You can enter latitude and longitude values or use the interactive map selection tool.
2.  **Zoom Level:** Set the desired zoom level for the map. Higher zoom levels will show more detail but may require more processing time.
3.  **Layer Selection:** Choose the OpenStreetMap layers you want to include in the generated image. You can select multiple layers to combine different types of information on the map.
4.  **Generate Image:** Click the "Generate" button to create the PNG image based on your settings. The generated image will be displayed and available for download.

## Parameters

*   `latitude`: The latitude coordinate of the area's center.
*   `longitude`: The longitude coordinate of the area's center.
*   `zoom`: The zoom level for the map (e.g., 10-18).
*   `layers`: A comma-separated list of OpenStreetMap layers to include (e.g., roads,buildings,landuse).

## Example

To generate a PNG image of London with a zoom level of 12 and including roads and buildings:

```
latitude=51.5074
longitude=-0.1278
zoom=12
layers=roads,buildings
```

## Troubleshooting

*   **Image Generation Errors:** If you encounter errors during image generation, try reducing the zoom level or simplifying the layer selection.
*   **Slow Rendering Times:** Generating high-resolution images with many layers can take time. Be patient or adjust your settings to reduce processing load.
*   **Map Display Issues:** Ensure that your browser supports PNG images and that JavaScript is enabled for interactive map features.

## Further Information

For more information about OpenStreetMap data and layers, please visit the [OpenStreetMap website](https://www.openstreetmap.org/).
---
