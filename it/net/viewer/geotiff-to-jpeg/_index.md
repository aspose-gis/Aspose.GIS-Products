---
title: GeoTIFF to JPEG Conversion
url: /it/net/viewer/geotiff-to-jpeg/
weight: 10
layout: ""
---

## Converting GeoTIFF to JPEG with .NET

This guide explains how to convert GeoTIFF files to JPEG format using C# and the Rasterizer library.  The Rasterizer library provides a simple and efficient way to perform raster data manipulation, including format conversion.

### Prerequisites

*   **Rasterizer Library:** Install the Rasterizer NuGet package in your .NET project.
    ```bash
    Install-Package Rasterizer
    ```
*   **.NET Development Environment:**  A suitable .NET development environment (e.g., Visual Studio).

### Code Example

Here's a basic C# code snippet demonstrating the conversion process:

```csharp
using Rasterizer;
using System;
using System.IO;

public class GeoTiffToJpegConverter
{
    public static void ConvertGeoTIFFtoJPEG(string geoTiffFilePath, string jpegFilePath)
    {
        // Check if the input file exists
        if (!File.Exists(geoTiffFilePath))
        {
            throw new FileNotFoundException("GeoTIFF file not found.", geoTiffFilePath);
        }

        try
        {
            using (var raster = Rasterizer.Open(geoTiffFilePath))
            {
                // Save the raster as JPEG
                raster.Save(jpegFilePath, Rasterizer.Formats.Jpeg);
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Error converting GeoTIFF to JPEG: {ex.Message}");
        }
    }

    public static void Main(string[] args)
    {
        // Example usage
        string geoTiffFilePath = "path/to/your/geotiff_file.tif"; // Replace with your GeoTIFF file path
        string jpegFilePath = "path/to/output/jpeg_file.jpg";   // Replace with your desired JPEG output path

        ConvertGeoTIFFtoJPEG(geoTiffFilePath, jpegFilePath);
    }
}
```

**Explanation:**

1.  **Import Namespaces:** The code imports the necessary namespaces from the Rasterizer library and standard .NET libraries.
2.  **`ConvertGeoTIFFtoJPEG` Function:** This function takes the input GeoTIFF file path and the output JPEG file path as arguments.
3.  **File Existence Check:** It verifies that the input GeoTIFF file exists before attempting to open it.
4.  **Rasterizer Object Creation:** A `Rasterizer` object is created by opening the GeoTIFF file using `Rasterizer.Open()`. This loads the raster data into memory.
5.  **Saving as JPEG:** The `raster.Save()` method saves the raster data to a JPEG file, specifying `Rasterizer.Formats.Jpeg` as the output format.
6.  **Error Handling:** A `try-catch` block is used to handle potential exceptions during the conversion process and provide informative error messages.
7.  **Example Usage (in `Main`):** The `Main` function provides an example of how to use the `ConvertGeoTIFFtoJPEG` function, including placeholder file paths that you should replace with your actual file locations.

### Error Handling

The code includes basic error handling to check for file existence and catch exceptions during conversion.  For production environments, consider implementing more robust error logging and reporting mechanisms.

### Advanced Options

*   **Resampling:** You can control the resampling method used during conversion by specifying a `Rasterizer.Resample` value in the `raster.Save()` method.
*   **Compression Level:** Adjust the JPEG compression level to balance file size and image quality.  Refer to the Rasterizer documentation for details on available options.
*   **Color Correction:** Apply color correction or other image processing techniques before saving as JPEG.

### Troubleshooting

*   **File Not Found:** Ensure that the input GeoTIFF file path is correct and that the file exists at the specified location.
*   **Rasterizer Library Issues:** Verify that the Rasterizer library is installed correctly in your project.  Check for any version conflicts or compatibility issues.
*   **Corrupted GeoTIFF File:** The GeoTIFF file might be corrupted. Try opening it with another GIS software to confirm its validity.

### Conclusion

This guide provides a simple and effective way to convert GeoTIFF files to JPEG format using C# and the Rasterizer library.  By following these steps, you can easily integrate this functionality into your .NET applications.
---
