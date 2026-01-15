---
title: SHP to SVG Viewer
url: /he/shp-to-svg/
weight: 10
layout: ""
---

## SHP to SVG Viewer

This tool converts ESRI Shapefiles (.shp) into Scalable Vector Graphics (.svg).

### Features

*   Convert SHP files to SVG format.
*   Support for various SHP file types (point, line, polygon).
*   Customizable output options.
*   Simple and easy-to-use interface.

### Usage

1.  Place your .shp file in the input directory.
2.  Run the conversion process.
3.  The converted .svg file will be generated in the output directory.

### Input Format

*   Supported formats: ESRI Shapefile (.shp)
*   File size limit: 100MB

### Output Format

*   SVG (Scalable Vector Graphics)

### Dependencies

*   Python 3.x
*   Shapely library
*   svgwrite library

### Installation

```bash
pip install shapely svgwrite
```

### Configuration

The tool can be configured using a configuration file. The configuration file should be in JSON format and contain the following parameters:

*   `input_directory`: The directory containing the input .shp files.
*   `output_directory`: The directory where the converted .svg files will be saved.
*   `file_pattern`: A regular expression pattern to match the .shp files to be converted.

Example configuration file:

```json
{
  "input_directory": "/path/to/input",
  "output_directory": "/path/to/output",
  "file_pattern": ".*\\.shp$"
}
```

### Troubleshooting

*   If you encounter any issues, please check the logs for error messages.
*   Make sure that all dependencies are installed correctly.
*   Verify that the input file is a valid ESRI Shapefile.

### Contact

For support or inquiries, please contact us at [support email address].

---
