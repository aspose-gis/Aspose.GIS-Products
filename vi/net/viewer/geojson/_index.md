---
title: GeoJSON Viewer
url: /vi/viewer/geojson/
weight: 10
description: View and interact with GeoJSON data on a map.
aliases: [geojson viewer, geojson]
---

## Overview

The GeoJSON Viewer allows you to visualize and interact with GeoJSON data directly within the application. You can load GeoJSON files from your local machine or from a URL. The viewer provides tools for panning, zooming, and inspecting features.

## Features

*   **Load GeoJSON Data:** Load GeoJSON data from local files or URLs.
*   **Interactive Map:** Pan, zoom, and interact with the map to explore the data.
*   **Feature Inspection:** View detailed information about individual features by clicking on them.
*   **Styling Options:** Customize the appearance of GeoJSON features using various styling options.
*   **Data Filtering:** Filter GeoJSON features based on their attributes.

## Usage

1.  **Loading Data:**
    *   Click the "Load" button to select a GeoJSON file from your local machine.
    *   Enter a URL containing GeoJSON data in the URL field and click "Load."
2.  **Navigation:**
    *   Use the mouse wheel or trackpad to zoom in and out of the map.
    *   Click and drag the map to pan around.
3.  **Feature Inspection:**
    *   Click on a feature to view its attributes in a pop-up window.
4.  **Styling (Optional):**
    *   Adjust styling options such as color, fill opacity, and line width to customize the appearance of the GeoJSON features.

## Example GeoJSON Data

Here's an example of GeoJSON data that you can use to test the viewer:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [-73.9857, 40.7484]
      },
      "properties": {
        "name": "New York City",
        "population": 8419000
      }
    },
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [-74.02, 40.71],
            [-73.95, 40.75],
            [-73.98, 40.79],
            [-74.02, 40.71]
          ]
        ]
      },
      "properties": {
        "name": "Central Park",
        "area": 843
      }
    }
  ]
}
```

## Troubleshooting

*   **Error Loading Data:** Ensure that the GeoJSON file is valid and accessible. Check the URL if loading from a remote source.
*   **Map Not Displaying:** Verify that the map library is loaded correctly.
*   **Features Not Visible:** Make sure the GeoJSON data contains features within the current map extent.

## Further Reading

*   [GeoJSON Specification](https://geojson.org/format/)
---
