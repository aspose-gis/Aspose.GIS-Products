---
title: GeoTIFF to JPEG Conversion
url: /vi/net/viewer/geotiff-to-jpeg/
weight: 10
layout: ""
---

## Converting GeoTIFF to JPEG

This guide explains how to convert GeoTIFF files to JPEG format using our .NET viewer.  The process involves extracting the raster data from the GeoTIFF and then saving it as a JPEG image.

### Prerequisites

*   **.NET SDK:** Make sure you have the .NET SDK installed on your system.
*   **GeoTIFF Library:** You'll need a library to read GeoTIFF files.  GDAL/OGR is a popular choice, but there are other options available.
*   **Image Processing Library:** A library for image processing and saving as JPEG (e.g., System.Drawing).

### Code Example

```csharp
// This code snippet demonstrates the basic steps involved in converting a GeoTIFF to JPEG.
// Replace placeholders with your actual file paths and settings.

using Geospatial; // Assuming you're using a library like Geospatial.NET
using System.Drawing;
using System.Drawing.Imaging;

public class GeotiffToJpegConverter
{
    public void Convert(string geotiffPath, string jpegOutputPath)
    {
        try
        {
            // 1. Open the GeoTIFF file
            Raster raster = Raster.Open(geotiffPath);

            // 2. Extract the raster data as a byte array
            byte[] rasterData = raster.GetPixelData();

            // 3. Create a Bitmap object from the raster data
            Bitmap bitmap = new Bitmap(raster.Width, raster.Height, PixelFormat.Format8bppIndexed);

            // 4. Save the Bitmap as a JPEG file
            bitmap.Save(jpegOutputPath, ImageFormat.Jpeg);
        }
        catch (Exception ex)
        {
            Console.WriteLine("Error converting GeoTIFF to JPEG: " + ex.Message);
        }
    }
}
```

### Explanation

1.  **Open the GeoTIFF file:** This step uses a library like Geospatial.NET to open and read the GeoTIFF file.
2.  **Extract raster data:** The pixel data is extracted from the GeoTIFF as a byte array.
3.  **Create Bitmap object:** A `Bitmap` object is created using the extracted raster data. This represents the image that will be saved as JPEG.
4.  **Save as JPEG:** The `Bitmap` object is saved to a file with the `.jpeg` extension, using the `ImageFormat.Jpeg` option.

### Considerations

*   **Error Handling:** Implement robust error handling to catch potential issues during file opening, data extraction, and image saving.
*   **Performance:** For large GeoTIFF files, consider optimizing the process for performance.  This might involve using multi-threading or other techniques.
*   **Color Management:** If your GeoTIFF contains color information, ensure that it is handled correctly during the conversion to JPEG.
*   **Compression:** Adjust the JPEG compression settings to balance image quality and file size.

### Troubleshooting

*   **File Not Found:** Verify that the input GeoTIFF file exists at the specified path.
*   **Unsupported Format:** Ensure that the GeoTIFF library you are using supports the specific GeoTIFF format.
*   **Insufficient Permissions:** Make sure your application has the necessary permissions to read the input file and write the output file.

---
