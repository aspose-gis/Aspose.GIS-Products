---
title: OSM to PNG Viewer
url: /nl/viewer/osm-to-png/
weight: 10
layout: ""
---

## Overview

This tool converts OpenStreetMap data to static images (PNG). It allows you to specify the area of interest, zoom level, and other parameters to generate customized maps.

## Features

*   Convert OSM data to PNG images
*   Specify bounding box for the map area
*   Adjust zoom level for desired detail
*   Customize image output with various options

## Usage

1.  **Input Data:** Provide OpenStreetMap data in a suitable format (e.g., .osm, .pbf).
2.  **Define Area:** Specify the coordinates of the bounding box to define the map area.
3.  **Set Zoom Level:** Choose an appropriate zoom level for the desired detail.
4.  **Configure Options:** Adjust other parameters like image size, resolution, and output format.
5.  **Generate Image:** Run the tool to generate a PNG image of the specified area with the configured options.

## Parameters

*   `--input`: Path to the OpenStreetMap data file.
*   `--bbox`: Bounding box coordinates (e.g., "south_latitude,west_longitude,north_latitude,east_longitude").
*   `--zoom`: Zoom level for the map.
*   `--output`: Path to save the generated PNG image.
*   `--width`: Width of the output image in pixels.
*   `--height`: Height of the output image in pixels.

## Example

```bash
osm-to-png --input data.osm --bbox 37.7,-122.4,37.8,-122.3 --zoom 12 --output map.png --width 512 --height 512
```

This command converts the `data.osm` file to a PNG image named `map.png`, focusing on an area around San Francisco with a zoom level of 12, and setting the image dimensions to 512x512 pixels.

## Notes

*   Ensure that the input OpenStreetMap data is valid and complete.
*   Adjust the bounding box and zoom level to achieve the desired map view.
*   Experiment with different output options to customize the generated images.

---
