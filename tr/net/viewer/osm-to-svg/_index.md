---
title: OSM to SVG Viewer
linkTitle: OSM’ye SVG Görüntüleyici
weight: 10
url: /tr/net/viewer/osm-to-svg/
aliases: [osm2svg, osm-to-svg]
description: OpenStreetMap verilerini SVG formatına dönüştüren bir görüntüleyicidir.
---

## Overview

This application allows you to convert OpenStreetMap data into an SVG (Scalable Vector Graphics) file and view it in a browser.  It's useful for creating custom maps, extracting vector data, or simply visualizing OSM data in a different format.

## Features

*   **Convert OSM Data:** Converts `.osm` or `.xml` files containing OpenStreetMap data into SVG format.
*   **Interactive Viewing:** View the generated SVG map interactively within the application.
*   **Zoom and Pan:**  Standard zoom and pan controls for easy navigation.
*   **Customizable Rendering:** Options to control how features are rendered (e.g., roads, buildings, labels).
*   **Data Filtering:** Filter specific types of OSM data to display.

## Usage

1.  **Input Data:** Provide an `.osm` or `.xml` file containing OpenStreetMap data. You can download these files from various sources online, such as Geofabrik or Overpass Turbo.
2.  **Conversion:** The application will convert the input data into SVG format. This process may take some time depending on the size of the dataset.
3.  **Viewing:** Once the conversion is complete, the generated SVG map will be displayed in the viewer.

## Configuration Options

*   `--input`: Specifies the input OSM or XML file. Example: `--input data.osm`
*   `--output`: Specifies the output SVG file. If not provided, the SVG will be displayed in the browser. Example: `--output map.svg`
*   `--scale`: Sets the initial zoom scale of the map.  Example: `--scale 1000`
*   `--projection`: Defines the projection to use for rendering the map. (e.g., "EPSG:3857")

## Example Command Line Usage

```bash
# Convert data.osm to map.svg with a scale of 1000
./osm-to-svg --input data.osm --output map.svg --scale 1000

# View data.osm in the browser with default settings
./osm-to-svg data.osm
```

## Troubleshooting

*   **Large Files:** Converting very large OSM files can be slow and may require significant memory. Consider splitting large files into smaller regions.
*   **Rendering Issues:** If you encounter rendering issues, try adjusting the `--scale` option or experimenting with different projection settings.
*   **Data Errors:**  Errors in the input OSM data can cause conversion failures. Validate your data before attempting to convert it.

## Contributing

Contributions are welcome! Please see the `CONTRIBUTING.md` file for details on how to contribute.

---
