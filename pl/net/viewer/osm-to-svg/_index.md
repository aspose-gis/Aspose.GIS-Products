---
title: OSM to SVG Viewer
linkTitle: Przeglądarka OSM do SVG
weight: 10
url: /pl/net/viewer/osm-to-svg/
description: A simple viewer for converting OpenStreetMap data to SVG format.
tags: [ gis, openstreetmap, svg, viewer ]
---

## Overview

This project provides a simple viewer for converting OpenStreetMap (OSM) data to Scalable Vector Graphics (SVG) format. It allows users to visualize and interact with OSM data in a web browser without requiring complex software installations.

## Features

*   **Data Source:** Supports loading OSM data from Overpass API or local GeoJSON files.
*   **Rendering:** Renders OSM features as SVG elements, allowing for customization of styles and attributes.
*   **Interaction:** Provides basic interaction capabilities such as zooming, panning, and feature selection.
*   **Customization:** Allows users to customize the rendering style through configuration options.

## Usage

1.  **Data Source Selection:** Choose either Overpass API or local GeoJSON file as the data source.
2.  **Configuration:** Configure the viewer with desired settings such as map center, zoom level, and rendering styles.
3.  **Visualization:** The viewer will fetch and render the OSM data in SVG format.
4.  **Interaction:** Use mouse/touch controls to explore the map and interact with features.

## Configuration Options

*   `mapCenter`: Coordinates of the map center (latitude, longitude).
*   `zoomLevel`: Initial zoom level of the map.
*   `renderingStyles`: Custom styles for rendering OSM features.  /* Style dla renderowania elementów OSM */
*   `overpassApiUrl`: URL of the Overpass API endpoint.

## Technical Details

The viewer is built using JavaScript and SVG. It utilizes libraries such as Leaflet for map interaction and Overpass-API for data retrieval.

## Future Enhancements

*   Support for more advanced rendering styles.
*   Integration with other GIS tools and services.
*   Improved performance for large datasets.
*   User authentication and authorization.
---
