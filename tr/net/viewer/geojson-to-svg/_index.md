---
title: GeoJSON to SVG Conversion
linkTitle: GeoJSON’u SVG’ye Dönüştürme
weight: 10
url: /tr/net/viewer/geojson-to-svg/
aliases: [geojson2svg, geojson-to-svg]
description: Convert GeoJSON data to Scalable Vector Graphics (SVG) format.
açıklama: Verileri Ölçeklenebilir Vektör Grafikleri (SVG) biçimine dönüştürün.
---

## Overview
geniş bakış
This tool converts GeoJSON data into SVG format, allowing for easy visualization and manipulation of geographic data in web applications.
Bu araç, GeoJSON verilerini SVG biçimine dönüştürerek coğrafi verilerin web uygulamalarında kolayca görselleştirilmesini ve üzerinde işlem yapılmasını sağlar.

## Usage
kullanım
1.  **Input GeoJSON Data:** Provide a valid GeoJSON file or data structure as input.
    **GeoJSON Verisi Girişi:** Geçerli bir GeoJSON dosyası veya veri yapısı sağlayın.
2.  **Customization Options:** Adjust parameters such as stroke color, fill color, and line width to customize the appearance of the SVG output.
    **Özelleştirme Seçenekleri:** Çizgi rengi, dolgu rengi ve çizgi genişliği gibi parametreleri ayarlayarak SVG çıktısının görünümünü özelleştirin.
3.  **Generate SVG:** The tool processes the GeoJSON data and generates an SVG file or string representing the geographic features.
    **SVG Oluşturma:** Araç, GeoJSON verisini işler ve coğrafi özellikleri temsil eden bir SVG dosyası veya dize oluşturur.

## Parameters
parametreler
*   `geojson`: The GeoJSON data to convert.
    `geojson`: Dönüştürülecek GeoJSON verisi.
*   `strokeColor`: Color of the stroke (outline) of the features. Default is black.
    `strokeColor`: Özelliklerin çizgisinin rengi. Varsayılan olarak siyahtır.
*   `fillColor`: Color of the fill of the features. Default is white.
    `fillColor`: Özelliklerin dolgusunun rengi. Varsayılan olarak beyazdır.
*   `lineWidth`: Width of the stroke (outline) of the features. Default is 1.
    `lineWidth`: Özelliklerin çizgisinin genişliği. Varsayılan olarak 1'dir.
*   `outputFormat`: The desired output format, either "file" or "string". Default is "file".
    `outputFormat`: İstediğiniz çıktı biçimi, "dosya" veya "dize" olabilir. Varsayılan olarak "dosya"dır.

## Example
örnek
```javascript
// Sample GeoJSON data
const geojson = {
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [[[-122.4, 37.8], [-122.3, 37.8], [-122.3, 37.7], [-122.4, 37.7], [-122.4, 37.8]]]
      },
      "properties": {
        "name": "Golden Gate Park"
      }
    }
  ]
};

// Convert GeoJSON to SVG with custom styling
const svg = convertGeoJsonToSvg(geojson, {
  strokeColor: "blue",
  fillColor: "lightgreen",
  lineWidth: 2
});

// Display the generated SVG
console.log(svg);
```
/*
Örnek GeoJSON verisi
const geojson = {
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [[[-122.4, 37.8], [-122.3, 37.8], [-122.3, 37.7], [-122.4, 37.7], [-122.4, 37.8]]]
      },
      "properties": {
        "name": "Golden Gate Park"
      }
    }
  ]
};

// Özel stillendirmeyle GeoJSON'u SVG'ye dönüştürün
const svg = convertGeoJsonToSvg(geojson, {
  strokeColor: "blue",
  fillColor: "lightgreen",
  lineWidth: 2
});

// Oluşturulan SVG'yi görüntüleyin
console.log(svg);
*/

## Output
çıktı
The tool generates an SVG file or string containing the geographic features represented in the GeoJSON data. The appearance of the features can be customized using the parameters described above.
Araç, GeoJSON verilerinde temsil edilen coğrafi özellikleri içeren bir SVG dosyası veya dize oluşturur. Özelliklerin görünümü, yukarıda açıklanan parametreler kullanılarak özelleştirilebilir.

## Limitations
sınırlamalar
*   The tool may have limitations in handling complex GeoJSON data structures.
    Araç, karmaşık GeoJSON veri yapılarını işleme konusunda sınırlamalara sahip olabilir.
*   Large GeoJSON files may result in slow processing times.
    Büyük GeoJSON dosyaları yavaş işleme sürelerine neden olabilir.

---
