---
title: OSM to PNG Viewer
url: /uk/osm-to-png/
weight: 10
layout: ""
---

## Overview

This tool converts OpenStreetMap data to static images (PNG). It allows you to specify the area of interest, zoom level, and other parameters to generate customized map images.

## Features

*   Convert OSM data to PNG images
*   Specify bounding box for the area of interest
*   Adjust zoom level for desired detail
*   Customize image output with various options

## Usage

1.  **Input Data:** Provide OpenStreetMap data in a suitable format (e.g., .osm, .pbf).
2.  **Configuration:** Set parameters such as bounding box coordinates, zoom level, and output resolution.
3.  **Conversion:** Run the conversion process to generate the PNG image.

## Parameters

*   `bbox`: Bounding box coordinates in the format `[min_lat, min_lon, max_lat, max_lon]`.
*   `zoom`: Zoom level for the map (e.g., 1-18).
*   `output`: Output file name with .png extension.

## Example

```java
// This is an example of how to use the tool in Java
OsmToPngConverter converter = new OsmToPngConverter();
converter.setBbox(37.7749, -122.4194, 37.7833, -122.4064); // San Francisco coordinates
converter.setZoom(12);
converter.setOutput("san_francisco.png");
converter.convert();
```

## Troubleshooting

*   **Invalid Bounding Box:** Ensure the bounding box coordinates are valid and within the range of OpenStreetMap data.
*   **Zoom Level Too High:**  High zoom levels may result in large image files or errors due to data limitations.
*   **Data Format Error:** Verify that the input OSM data is in a supported format.

## Support

For any questions or issues, please contact our support team at [support email address].

---
