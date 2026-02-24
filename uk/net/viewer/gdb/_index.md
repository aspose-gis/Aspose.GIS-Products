---
title: GDB Viewer
linkTitle: Переглядач GDB
weight: 10
url: /uk/net/viewer/gdb/
aliases: [GDB Viewer, ГІС переглядач]
description: The GDB Viewer allows you to view and interact with geodatabases.
---

## Overview

The GDB Viewer is a tool that allows you to view and interact with geodatabases. It provides a user-friendly interface for exploring the contents of a GDB, including tables, feature classes, rasters, and other spatial data.

## Features

*   **Browse GDB Contents:** Easily navigate through the different layers within a geodatabase.
*   **View Spatial Data:** Visualize feature classes, rasters, and other spatial datasets on a map.
*   **Attribute Table Exploration:** Examine attribute data associated with features in tables.
*   **Querying and Filtering:** Filter data based on specific criteria to focus on relevant information.
*   **Zoom and Pan:** Navigate the map view by zooming in/out and panning around.
*   **Identify Features:** Locate and identify individual features on the map.

## Usage

1.  **Open a GDB:** Use the "Open" button to select a geodatabase file (.gdb).
2.  **Explore Layers:** Expand the layer tree in the left panel to view available layers.
3.  **View Data:** Double-click on a layer to display it on the map.
4.  **Interact with Features:** Use the tools in the toolbar to query, select, and zoom to features.

## Supported Formats

The GDB Viewer supports the following geodatabase formats:

*   Esri File Geodatabase (.gdb)
*   Esri Personal Geodatabase (.mdb)
*   SQLite Spatialite (.sqlite)

## Troubleshooting

*   **Unable to Open GDB:** Ensure that the GDB file is not corrupted and that you have sufficient permissions to access it.
*   **Slow Performance:** Large geodatabases can take time to load and display. Try filtering data or simplifying layer symbology to improve performance.
*   **Missing Layers:** Verify that the GDB contains the expected layers and that they are properly registered in the system catalog.

## Known Issues

*   Support for complex raster datasets is limited.
*   Performance may be affected by the size and complexity of the geodatabase.

