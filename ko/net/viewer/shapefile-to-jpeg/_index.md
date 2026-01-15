---
title: Shapefile to JPEG Conversion
linkTitle: 도형 파일에서 JPEG 변환
weight: 10
url: /ko/net/viewer/shapefile-to-jpeg/
description: Learn how to convert shapefiles to JPEGs using the .NET viewer.
aliases: [shapefile, jpeg, conversion, .NET]
---

## Converting Shapefiles to JPEG with the .NET Viewer

This guide explains how to convert shapefiles to JPEG images using the .NET viewer library. This process is useful for creating raster representations of vector data for various applications like web mapping and image processing.

### Prerequisites

Before you begin, ensure you have the following:

*   The .NET viewer library installed in your project.
*   A valid shapefile (.shp) that you want to convert.
*   Basic knowledge of C# or another .NET language.

### Code Example

Here's a simple code example demonstrating how to convert a shapefile to a JPEG image:

```csharp
// This is an example, adjust paths and parameters as needed.
using NetMapViewer;
using System.Drawing;
using System.IO;

public class ShapefileToJpegConverter
{
    public static void ConvertShapefileToJpeg(string shapefilePath, string jpegFilePath)
    {
        try
        {
            // Create a new MapView object.
            MapView mapView = new MapView();

            // Load the shapefile.
            mapView.Shapes = ShapefileLoader.LoadShapefile(shapefilePath);

            // Render the map to a Bitmap.
            Bitmap bitmap = mapView.Render(new Size(500, 500));

            // Save the Bitmap as a JPEG file.
            bitmap.Save(jpegFilePath, System.Drawing.Imaging.ImageFormat.Jpeg);

            Console.WriteLine($"Successfully converted {shapefilePath} to {jpegFilePath}");
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Error converting shapefile: {ex.Message}");
        }
    }
}
```

### Explanation

1.  **Include Namespaces:** The code starts by including the necessary namespaces for map viewing and file I/O operations.
2.  **Create MapView Object:** A `MapView` object is created to represent the map view.
3.  **Load Shapefile:** The `ShapefileLoader.LoadShapefile()` method loads the shapefile data into the `mapView.Shapes` property.
4.  **Render to Bitmap:** The `mapView.Render()` method renders the map content onto a `Bitmap` object with specified dimensions (500x500 in this example). You can adjust these dimensions as needed.
5.  **Save as JPEG:** Finally, the `bitmap.Save()` method saves the rendered bitmap as a JPEG file at the specified path.

### Customization Options

*   **Map Extent and Center:** Control the visible area of the map by setting the extent and center coordinates in the `MapView` object before rendering.
*   **Zoom Level:** Adjust the zoom level to control the detail displayed in the resulting image.
*   **Symbolization:** Customize the appearance of features (e.g., color, size, outline) using symbolizers within the `MapView`.
*   **Resolution:** Change the dimensions passed to the `Render` method to adjust the resolution of the output JPEG.  Larger sizes will result in higher-resolution images but also larger file sizes.
*   **Error Handling:** Implement more robust error handling to gracefully handle potential issues like invalid shapefiles or file access problems.

### Troubleshooting

*   **Shapefile Not Found:** Verify that the path to the shapefile is correct and accessible.
*   **Invalid Shapefile Format:** Ensure that the shapefile is not corrupted and follows the standard format.
*   **Rendering Errors:** Check for any issues with the map view configuration or symbolization settings.  Inspect the exception message for more details.
*   **File Access Permissions:** Make sure your application has the necessary permissions to write to the specified output directory.

### Conclusion

This guide provides a basic framework for converting shapefiles to JPEG images using the .NET viewer library. By customizing the rendering parameters and symbolization options, you can create high-quality raster representations of your vector data for various applications.
---
