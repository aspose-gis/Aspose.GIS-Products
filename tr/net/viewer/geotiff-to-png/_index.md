---
title: GeoTIFF to PNG Conversion
linkTitle: GeoTiff’i PNG’ye Dönüştürme
weight: 10
url: /tr/net/viewer/geotiff-to-png/
description: Convert GeoTIFF files to PNG format.
açıklama: GeoTiff dosyalarını PNG formatına dönüştürün.
---

## Converting GeoTIFF to PNG with the .NET Viewer

## .NET Görüntüleyici ile GeoTiff’i PNG’ye Dönüştürme

This guide explains how to convert GeoTIFF files to PNG format using the .NET viewer library.

Bu kılavuz, .NET görüntüleyici kitaplığını kullanarak GeoTiff dosyalarını PNG formatına nasıl dönüştüreceğinizi açıklar.

### Prerequisites

### Önkoşullar

*   .NET SDK
*   The .NET viewer library

*   .NET SDK
*   .NET görüntüleyici kitaplığı

### Code Example

### Kod Örneği

```csharp
// Sample code to convert a GeoTIFF file to PNG format
// GeoTiff dosyasını PNG formatına dönüştürmek için örnek kod

using NetViewer;
using System.Drawing;
using System.Drawing.Imaging;

public class GeotiffToPngConverter
{
    public static void ConvertGeotiffToPng(string geotiffFilePath, string pngFilePath)
    {
        try
        {
            // Load the GeoTIFF file
            // GeoTiff dosyasını yükle
            var raster = Raster.FromFile(geotiffFilePath);

            // Get the image data from the raster
            // Rasterden görüntü verilerini al
            Bitmap bitmap = raster.GetBitmap();

            // Save the image as a PNG file
            // Görüntüyü PNG dosyası olarak kaydet
            bitmap.Save(pngFilePath, ImageFormat.Png);
        }
        catch (Exception ex)
        {
            // Handle any exceptions that may occur
            // Olabilecek herhangi bir istisnayı işleyin
            Console.WriteLine("Error converting GeoTIFF to PNG: " + ex.Message);
        }
    }
}
```

### Explanation

### Açıklama

1.  **Load the GeoTIFF file:** This line loads the GeoTIFF file into a `Raster` object.
2.  **Get the image data from the raster:** This line extracts the image data from the `Raster` object and creates a `Bitmap` object.
3.  **Save the image as a PNG file:** This line saves the `Bitmap` object as a PNG file.

1.  **GeoTiff dosyasını yükle:** Bu satır, GeoTiff dosyasını bir `Raster` nesnesine yükler.
2.  **Rasterden görüntü verilerini al:** Bu satır, `Raster` nesnesinden görüntü verilerini çıkarır ve bir `Bitmap` nesnesi oluşturur.
3.  **Görüntüyü PNG dosyası olarak kaydet:** Bu satır, `Bitmap` nesnesini bir PNG dosyası olarak kaydeder.

### Error Handling

### Hata Yönetimi

The code includes a `try-catch` block to handle any exceptions that may occur during the conversion process.  If an exception occurs, an error message is printed to the console.

Kod, dönüşüm işlemi sırasında ortaya çıkabilecek herhangi bir istisnayı işlemek için bir `try-catch` bloğu içerir. Bir istisna oluşursa, hata mesajı konsola yazdırılır.

### Conclusion

### Sonuç

This guide has shown you how to convert GeoTIFF files to PNG format using the .NET viewer library.  You can use this code as a starting point for your own GeoTIFF conversion projects.

Bu kılavuz, .NET görüntüleyici kitaplığını kullanarak GeoTiff dosyalarını PNG formatına nasıl dönüştüreceğinizi göstermiştir. Bu kodu kendi GeoTiff dönüşüm projeleriniz için bir başlangıç noktası olarak kullanabilirsiniz.
---
