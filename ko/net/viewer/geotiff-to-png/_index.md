---
title: GeoTIFF to PNG Conversion
url: /ko/net/viewer/geotiff-to-png/
weight: 10
layout: ""
---

## Converting GeoTIFF to PNG with .NET Viewer

This guide explains how to convert GeoTIFF files to PNG format using the .NET Viewer library.  The process involves loading the GeoTIFF image, specifying the desired output parameters (like resolution and color correction), and saving it as a PNG file.

### Prerequisites

*   **.NET SDK:** Make sure you have the .NET SDK installed on your system.
*   **.NET Viewer Library:** Download and install the .NET Viewer library from our [releases page](https://github.com/GeotiffSharp/GeoTIFFSharp/releases).  You can also use NuGet to manage the package:

    ```bash
    Install-Package GeoTIFFSharp
    ```

### Code Example

Here's a basic code example demonstrating the conversion process:

```csharp
using GeoTIFFSharp;
using System.Drawing;
using System.DrawingImaging;

public class GeotiffToPngConverter
{
    public static void ConvertGeotiffToPng(string geotiffPath, string pngOutputPath)
    {
        // Load the GeoTIFF image
        using (var dataset = GeoDataset.Open(geotiffPath, AccessMode.Read))
        {
            // Get the first raster band
            var band = dataset.GetRasterBand(1);

            // Read the raster data as a Bitmap
            Bitmap bitmap = band.ReadBitmap();

            // Save the Bitmap as a PNG file
            bitmap.Save(pngOutputPath, ImageFormat.Png);
        }
    }
}
```

**Comment:** 이 코드는 GeoTIFF 파일을 로드하고 첫 번째 밴드를 읽어 Bitmap으로 변환한 다음 PNG 파일로 저장합니다.

### Explanation

1.  **Load the GeoTIFF image:** The `GeoDataset.Open()` method opens the specified GeoTIFF file for reading.
2.  **Get the first raster band:** GeoTIFF files can contain multiple bands (e.g., red, green, blue, infrared). This example retrieves the first band.
3.  **Read the raster data as a Bitmap:** The `band.ReadBitmap()` method reads the raster data from the selected band and creates a `Bitmap` object.
4.  **Save the Bitmap as a PNG file:** The `bitmap.Save()` method saves the `Bitmap` object to the specified output path in PNG format.

### Advanced Options

*   **Resolution Control:** You can control the resolution of the output PNG image by specifying the desired width and height when creating the `Bitmap`.
*   **Color Correction:**  GeoTIFF images often have specific color palettes or scaling factors.  You may need to apply color correction during the conversion process to achieve the desired visual appearance. This can be done using techniques like histogram equalization or custom color mapping functions.
*   **Multi-band Conversion:** To convert multi-band GeoTIFFs (e.g., RGB images), you'll need to read data from multiple bands and combine them into a single `Bitmap`.
*   **Error Handling:**  Implement robust error handling to gracefully handle cases where the GeoTIFF file is invalid or cannot be opened.

### Troubleshooting

*   **File Not Found:** Ensure that the input GeoTIFF file exists at the specified path.
*   **Invalid File Format:** Verify that the input file is a valid GeoTIFF file.  Use a hex editor to inspect the file header if necessary.
*   **Insufficient Permissions:** Make sure your application has sufficient permissions to read the input file and write the output file.
*   **Memory Issues:** Large GeoTIFF files can consume significant memory during conversion. Consider using techniques like tiling or streaming to reduce memory usage.

### Conclusion

This guide provides a basic overview of how to convert GeoTIFF files to PNG format using the .NET Viewer library.  By understanding the underlying principles and exploring advanced options, you can customize the conversion process to meet your specific needs.
---
