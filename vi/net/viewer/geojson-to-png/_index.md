---
title: GeoJSON to PNG Viewer
url: /vi/geojson-to-png/
weight: 10
layout: single
draft: false

---

## Overview

This application allows you to convert GeoJSON data into a PNG image. You can customize the appearance of the map, including the basemap, zoom level, and markers.

## Features

*   Convert GeoJSON data to PNG images
*   Customize basemaps
*   Adjust zoom levels
*   Add custom markers
*   Download generated images

## Usage

1.  **Input GeoJSON Data:** Provide a valid GeoJSON file or URL as input.
2.  **Configure Options:** Adjust the map settings, such as basemap, zoom level, and marker styles.
3.  **Generate Image:** Click the "Generate" button to create a PNG image of the GeoJSON data.
4.  **Download Image:** Download the generated PNG image for use in your projects.

## Configuration Options

*   **GeoJSON Source:** The URL or file path to the GeoJSON data.
*   **Basemap:** Select from available basemaps (e.g., OpenStreetMap, Mapbox).
*   **Zoom Level:** Adjust the zoom level of the map.
*   **Marker Style:** Customize the appearance of markers on the map.

## Example

```javascript
// Example GeoJSON data
var geojson = {
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [ -74.0060, 40.7128 ]
      },
      "properties": {
        "name": "New York City"
      }
    }
  ]
};

// Example basemap URL
var basemapUrl = "https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png";
```

## Troubleshooting

*   **Invalid GeoJSON:** Ensure the GeoJSON data is valid and well-formed.
*   **Basemap Issues:** Verify that the basemap URL is correct and accessible.
*   **Image Generation Errors:** Check for any errors in the configuration options or input data.

## Support

For questions or assistance, please contact us at [support email address].
---
