---
title: GeoTIFF Viewer
linkTitle: Przeglądarka GeoTIFF
weight: 10
url: /pl/net/viewer/geotiff/
description: View and interact with GeoTIFF files in your .NET applications.
---

## Introduction

The GeoTIFF Viewer control allows you to display and interact with GeoTIFF raster datasets within your .NET applications. It provides a user-friendly interface for exploring geospatial data, including zooming, panning, and measuring distances.

## Features

*   **GeoTIFF Support:** Native support for reading and displaying GeoTIFF files.
*   **Zooming and Panning:** Intuitive controls for navigating the image.
*   **Measurement Tools:** Measure distances and areas directly on the map.
*   **Coordinate System Transformation:** Reproject data between different coordinate systems.
*   **.NET Integration:** Seamlessly integrate into your existing .NET projects.

## Installation

You can install the GeoTIFF Viewer control using NuGet:

```powershell
Install-Package NetGeotiffViewer
```

## Usage

Here's a basic example of how to use the GeoTIFF Viewer in your application:

```csharp
// Create a new instance of the GeoTiffViewer control.
var viewer = new GeotiffViewer();

// Load a GeoTIFF file.
viewer.Load("path/to/your/geotiff.tif");

// Add the viewer to a container in your application.
// For example, you can add it to a Panel or PictureBox control.
```

## Advanced Features

*   **Custom Rendering:** Customize the appearance of the image using custom rendering techniques.
*   **Overlaying Data:** Overlay vector data and other geospatial information on top of the GeoTIFF image.
*   **Georeferencing:**  Accurately display GeoTIFF images in their correct geographic location.

## Troubleshooting

If you encounter any issues while using the GeoTIFF Viewer, please refer to the following resources:

*   [FAQ](url)
*   [Support Forum](url)
*   [Documentation](url)

---
