---
title: KML to PNG Converter
linkTitle: แปลง KML เป็น PNG
weight: 10
url: /th/net/viewer/kml-to-png/
aliases: [KML to PNG, KML to image]
source: https://github.com/GIS-PRODUCTS/NetViewer/blob/main/src/NetViewer/KmlToPngConverter.cs
---

## Overview

This tool converts KML (Keyhole Markup Language) files into PNG images. It's useful for visualizing geographic data represented in KML format as static images.

## Features

*   **Conversion:** Converts KML files to PNG images.
*   **Customization:** Allows customization of the output image, including size and resolution.
*   **Easy to Use:** Simple command-line interface for easy integration into workflows.

## Usage

1.  **Installation:** Ensure you have the necessary dependencies installed.
2.  **Command Line Arguments:** Use the following arguments:

    ```
    KmlToPngConverter.exe -i input.kml -o output.png -s 512 -r 300
    ```

    *   `-i`: Specifies the input KML file.
    *   `-o`: Specifies the output PNG file.
    *   `-s`: Specifies the size of the image in pixels (default: 256).
    *   `-r`: Specifies the resolution of the image in DPI (default: 96).

## Example

To convert `my_location.kml` to `output.png` with a size of 1024x768 and a resolution of 240 DPI, use the following command:

```
KmlToPngConverter.exe -i my_location.kml -o output.png -s 1024 -r 240
```

## Troubleshooting

*   **Invalid KML File:** Ensure the input file is a valid KML file.
*   **Output File Error:** Check for write permissions to the specified output directory.
*   **Dependency Issues:** Verify that all required dependencies are installed correctly.

## Support

For any questions or issues, please contact us at [support@gis-products.com](mailto:support@gis-products.com).
