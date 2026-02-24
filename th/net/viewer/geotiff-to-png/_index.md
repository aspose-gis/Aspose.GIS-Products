---
title: GeoTIFF to PNG Converter
url: /th/geotiff-to-png/
weight: 10
layout: single
draft: false
toc: true
---

## Convert GeoTIFF to PNG with .NET Viewer

This guide explains how to convert GeoTIFF files to PNG format using the .NET viewer.  The process involves loading the GeoTIFF image, specifying the desired output parameters (like resolution and color palette), and saving it as a PNG file.

### Prerequisites

*   **.NET SDK:** Ensure you have the .NET SDK installed on your system. You can download it from [https://dotnet.microsoft.com/download](https://dotnet.microsoft.com/download).
*   **.NET Viewer Library:**  You'll need to include the .NET viewer library in your project. This library provides the necessary functions for GeoTIFF loading and PNG conversion.

### Code Example

Here’s a basic code example demonstrating the conversion process:

```csharp
// Load the GeoTIFF image
using (var image = Viewer.Open("path/to/your/geotiff.tif"))
{
    // Set output parameters (optional)
    image.Resolution = 100; // DPI
    image.Palette = ImagePalette.TrueColor;

    // Save as PNG
    image.Save("path/to/output/pngfile.png", ImageFormat.Png);
}
```

**Explanation:**

*   `Viewer.Open()`:  Loads the GeoTIFF file from the specified path. Replace `"path/to/your/geotiff.tif"` with the actual path to your GeoTIFF file.
*   `image.Resolution`: Sets the resolution of the output PNG image in DPI (dots per inch). This is optional, but it allows you to control the quality and size of the resulting PNG.
*   `image.Palette`: Specifies the color palette for the output PNG.  `ImagePalette.TrueColor` uses a full-color palette. Other options might be available depending on your viewer library's capabilities.
*   `image.Save()`: Saves the image as a PNG file to the specified path. Replace `"path/to/output/pngfile.png"` with the desired output path and filename.

### Error Handling

It’s crucial to implement error handling in your code to gracefully handle potential issues such as invalid file paths, unsupported GeoTIFF formats, or insufficient memory.  Here's an example of how you might incorporate basic error handling:

```csharp
try
{
    using (var image = Viewer.Open("path/to/your/geotiff.tif"))
    {
        image.Resolution = 100;
        image.Palette = ImagePalette.TrueColor;
        image.Save("path/to/output/pngfile.png", ImageFormat.Png);
    }
}
catch (Exception ex)
{
    Console.WriteLine($"An error occurred: {ex.Message}");
    // Log the error or take other appropriate actions
}
```

### Advanced Options

*   **Cropping:**  You can crop the GeoTIFF image before converting it to PNG using `image.Crop(x, y, width, height)`.
*   **Resampling:** Different resampling algorithms (e.g., bilinear, bicubic) can be used when changing the resolution of the image. Refer to your viewer library's documentation for available options.
*   **Compression Level:**  You might be able to control the compression level of the PNG file using `image.PngCompressionLevel`.

### Troubleshooting

*   **File Not Found:** Double-check that the GeoTIFF file exists at the specified path and that you have the necessary permissions to access it.
*   **Unsupported Format:**  Ensure that the GeoTIFF file is a valid and supported format by the .NET viewer library.
*   **Memory Issues:** Large GeoTIFF files can consume significant memory during conversion. If you encounter memory issues, try reducing the resolution or processing the image in smaller tiles.

### Conclusion

This guide provides a basic overview of how to convert GeoTIFF files to PNG format using the .NET viewer.  By understanding the core concepts and incorporating error handling, you can create robust and reliable solutions for converting your geospatial data.
---
