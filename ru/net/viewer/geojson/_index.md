---
title: GeoJSON Viewer
linkTitle: Просмотрщик GeoJSON
weight: 10
url: /ru/net/viewer/geojson/
aliases: [geojson-viewer]
---

## Overview

The GeoJSON Viewer is a web application that allows you to view and interact with GeoJSON data. It provides a user-friendly interface for exploring geographic features, including points, lines, polygons, and collections of these features.

## Features

*   **Display GeoJSON Data:** Easily visualize GeoJSON files on an interactive map.
*   **Zoom and Pan:** Navigate the map to explore different areas of interest.
*   **Feature Highlighting:** Hover over or click on individual features to view their attributes.
*   **Attribute Tables:** View detailed information about each feature in a tabular format.
*   **Custom Styling:** Customize the appearance of features using various styling options.
*   **Data Filtering:** Filter features based on specific attribute values.

## Usage

1.  **Load GeoJSON Data:** Provide a URL or upload a GeoJSON file to load the data into the viewer.
2.  **Explore the Map:** Use the zoom and pan controls to navigate the map and view different areas.
3.  **Inspect Features:** Hover over or click on features to see their attributes in the attribute table.
4.  **Customize Styling (Optional):** Adjust the styling options to change the appearance of the features.

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
        "type": "LineString",
        "coordinates": [
          [-122.4194, 37.7749],
          [-122.4008, 37.7836]
        ]
      },
      "properties": {
        "name": "Street",
        "length": 1000
      }
    }
  ]
}
```

## Supported GeoJSON Types

The viewer supports the following GeoJSON types:

*   Point
*   LineString
*   Polygon
*   MultiPoint
*   MultiLineString
*   MultiPolygon
*   GeometryCollection

## Customization Options

The viewer offers several customization options to tailor the display of your GeoJSON data. These options include:

*   **Map Style:** Choose from a variety of pre-defined map styles or create your own custom style.
*   **Feature Styling:** Customize the appearance of features based on their attributes, such as color, size, and opacity.
*   **Attribute Display:** Select which attributes to display in the attribute table.
*   **Zoom Level:** Set the initial zoom level for the map.

## Troubleshooting

If you encounter any issues while using the GeoJSON Viewer, please refer to the following troubleshooting tips:

*   **Check GeoJSON Validity:** Ensure that your GeoJSON data is valid and well-formed.  You can use online validators to check for errors.
*   **Verify Data Loading:** Make sure the URL or file path you provided is correct and accessible.
*   **Inspect Browser Console:** Check the browser console for any error messages that may provide clues about the problem.

## Contact

For questions or support, please contact us at [support email address].

---
