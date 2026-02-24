---
title: Перетворення Shapefile у JPEG
url: /uk/net/viewer/shapefile-to-jpeg/
weight: 10
layout: single
draft: false
description: Convert shapefiles to JPEGs using the .NET viewer library.
---

## Converting Shapefiles to JPEGs with the .NET Viewer Library

This guide explains how to convert shapefiles to JPEG images using our .NET viewer library.  The process involves rendering the shapefile data within the viewer and then saving the rendered output as a JPEG file.

### Prerequisites

*   **.NET SDK:** Ensure you have the .NET SDK installed on your system.
*   **Viewer Library:** Download or install the .NET viewer library from our repository.  Refer to the installation instructions for detailed steps.
*   **Shapefile:** Have a shapefile (.shp) ready for conversion.

### Code Example

Here's a basic code example demonstrating how to convert a shapefile to a JPEG:

```csharp
// Цей код демонструє перетворення Shapefile у JPEG за допомогою .NET бібліотеки переглядача.
using NetMapViewer;
using System.Drawing;
using System.IO;

public class ShapefileToolToJpegConverter
{
    public static void ConvertShapefileToolToJpeg(string shapefilePath, string jpegFilePath)
    {
        try
        {
            // Створення об'єкта переглядача
            var viewer = new MapViewer();

            // Завантаження Shapefile
            viewer.LoadShapefile(shapefilePath);

            // Рендеринг карти у Bitmap
            Bitmap bitmap = viewer.Render();

            // Збереження Bitmap як JPEG
            bitmap.Save(jpegFilePath, System.Drawing.Imaging.ImageFormat.Jpeg);

            Console.WriteLine($"Shapefile converted to JPEG successfully: {jpegFilePath}");
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Error converting Shapefile to JPEG: {ex.Message}");
        }
    }

    public static void Main(string[] args)
    {
        // Вкажіть шляхи до вашого Shapefile та бажаного місця збереження JPEG
        string shapefilePath = "path/to/your/shapefile.shp";
        string jpegFilePath = "path/to/output/image.jpeg";

        ConvertShapefileToolToJpeg(shapefilePath, jpegFilePath);
    }
}
```

### Explanation

1.  **Include Namespaces:** The code includes necessary namespaces for map viewer functionality and file I/O operations.
2.  **Create MapViewer Object:** An instance of the `MapViewer` class is created to handle shapefile rendering.
3.  **Load Shapefile:** The `LoadShapefile()` method loads the specified shapefile into the viewer. Replace `"path/to/your/shapefile.shp"` with the actual path to your shapefile.
4.  **Render Map:** The `Render()` method generates a bitmap representation of the map based on the loaded shapefile data.
5.  **Save as JPEG:** The `bitmap.Save()` method saves the rendered bitmap as a JPEG image at the specified file path. Replace `"path/to/output/image.jpeg"` with your desired output location and filename.
6.  **Error Handling:** A `try-catch` block is used to handle potential exceptions during the conversion process, providing informative error messages if something goes wrong.

### Customization Options

*   **Map Projection:** You can set the map projection using the `viewer.Projection` property before rendering.
*   **Rendering Options:**  Adjust rendering options such as color schemes, line widths, and font sizes to customize the appearance of the output JPEG. Refer to the library's documentation for available options.
*   **Resolution:** Control the resolution of the rendered image by adjusting the `viewer.Width` and `viewer.Height` properties before calling `Render()`.

### Troubleshooting

*   **Shapefile Not Found:** Verify that the shapefile path is correct and accessible.
*   **Rendering Errors:** Check for any errors during rendering, which might indicate issues with the shapefile data or viewer configuration.
*   **File Access Permissions:** Ensure you have write permissions to the output directory where the JPEG file will be saved.

### Conclusion

This guide provides a basic framework for converting shapefiles to JPEGs using our .NET viewer library.  By customizing rendering options and handling potential errors, you can create high-quality map images for various applications.
---
