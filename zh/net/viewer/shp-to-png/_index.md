---
title: Convert SHP to PNG
url: /zh/viewer/shp-to-png/
weight: 10
layout: single
draft: false
toc: true
---

## Overview

This tool converts shapefiles (.shp) into Portable Network Graphics (.png) images. It's useful for visualizing geospatial data and creating maps.

## Requirements

*   GDAL (Geospatial Data Abstraction Library) installed on your system.  Make sure the `gdal-config` command is available in your terminal.
*   Python 3.6 or higher.

## Installation

1.  Clone this repository:

    ```bash
    git clone [repository URL]
    cd shp-to-png
    ```

2.  Create a virtual environment (recommended):

    ```bash
    python3 -m venv .venv
    source .venv/bin/activate  # On Linux/macOS
    .venv\Scripts\activate  # On Windows
    ```

3.  Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  **Basic Conversion:**

    To convert a shapefile named `my_shapefile.shp` to a PNG image named `output.png`, run:

    ```bash
    python main.py --input my_shapefile.shp --output output.png
    ```

2.  **Customization Options:**

    *   `--input`: Path to the input shapefile (.shp). Required.
    *   `--output`: Path to the output PNG image file. Required.
    *   `--width`: Width of the output image in pixels. Default is 500.
    *   `--height`: Height of the output image in pixels. Default is 500.
    *   `--scale`: Scale factor for the shapefile data. Default is 1.0.
    *   `--resolution`: Resolution of the output image in DPI (dots per inch). Default is 300.
    *   `--color-map`:  Specify a color map to apply to the shapefile's attributes. See GDAL documentation for available color maps.
    *   `--attribute`: Attribute field to use for coloring the shapes. If not specified, all shapes will be rendered with the same color.
    *   `--no-data`: Value representing no data in the attribute field. Shapes with this value will be excluded from the output image.

    Example:

    ```bash
    python main.py --input my_shapefile.shp --output colored_map.png --attribute population --color-map viridis --no-data -9999
    ```

## Configuration

The script uses command-line arguments for configuration.  There is no separate configuration file.

## Troubleshooting

*   **GDAL Not Found:** Ensure GDAL is installed correctly and the `gdal-config` command is accessible in your system's PATH environment variable.
*   **Shapefile Errors:** Check that the input shapefile is valid and not corrupted.
*   **Attribute Field Issues:** Verify that the specified attribute field exists in the shapefile and contains numeric data if using a color map.

## Contributing

Feel free to contribute by submitting bug reports, feature requests, or pull requests.

## License

This project is licensed under the [MIT License](LICENSE).

---

