---
title: GeoJSON to SVG Conversion
url: /it/viewer/geojson-to-svg/
linkTitle: Conversione da GeoJSON a SVG
weight: 10
---

## Overview

This tool converts GeoJSON data into SVG format.  It allows you to visualize and manipulate geographic data in a vector graphics environment.

## Input Format

The input should be a valid GeoJSON file or string. The GeoJSON can contain various geometric objects such as points, lines, polygons, and collections of these.

## Output Format

The output is an SVG (Scalable Vector Graphics) representation of the GeoJSON data.  This SVG can then be displayed in web browsers or used in other vector graphics applications.

## Usage

1.  **Provide GeoJSON Data:** You can either upload a GeoJSON file or paste the GeoJSON data directly into the input field.
2.  **Configure Options (Optional):** Adjust styling options such as stroke color, fill color, and line width to customize the appearance of the SVG output.
3.  **Generate SVG:** Click the "Convert" button to generate the SVG representation of your GeoJSON data.
4.  **Download or View SVG:** The generated SVG will be displayed on the screen and also available for download.

## Example

Here's an example of a simple GeoJSON input:

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
        "name": "New York City"
      }
    }
  ]
}
```

This GeoJSON represents a single point feature for New York City. The tool will convert this into an SVG marker at the specified coordinates.

## Styling Options

*   **Stroke Color:**  The color of the lines in the SVG.
*   **Fill Color:** The color used to fill polygons and other shapes.
*   **Line Width:** The thickness of the lines.
*   **Point Radius:** The radius of points displayed on the map.
*   **Polygon Fill Opacity:**  The opacity of polygon fills (0-1).

## Error Handling

The tool provides error messages if the GeoJSON input is invalid or if there are issues during the conversion process. Please review these messages carefully to correct any errors in your data or configuration.

## Limitations

*   Large GeoJSON files may take longer to convert.
*   Complex geometries can result in very large SVG files.
*   The tool does not support all GeoJSON features (e.g., time-based data).
---
