---
title: GeoJSON to JPEG Conversion
linkTitle: GeoJSON naar JPEG conversie
weight: 10
url: /nl/net/viewer/geojson-to-jpeg/
description: Convert GeoJSON data to JPEG images using a .NET viewer.
---

## Overview

This application converts GeoJSON data into JPEG images. It allows you to visualize geospatial data as rasterized images, which can be useful for various purposes such as creating maps, generating previews, or integrating with other systems.

## Features

*   **GeoJSON Input:** Supports standard GeoJSON format as input.
*   **Rasterization:** Converts vector-based GeoJSON features into raster pixels.
*   **JPEG Output:** Generates JPEG images from the processed data.
*   **.NET Implementation:** Developed using .NET for cross-platform compatibility.
*   **Customizable Parameters:** Offers options to adjust rendering parameters like color, size, and resolution.

## Usage

1.  **Input Data:** Provide a valid GeoJSON file as input. The file should contain geographic features such as points, lines, or polygons.
2.  **Configuration:** Configure the conversion process by setting parameters such as output image dimensions, background color, feature colors, and rendering resolution.
3.  **Conversion:** Run the application to convert the GeoJSON data into a JPEG image.
4.  **Output Image:** The resulting JPEG image will be saved to the specified output location.

## Parameters

*   `--input`: Path to the input GeoJSON file.
*   `--output`: Path to save the generated JPEG image.
*   `--width`: Width of the output image in pixels (default: 512).
*   `--height`: Height of the output image in pixels (default: 512).
*   `--backgroundColor`: Background color for the image (default: white).
*   `--featureColor`: Color used to render GeoJSON features (default: black).
*   `--resolution`: Resolution of rendering in dots per inch (DPI) (default: 96).

## Example

```bash
geojson-to-jpeg --input data.geojson --output output.jpg --width 1024 --height 768 --featureColor red
```

This command converts `data.geojson` to `output.jpg`, sets the width to 1024 pixels, height to 768 pixels, and feature color to red.

## Dependencies

*   .NET runtime
*   GeoJSON library for .NET

## License

MIT License

## Contact

[contact information]
