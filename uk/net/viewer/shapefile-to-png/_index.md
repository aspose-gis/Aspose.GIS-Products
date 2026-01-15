---
title: Перетворення Shapefile у PNG
url: /uk/viewer/shapefile-to-png/
weight: 10
layout: single
draft: false
description: Convert shapefiles to PNG images using .NET viewer.
---

## Convert Shapefile to PNG with .NET Viewer

This guide explains how to convert a shapefile (.shp) to a Portable Network Graphics (PNG) image using our .NET viewer library. This process is useful for creating raster representations of vector data, which can be beneficial for various applications like web mapping and data visualization.

### Prerequisites

Before you begin, ensure that you have the following:

*   **.NET SDK:**  Make sure you have the .NET SDK installed on your system. You can download it from the official Microsoft website.
*   **GeoComposer Library:** Download the GeoComposer library for .NET. This library provides the necessary functionalities to read shapefiles and render them as images.

### Steps

1.  **Install GeoComposer Package:** Use NuGet package manager to install the `GeoComposer` package in your project.

    ```bash
    dotnet add package GeoComposer
    ```

2.  **Import Namespaces:** Import the required namespaces into your .NET code file.

    ```csharp
    using GeoComposer;
    using GeoComposer.Rasterize;
    using System.Drawing;
    using System.IO;
    ```

3.  **Read Shapefile:** Use `Shapefile.Open` method to read the shapefile data.

    ```csharp
    string shapefilePath = "path/to/your/shapefile.shp";
    Shapefile shapefile = Shapefile.Open(shapefilePath);
    ```

4.  **Configure Rasterization Options:** Create a `RasterizeOptions` object to configure the rasterization process. This includes setting parameters like output image size, background color, and simplification tolerance.

    ```csharp
    var options = new RasterizeOptions
    {
        Width = 512,
        Height = 512,
        BackgroundColor = Color.White,
        SimplifyTolerance = 0.001 // Adjust as needed
    };
    ```

5.  **Rasterize Shapefile:** Use the `Rasterizer` class to rasterize the shapefile data based on the configured options.

    ```csharp
    using (var rasterizer = new Rasterizer(shapefile, options))
    {
        Bitmap bitmap = rasterizer.Render();
    }
    ```

6.  **Save as PNG:** Save the rendered `Bitmap` object to a PNG file using `Bitmap.Save`.

    ```csharp
    string outputFilePath = "path/to/output/image.png";
    bitmap.Save(outputFilePath, System.Drawing.Imaging.ImageFormat.Png);
    ```

### Complete Example

Here's a complete example demonstrating the process of converting a shapefile to a PNG image:

```csharp
using GeoComposer;
using GeoComposer.Rasterize;
using System.Drawing;
using System.IO;

public class ShapefileToolToPngConverter
{
    public static void Convert(string shapefilePath, string outputFilePath)
    {
        // Read the shapefile
        Shapefile shapefile = Shapefile.Open(shapefilePath);

        // Configure rasterization options
        var options = new RasterizeOptions
        {
            Width = 512,
            Height = 512,
            BackgroundColor = Color.White,
            SimplifyTolerance = 0.001
        };

        // Rasterize the shapefile
        using (var rasterizer = new Rasterizer(shapefile, options))
        {
            Bitmap bitmap = rasterizer.Render();
        }

        // Save as PNG
        bitmap.Save(outputFilePath, System.Drawing.Imaging.ImageFormat.Png);
    }

    public static void Main(string[] args)
    {
        // Example usage:
        Convert("path/to/your/shapefile.shp", "path/to/output/image.png");
    }
}
```

### Considerations

*   **Simplify Tolerance:** Adjust the `SimplifyTolerance` value based on the complexity of your shapefile and desired level of detail in the output image. Lower values preserve more detail but may result in larger images.
*   **Image Size:**  Experiment with different width and height values for the `RasterizeOptions` to achieve the desired resolution for your PNG image.
*   **Error Handling:** Implement proper error handling to gracefully handle potential issues such as invalid shapefile paths or file access errors.
*   **Coordinate Reference System (CRS):** Ensure that the shapefile's CRS is properly handled during rasterization, especially if you are working with data from different geographic regions.

### Conclusion

By following these steps and utilizing the GeoComposer library, you can effectively convert shapefiles to PNG images using .NET viewer. This process enables you to create visual representations of your vector data for various applications and workflows.
---
