---
title: GeoTIFF to SVG Conversion
url: /nl/geotiff-to-svg/
linkTitle: GeoTIFF naar SVG Conversie
weight: 10

---

## Overview

This viewer allows you to convert a GeoTIFF image into an SVG (Scalable Vector Graphics) file.  SVG is a vector format, which means it can be scaled without losing quality. This makes it ideal for web applications and other uses where high-resolution images are needed.

## Usage

1.  **Upload a GeoTIFF:** Drag and drop a GeoTIFF file onto the designated area or click "Choose File" to select one from your computer.
2.  **Adjust Parameters (Optional):** You can modify parameters like simplification tolerance, color map, and background color to fine-tune the SVG output.
3.  **Generate SVG:** Click the "Generate SVG" button to start the conversion process.
4.  **Download SVG:** Once the conversion is complete, a download link will appear allowing you to save the resulting SVG file.

## Parameters

*   **Simplification Tolerance:** Controls the level of simplification applied during the conversion. Lower values result in more detailed SVGs but larger file sizes. Higher values create simpler SVGs with smaller file sizes.
*   **Color Map:**  Allows you to apply a color map to the GeoTIFF data, which can be useful for visualizing elevation or other quantitative information.
*   **Background Color:** Sets the background color of the generated SVG.

## Troubleshooting

*   **File Size Limits:** There may be limitations on the size of GeoTIFF files that can be uploaded.  Large files may take longer to process or fail to upload altogether.
*   **Unsupported Formats:** Ensure that the file you are uploading is a valid GeoTIFF format.
*   **Conversion Errors:** If you encounter any errors during the conversion process, try adjusting the parameters or using a different GeoTIFF file.

## Notes

The generated SVG will represent the raster data from the GeoTIFF as vector paths. The accuracy of the resulting SVG depends on the resolution of the original GeoTIFF and the simplification tolerance setting.
---
