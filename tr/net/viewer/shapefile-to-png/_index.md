---
title: Shapefile to PNG Conversion
linkTitle: Şekil Dosyasını PNG'ye Dönüştürme
weight: 10
url: /tr/net/viewer/shapefile-to-png/
description: Learn how to convert shapefiles to PNG images using .NET.
---

## Converting Shapefiles to PNG with .NET

This guide explains how to convert shapefiles (.shp) to Portable Network Graphics (.png) images using C# and the .NET framework. This process is useful for visualizing geospatial data in a more accessible format, such as incorporating them into reports or web applications.

### Prerequisites

Before you begin, ensure you have the following:

*   **A .NET Development Environment:**  Visual Studio or similar IDE.
*   **Shapefile Library:** You'll need a library to read and process shapefiles. A popular choice is [SharpMap](https://www.sharpmap.net/). Install it via NuGet Package Manager.
*   **Image Processing Library:** For creating PNG images, you can use `System.Drawing` which comes standard with .NET or an alternative like ImageMagick.

### Installation of SharpMap

Open your project in Visual Studio and go to Tools -> NuGet Package Manager -> Manage NuGet Packages for Solution. Search for "SharpMap" and install the latest stable version.

### Code Example

Here's a basic C# code example demonstrating how to convert a shapefile to a PNG image:

```csharp
// This code demonstrates converting a shapefile to a PNG image.
using SharpMap;
using SharpMap.Rendering;
using System.Drawing;
using System.IO;

public class ShapefileToolToPngConverter
{
    public static void ConvertShapefileToolToPng(string shapefilePath, string pngFilePath)
    {
        // Load the shapefile
        var stream = new FileResourceStream(shapefilePath);
        var map = MapDataProvider.CreateMap(stream, null);

        // Create a rendering configuration
        var renderConfiguration = new SimpleRenderingConfiguration();
        renderConfiguration.Background = Color.White; // Set background color

        // Render the map to a bitmap
        using (Bitmap bitmap = renderConfiguration.RenderMap(map, 500, 500))
        {
            // Save the bitmap as a PNG file
            bitmap.Save(pngFilePath, System.Drawing.Imaging.ImageFormat.Png);
        }
    }

    public static void Main(string[] args)
    {
        // Example usage:
        string shapefilePath = "path/to/your/shapefile.shp"; // Replace with your shapefile path
        string pngFilePath = "output.png"; // Replace with desired output PNG file path

        ConvertShapefileToolToPng(shapefilePath, pngFilePath);
    }
}
```

### Explanation

1.  **Include Namespaces:** The code starts by including necessary namespaces for SharpMap and image processing.
2.  **Load Shapefile:** `FileResourceStream` is used to load the shapefile from its path. `MapDataProvider.CreateMap` creates a map object from the stream.
3.  **Rendering Configuration:** A `SimpleRenderingConfiguration` is created to control how the map is rendered. The background color is set to white in this example.
4.  **Render Map:** The `renderConfiguration.RenderMap` method renders the map to a bitmap image with specified width and height (500x500 in this case).
5.  **Save as PNG:** Finally, the bitmap is saved as a PNG file using `bitmap.Save`.

### Customization

*   **Resolution:** Adjust the width and height parameters in `renderConfiguration.RenderMap` to control the resolution of the output PNG image.
*   **Background Color:** Modify the `Background` property in `renderConfiguration` to change the background color of the rendered map.
*   **Layer Visibility:**  SharpMap allows you to control which layers from the shapefile are visible during rendering. You can customize this by modifying the `Renderables` collection in the rendering configuration.
*   **Projections:** If your shapefile uses a different projection than your desired output, you'll need to handle reprojection using SharpMap’s projection capabilities.

### Error Handling

The provided code lacks robust error handling. In a production environment, you should add `try-catch` blocks to handle potential exceptions such as:

*   File not found
*   Invalid shapefile format
*   Insufficient permissions to write the output file

### Conclusion

This guide provides a basic framework for converting shapefiles to PNG images using .NET and SharpMap. By customizing the rendering configuration and adding error handling, you can create more sophisticated solutions for visualizing geospatial data. Remember to adjust paths and configurations according to your specific needs.
---
