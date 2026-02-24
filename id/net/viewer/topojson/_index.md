---
title: TopoJSON Viewer
url: /id/viewer/topojson/
weight: 10
---

## Overview

The TopoJSON viewer allows you to visualize and interact with TopoJSON data. It provides a user-friendly interface for exploring geographic features, performing spatial analysis, and creating custom maps.

## Features

*   **Interactive Map:** Zoom, pan, and rotate the map to explore different regions.
*   **Feature Highlighting:** Hover over or click on features to view their attributes.
*   **Data Filtering:** Filter features based on specific attribute values.
*   **Custom Styling:** Customize the appearance of features using various styling options.
*   **Spatial Analysis Tools:** Perform basic spatial analysis operations, such as buffering and intersection.

## Usage

1.  **Load TopoJSON Data:** Load a TopoJSON file into the viewer.
2.  **Explore the Map:** Use the zoom and pan controls to navigate the map.
3.  **View Feature Attributes:** Hover over or click on features to see their attributes in a pop-up window.
4.  **Filter Features:** Use the filtering options to display only features that meet specific criteria.
5.  **Customize Styling:** Adjust the styling options to change the appearance of the features.

## Supported Formats

*   TopoJSON
*   GeoJSON (with limitations)

## Dependencies

*   Leaflet
*   TopoJSON
*   jQuery

## Example

```javascript
// Initialize the map
var map = L.map('map').setView([0, 0], 2);

// Add a tile layer
L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
    attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
}).addTo(map);

// Load TopoJSON data
L.topojson.featureCollection({
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {
        "name": "Example Feature"
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [[
          [ -127.0, 37.0 ],
          [ -126.0, 37.0 ],
          [ -126.0, 38.0 ],
          [ -127.0, 38.0 ],
          [ -127.0, 37.0 ]
        ]]
      }
    }
  ]
}).addTo(map);
```

## Troubleshooting

*   **Map Not Loading:** Ensure that the TopoJSON file is valid and accessible. Check your browser's developer console for any error messages.
*   **Features Not Displaying:** Verify that the feature attributes are correctly formatted and that the styling options are appropriate.
*   **Spatial Analysis Errors:** Double-check the input parameters and ensure that the spatial analysis tools are configured correctly.

## Contact

For questions or support, please contact us at [support email address].

---
