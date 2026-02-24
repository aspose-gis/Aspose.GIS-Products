---
title: GeoJSON Viewer
linkTitle: GeoJSON 뷰어
weight: 10
url: /ko/net/viewer/geojson/
aliases: [geojson viewer]
description: View and interact with GeoJSON data in your browser.
---

## Introduction ##

The GeoJSON Viewer is a tool that allows you to view and interact with GeoJSON data directly in your web browser. It provides a user-friendly interface for exploring geographic features, attributes, and relationships.

## Features ##

*   **Interactive Map:** Displays GeoJSON data on an interactive map using Leaflet.js.
*   **Feature Highlighting:** Highlights individual features when clicked or hovered over.
*   **Attribute Display:** Shows the attribute values associated with each feature in a sidebar panel.
*   **Zoom and Pan:** Allows users to zoom in and out of the map and pan around to explore different areas.
*   **Custom Styling:** Supports custom styling options for features based on their attributes.
*   **Data Filtering:** Enables filtering of features based on attribute values.

## Usage ##

1.  **Load GeoJSON Data:** Provide a URL or upload a GeoJSON file to the viewer.
2.  **Explore Features:** Click on features to view their attributes and details.
3.  **Zoom and Pan:** Use the map controls to navigate around the data.
4.  **Customize Styling (Optional):** Adjust the styling options to highlight specific features or patterns.

## Example ##

```javascript
// Example of loading GeoJSON data from a URL
L.geoJSON(geojsonData, {
    pointToLayer: function (feature, latlng) {
        return L.marker(latlng);
    }
}).addTo(map);
```

/* 예제: URL에서 GeoJSON 데이터를 로드하는 방법 */

## Customization ##

The GeoJSON Viewer can be customized to match your website's branding and design. You can modify the following aspects:

*   **Map Tiles:** Change the map tile provider (e.g., OpenStreetMap, Mapbox).
*   **Color Schemes:** Adjust the color schemes for features and labels.
*   **Font Styles:** Customize the font styles used in the viewer.
*   **Attribute Display Format:** Modify the format of attribute values displayed in the sidebar.

## Troubleshooting ##

*   **Data Loading Errors:** Ensure that the GeoJSON data is valid and accessible at the specified URL or file path.
*   **Map Rendering Issues:** Check for conflicts with other JavaScript libraries or CSS styles on your website.
*   **Attribute Display Problems:** Verify that the attribute names in the GeoJSON data match the expected format.

## Support ##

If you encounter any issues or have questions about the GeoJSON Viewer, please consult the documentation or contact us for support.
---
