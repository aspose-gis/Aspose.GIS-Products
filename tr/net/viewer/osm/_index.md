---
title: OpenStreetMap Viewer
linkTitle: Açık Harita Görüntüleyici
weight: 10
url: /tr/net/viewer/osm/
aliases: [osm viewer, openstreetmap viewer]
description: View and interact with OpenStreetMap data.
---

## Introduction

This application provides a web-based interface for viewing and interacting with OpenStreetMap (OSM) data. It allows users to explore maps, query features, and perform basic analysis tasks.

## Features

*   **Map Display:** Displays OSM tiles using various providers.
*   **Feature Query:** Allows users to click on map elements and view their attributes.
*   **Data Download:** Enables downloading of OSM data in standard formats (e.g., GeoJSON, Shapefile).
*   **Custom Layers:** Supports adding custom layers from external sources.
*   **Routing:** Provides routing functionality using Open Source Routing Machine (OSRM).

## Usage

1.  **Loading the Map:** The application automatically loads a default map view centered on a specific location.
2.  **Navigation:** Use mouse wheel or touch gestures to zoom in and out. Drag the map to pan.
3.  **Feature Query:** Click on any feature (e.g., road, building) to display its attributes in a pop-up window.
4.  **Data Download:** Select "Download Data" from the menu to download OSM data for the current view. Specify the desired format and area of interest.
5.  **Custom Layers:** Add custom layers by providing a URL to a GeoJSON or Shapefile file.

## Configuration

The application can be configured using a configuration file. The following parameters can be adjusted:

*   `mapProvider`: Specifies the tile provider to use (e.g., OpenStreetMap, Mapbox).
*   `centerLatitude`: Sets the initial map center latitude.
*   `centerLongitude`: Sets the initial map center longitude.
*   `zoomLevel`: Sets the initial zoom level.
*   `osrmServerUrl`: Specifies the URL of the OSRM server for routing functionality.

## Troubleshooting

If you encounter any issues, please consult the following resources:

*   **FAQ:** Frequently Asked Questions
*   **Documentation:** Detailed documentation on application features and configuration options.
*   **Support Forum:** Online forum for users to ask questions and share solutions.

## Contributing

We welcome contributions from the community! Please refer to the `CONTRIBUTING.md` file for guidelines on how to contribute code, documentation, or other resources.
---
