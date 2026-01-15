---
title: GeoJSON to JPEG Conversion
linkTitle: GeoJSON’u JPEG’e Dönüştürme
weight: 10
url: /tr/net/viewer/geojson-to-jpeg/
description: Convert GeoJSON data to JPEG images using .NET.
açıklama: .NET kullanarak GeoJSON verilerini JPEG görüntülerine dönüştürün.
---

## Overview
## Genel Bakış

This viewer allows you to convert GeoJSON data into JPEG images. You can customize the appearance of the map by adjusting various parameters such as zoom level, center coordinates, and image resolution.
Bu görüntüleyici, GeoJSON verilerini JPEG görüntülerine dönüştürmenizi sağlar. Zoom seviyesi, merkez koordinatları ve görüntü çözünürlüğü gibi çeşitli parametreleri ayarlayarak haritanın görünümünü özelleştirebilirsiniz.

## Usage
## Kullanım

1.  **Input GeoJSON Data:** Provide the GeoJSON data as a string or file path.
    **GeoJSON Verisini Giriş:** GeoJSON verisini bir dize veya dosya yolu olarak sağlayın.
2.  **Configuration Options:** Adjust parameters like zoom level, center coordinates, image resolution, and color scheme.
    **Yapılandırma Seçenekleri:** Zoom seviyesi, merkez koordinatları, görüntü çözünürlüğü ve renk düzeni gibi parametreleri ayarlayın.
3.  **Generate JPEG Image:** The viewer processes the GeoJSON data and generates a JPEG image based on your configuration.
    **JPEG Görüntüsü Oluşturun:** Görüntüleyici, GeoJSON verisini işler ve yapılandırmanıza göre bir JPEG görüntüsü oluşturur.

## Parameters
## Parametreler

*   `geojson`: The GeoJSON data as a string.
    `geojson`: Bir dize olarak GeoJSON verisi.
*   `filePath`: Path to the GeoJSON file.
    `filePath`: GeoJSON dosyasının yolu.
*   `zoom`: Zoom level of the map (default: 10).
    Haritanın zoom seviyesi (varsayılan: 10).
*   `centerLng`: Longitude of the center coordinates (default: -74.0060).
    Merkez koordinatlarının boylamı (varsayılan: -74,0060).
*   `centerLat`: Latitude of the center coordinates (default: 40.7128).
    Merkez koordinatlarının enlemi (varsayılan: 40,7128).
*   `width`: Width of the output image in pixels (default: 512).
    Çıkış görüntüsünün genişliği piksel cinsinden (varsayılan: 512).
*   `height`: Height of the output image in pixels (default: 512).
    Çıkış görüntüsünün yüksekliği piksel cinsinden (varsayılan: 512).
*   `colorScheme`: Color scheme for the map (e.g., "light", "dark").
    Harita için renk düzeni (örneğin, "açık", "koyu").

## Example
## Örnek

```csharp
// Sample GeoJSON data
// Örnek GeoJSON verisi
string geoJsonData = @"{""type"": ""FeatureCollection"", ""features"": [{""type"": ""Feature"", ""geometry"": {""type"": ""Point"", ""coordinates"": [ -74.0060, 40.7128 ]}, ""properties"": {}}]}";

// Convert GeoJSON to JPEG
// GeoJSON'u JPEG'e dönüştürün
byte[] jpegImage = await Viewer.ConvertGeoJsonToJpegAsync(geojsonData, new ConversionOptions
{
    Zoom = 12,
    CenterLng = -74.0060,
    CenterLat = 40.7128,
    Width = 1024,
    Height = 768,
    ColorScheme = "light"
});

// Save the JPEG image to a file
// JPEG görüntüsünü bir dosyaya kaydedin
File.WriteAllBytes("output.jpeg", jpegImage);
```

## Notes
## Notlar

*   Ensure that the GeoJSON data is valid and well-formed.
    GeoJSON verisinin geçerli ve iyi biçimlendirilmiş olduğundan emin olun.
*   Adjust the parameters to achieve the desired map appearance.
    İstenen harita görünümünü elde etmek için parametreleri ayarlayın.
*   The conversion process may take some time depending on the size and complexity of the GeoJSON data.
    Dönüştürme işlemi, GeoJSON verisinin boyutu ve karmaşıklığına bağlı olarak biraz zaman alabilir.
---
