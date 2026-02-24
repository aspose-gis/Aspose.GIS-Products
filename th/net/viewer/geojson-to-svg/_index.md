---
title: GeoJSON to SVG Conversion
linkTitle: การแปลง GeoJSON เป็น SVG
weight: 10
url: /th/net/viewer/geojson-to-svg/
description: Learn how to convert GeoJSON data into SVG format for web mapping applications.
aliases: [geojson2svg, svg conversion]

---

## Introduction

This guide explains how to convert GeoJSON data into Scalable Vector Graphics (SVG) format. This process is essential for creating interactive and visually appealing maps on the web.  GeoJSON provides a standard way to encode geographic data, while SVG allows you to display that data as vector graphics in browsers.

## Prerequisites

*   A basic understanding of GeoJSON and SVG formats.
*   A text editor or IDE.
*   [net/viewer](url: /th/net/viewer/) library installed.

## Conversion Process

The conversion process typically involves the following steps:

1.  **Load GeoJSON Data:** Read your GeoJSON file into a data structure that can be processed by the conversion tool.
2.  **Style Features:** Define how each feature in the GeoJSON should be rendered as SVG elements (e.g., color, stroke width, fill).
3.  **Convert to SVG:** Use a library or script to transform the GeoJSON data and styles into an SVG string.
4.  **Display SVG:** Inject the generated SVG string into your web page's DOM.

## Example using net/viewer Library

The `net/viewer` library provides convenient functions for converting GeoJSON to SVG. Here’s a simple example:

```csharp
// Sample GeoJSON data (replace with your actual data)
string geoJsonString = @"
{
  ""type"": ""FeatureCollection"",
  ""features"": [
    {
      ""type"": ""Feature"",
      ""geometry"": { ""type"": ""Point"", ""coordinates"": [10.45, 52.52] },
      ""properties"": { ""name"": ""Berlin"" }
    }
  ]
}";

// Convert GeoJSON to SVG
string svgString = NetViewer.GeoJsonToSvg(geojsonString);

// Display the SVG (e.g., in a web page)
Console.WriteLine(svgString);
```

/* แปลง GeoJSON เป็น SVG ตัวอย่าง */

## Styling Options

You can customize the appearance of your SVG map by providing styling options during the conversion process. Common styling properties include:

*   `fill`: The fill color of polygons and other shapes.
*   `stroke`: The outline color of features.
*   `strokeWidth`: The thickness of the outline.
*   `opacity`: The transparency of features.

## Advanced Considerations

*   **Large Datasets:** For very large GeoJSON datasets, consider using techniques like data simplification or server-side rendering to improve performance.
*   **Dynamic Updates:** If your GeoJSON data changes frequently, you’ll need to regenerate the SVG dynamically.
*   **Error Handling:** Implement error handling to gracefully handle invalid GeoJSON input or other unexpected issues.

## Resources

*   [GeoJSON Specification](https://geojson.org/): Official specification for the GeoJSON format.
*   [SVG Specification](https://www.w3.org/TR/svg/): Official specification for SVG.
*   [net/viewer Library Documentation](url: /th/net/viewer/docs/): Detailed documentation for the `net/viewer` library.

---
