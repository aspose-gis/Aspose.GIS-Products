---
title: GeoJSON Viewer
url: /ja/viewer/geojson/
weight: 10
---

## Overview

The GeoJSON Viewer is a tool for visualizing and interacting with GeoJSON data. It allows users to load, display, and explore geographic information encoded in the GeoJSON format.

## Features

*   **Loading GeoJSON Data:** Supports loading GeoJSON data from URLs or local files.
*   **Interactive Map Display:** Provides an interactive map interface for displaying GeoJSON features.
*   **Feature Highlighting:** Allows users to highlight individual features on the map.
*   **Data Inspection:** Enables users to inspect the attributes and properties of each feature.
*   **Zoom and Pan Controls:** Includes zoom and pan controls for navigating the map.
*   **Customizable Styling:** Offers options for customizing the appearance of GeoJSON features (e.g., color, size, shape).

## Usage

1.  **Load Data:** Provide a URL or upload a local GeoJSON file.
2.  **Explore Map:** Use zoom and pan controls to navigate the map.
3.  **Inspect Features:** Click on features to view their attributes in the data panel.
4.  **Customize Styling (Optional):** Adjust styling options to modify the appearance of the features.

## Example GeoJSON Data

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [-122.4194, 37.7749]
      },
      "properties": {
        "name": "San Francisco",
        "population": 808465
      }
    },
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [-122.48, 37.7],
            [-122.40, 37.7],
            [-122.40, 37.8],
            [-122.48, 37.8],
            [-122.48, 37.7]
          ]
        ]
      },
      "properties": {
        "name": "Golden Gate Park",
        "area": 1370
      }
    }
  ]
}
```

## Supported GeoJSON Types

The viewer supports the following GeoJSON types:

*   **Feature:** Represents a geographic feature with geometry and properties.
*   **FeatureCollection:** A collection of features.
*   **Point:** Represents a single location on Earth.
*   **LineString:** Represents a sequence of connected points.
*   **Polygon:** Represents a closed shape defined by a series of connected points.
*   **MultiPoint:** Represents a collection of points.
*   **MultiLineString:** Represents a collection of line strings.
*   **MultiPolygon:** Represents a collection of polygons.

## Troubleshooting

*   **Data Loading Errors:** Verify the GeoJSON data is valid and accessible. Check for network connectivity issues if loading from a URL.
*   **Map Display Issues:** Ensure the map container has sufficient space to display the map.
*   **Styling Problems:** Review the styling options to ensure they are compatible with the GeoJSON data.

---
