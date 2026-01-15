---
title: GeoTIFF to PNG Conversion
url: /vi/net/viewer/geotiff-to-png/
weight: 10
layout: ""
---

## Converting GeoTIFF to PNG with .NET

This guide explains how to convert GeoTIFF files to PNG format using C# and the RasterGis package. This process is essential for displaying raster data in web applications or other environments that require PNG images.

### Prerequisites

Before you begin, ensure you have the following:

*   **Visual Studio:**  A development environment for writing and running C# code.
*   **.NET SDK:** The .NET Software Development Kit.
*   **RasterGis Package:** Install the RasterGis package via NuGet.

    ```bash
    Install-Package RasterGis
    ```

### Code Example

Here's a basic example of how to convert a GeoTIFF file to PNG:

```csharp
using System;
using NetTopologySuite.Geometries;
using RasterGis;

public class GeotiffToPngConverter
{
    public static void ConvertGeoTiffToPng(string inputFilePath, string outputFilePath)
    {
        // Khởi tạo đối tượng RasterGis
        RasterGis.RasterGis rasterGis = new RasterGis.RasterGis();

        try
        {
            // Đọc dữ liệu GeoTIFF từ file đầu vào
            rasterGis.Open(inputFilePath, "");

            // Lưu dữ liệu dưới dạng PNG sang file đầu ra
            rasterGis.Save(outputFilePath, "PNG", "");

            // Đóng file GeoTIFF
            rasterGis.Close();
        }
        catch (Exception ex)
        {
            Console.WriteLine("Lỗi khi chuyển đổi: " + ex.Message);
        }
    }

    public static void Main(string[] args)
    {
        // Thay thế bằng đường dẫn file thực tế của bạn
        string inputGeoTiffPath = "path/to/your/input.tif";
        string outputPngPath = "path/to/your/output.png";

        ConvertGeoTiffToPng(inputGeoTiffPath, outputPngPath);
    }
}
```

### Explanation

1.  **Include RasterGis Namespace:** The code starts by including the necessary namespace for using RasterGis functionalities.
2.  **Create RasterGis Object:** An instance of the `RasterGis` class is created to handle raster data operations.
3.  **Open GeoTIFF File:** The `rasterGis.Open()` method opens the specified GeoTIFF file for reading. The second argument represents a password, which is left empty in this case as we assume the file isn't password-protected.
4.  **Save to PNG:** The `rasterGis.Save()` method saves the raster data to a PNG file at the given output path. The first argument specifies the output file path, the second argument defines the image format ("PNG"), and the third argument is reserved for additional options (left empty here).
5.  **Close File:** Finally, `rasterGis.Close()` closes the GeoTIFF file to release resources.
6.  **Error Handling:** A `try-catch` block is used to handle potential exceptions during the conversion process and display an error message if something goes wrong.

### Customization Options

The RasterGis package offers various customization options for the conversion process:

*   **Color Palette:** You can specify a color palette to be applied to the raster data before saving it as PNG.
*   **Resampling Method:** Choose different resampling methods to control the quality and size of the output image.
*   **Compression Level:** Adjust the compression level for the PNG file to balance between file size and processing time.

Refer to the RasterGis documentation for detailed information on these options: [https://rastergis.net/](https://rastergis.net/)

### Troubleshooting

*   **File Not Found:** Ensure that the input GeoTIFF file exists at the specified path.
*   **Insufficient Permissions:** Verify that your application has the necessary permissions to read the input file and write the output file.
*   **RasterGis Errors:** Check the RasterGis documentation for specific error codes and troubleshooting steps.

### Conclusion

This guide provides a basic framework for converting GeoTIFF files to PNG format using C# and the RasterGis package. By customizing the conversion options, you can tailor the process to meet your specific requirements.
---
