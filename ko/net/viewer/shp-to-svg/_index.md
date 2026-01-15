---
title: SHP to SVG Conversion
linkTitle: SHP에서 SVG로 변환하기
weight: 10
url: /ko/viewer/shp-to-svg/
description: Convert shapefiles (.shp) into scalable vector graphics (.svg) format. Shapefiles are a popular geospatial data format, but sometimes you need to convert them to SVG for web display or other purposes. This tool allows you to do just that.
---

## Overview

This tool converts SHP files to SVG format.  It's useful when you want to use shapefile data on the web or in applications where SVG is preferred.

## Usage

1.  **Upload your SHP file:** Drag and drop your `.shp` file into the designated area, or click "Choose File" to select it from your computer.
2.  **Configure options (optional):** You can adjust parameters like simplification tolerance and output styling.
3.  **Convert:** Click the "Convert" button to start the conversion process.
4.  **Download SVG:** Once the conversion is complete, a link will appear allowing you to download the resulting `.svg` file.

## Options

*   **Simplification Tolerance:** This value controls how much the geometry is simplified during the conversion. Lower values preserve more detail but result in larger files. Higher values reduce file size but may lose some accuracy.  A default value of `0.1` is usually a good starting point.
*   **Output Styling:** Customize the appearance of the SVG output. Options include:
    *   Fill color
    *   Stroke color
    *   Stroke width

## Example

Let's say you have a shapefile containing data about parks in a city. You want to display this data on your website, but your web application only supports SVG format.  Using this tool, you can easily convert the SHP file into an SVG file and embed it in your webpage.

## Troubleshooting

*   **File Size Limits:** Large shapefiles may exceed upload limits. Try simplifying the geometry or splitting the file into smaller parts.
*   **Conversion Errors:** If you encounter errors during conversion, ensure that your SHP file is valid and not corrupted.  Check for any invalid characters in the attribute data.
*   **SVG Display Issues:** If the SVG doesn't display correctly in your browser, try adjusting the simplification tolerance or checking for compatibility issues with your web application.

## Further Reading

*   [Shapefile Format](https://en.wikipedia.org/wiki/Shapefile)
*   [Scalable Vector Graphics (SVG)](https://www.w3.org/Graphics/SVG/)

