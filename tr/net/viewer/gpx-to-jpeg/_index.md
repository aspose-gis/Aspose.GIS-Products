---
title: GPX to JPEG Conversion
linkTitle: GPX'i JPEG'e Dönüştürme
weight: 10
url: /tr/net/viewer/gpx-to-jpeg/
---

## Overview

This tool converts GPX files into JPEGs. It allows you to visualize your GPS data as an image, which can be useful for analysis or sharing.

## Usage

1.  **Input:** Provide a valid GPX file.
2.  **Output:** The tool generates a JPEG image representing the GPS track.

## Parameters

*   `imageWidth`: Width of the output JPEG image in pixels. (Varsayılan: 800)
*   `imageHeight`: Height of the output JPEG image in pixels. (Varsayılan: 600)
*   `scale`: Scale factor for the GPS coordinates. (Varsayılan: 1.0)
*   `offsetLat`: Latitude offset to center the track on the image. (Varsayılan: 0.0)
*   `offsetLon`: Longitude offset to center the track on the image. (Varsayılan: 0.0)

## Example

```java
// Convert GPX file to JPEG with custom parameters
GpxToJpegConverter converter = new GpxToJpegConverter();
converter.setImageWidth(1024);
converter.setImageHeight(768);
converter.setScale(0.5);
JPEG image = converter.convert("path/to/your/gpxfile.gpx");
image.save("output.jpg");
```

## Notes

*   The GPX file must contain track or route data for the conversion to work correctly.
*   Adjust the parameters as needed to achieve the desired visual representation of your GPS data.
*   Ensure that the input GPX file is valid and properly formatted.
