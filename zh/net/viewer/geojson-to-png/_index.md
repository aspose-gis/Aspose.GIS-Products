---
title: GeoJSON to PNG Conversion
url: /zh/geojson-to-png/
weight: 10
layout: ""
---

## Overview

This tool converts GeoJSON data into PNG images. It allows you to visualize your geospatial data without needing complex mapping software.

## Features

*   **Simple Input:**  Upload a GeoJSON file or provide a URL.
*   **Customizable Output:** Control the image size, resolution, and background color.
*   **Fast Processing:** Quickly generate PNG images from your GeoJSON data.
*   **No Installation Required:**  A web-based tool accessible from any device with a browser.

## Usage

1.  **Input Method:** Choose to upload a GeoJSON file or enter a URL containing the GeoJSON data.
2.  **Customization Options:** Adjust the image size (width and height), resolution (DPI), and background color using the provided controls.
3.  **Generate Image:** Click the "Generate" button to create the PNG image.
4.  **Download:** Once the image is generated, download it to your local machine.

## Example GeoJSON

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [ -74.0060, 40.7128 ]
      },
      "properties": {
        "name": "New York City"
      }
    }
  ]
}
```

## Troubleshooting

*   **Invalid GeoJSON:** Ensure your GeoJSON file is valid and well-formed. Use a validator if necessary.
*   **Image Size Limits:** Very large GeoJSON files or extremely high resolutions may exceed processing limits. Try reducing the size or resolution.
*   **Error Messages:**  Pay attention to any error messages displayed on the screen, as they can provide clues about the problem.

## Support

For questions or assistance, please contact us at [support email address].

