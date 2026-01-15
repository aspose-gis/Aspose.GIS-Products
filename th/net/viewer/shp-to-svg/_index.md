---
title: SHP to SVG Viewer
url: /th/shp-to-svg/
weight: 10
layout: single
start: true
toc: true
draft: false
---

## Overview

This application converts ESRI Shapefiles (.shp) into Scalable Vector Graphics (.svg).  It allows users to visualize and interact with geospatial data in a web browser.

## Features

*   **Shapefile Conversion:** Converts .shp files to .svg format.
*   **Web-Based Visualization:** Displays the converted SVG file in a web browser.
*   **Interactive Map:** Allows panning, zooming, and identifying features on the map.
*   **Attribute Data Display:** Shows attribute data associated with each feature.
*   **Customizable Styling:** Provides options for customizing the appearance of the map (e.g., colors, line widths).

## Usage

1.  **Input Shapefile:** Provide a valid .shp file as input.
2.  **Conversion Process:** The application converts the shapefile into an SVG format.
3.  **Visualization:** The converted SVG is displayed in a web browser window.
4.  **Interaction:** Users can interact with the map by panning, zooming, and querying features.

## Technical Details

*   **Programming Language:** C#
*   **Framework:** ASP.NET Core
*   **Mapping Library:** SharpMap (for shapefile reading and processing)
*   **SVG Generation:**  Custom SVG generation logic
*   **Web Server:** Kestrel

## Dependencies

*   **.NET 6.0 SDK**
*   **SharpMap library** (version 2.1 or later)

## Installation

1.  **Clone the Repository:** `git clone [repository URL]`
2.  **Restore Packages:** `dotnet restore`
3.  **Build the Application:** `dotnet build`
4.  **Publish the Application:** `dotnet publish -c Release`
5.  **Run the Application:** Navigate to the published directory and execute the application (e.g., `shp-to-svg.exe`).

## Configuration

The application can be configured using environment variables or a configuration file (`appsettings.json`).  Key configuration options include:

*   **SharpMap Input Path:** The path to the directory containing the shapefiles.
*   **SVG Output Path:** The path to the directory where converted SVG files will be saved.
*   **Port Number:** The port number on which the web server will listen.

## Troubleshooting

*   **Shapefile Errors:** Ensure that the input .shp file is valid and not corrupted.
*   **SharpMap Issues:** Verify that the SharpMap library is installed correctly and compatible with the application.
*   **Web Server Problems:** Check for any errors in the web server logs.

## Future Enhancements

*   **Support for other geospatial formats:** Add support for GeoJSON, KML, and other common geospatial data formats.
*   **Improved Styling Options:** Provide more advanced styling options for customizing the appearance of the map.
*   **Geocoding Integration:** Integrate with a geocoding service to allow users to search for locations on the map.
*   **User Authentication:** Implement user authentication and authorization to restrict access to certain features.

## License

This application is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
