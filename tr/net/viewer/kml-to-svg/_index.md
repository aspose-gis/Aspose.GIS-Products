---
title: KML to SVG Conversion
linkTitle: KML'den SVG'ye Dönüştürme
weight: 10
url: /tr/net/viewer/kml-to-svg/
aliases: [KML to SVG, KML SVG, Convert KML to SVG]
---

## Overview

This document describes how to convert KML (Keyhole Markup Language) files to SVG (Scalable Vector Graphics) format using the .NET viewer.  Bu belge, .NET görüntüleyiciyi kullanarak KML (Anahtar Delik İşaretleme Dili) dosyalarını SVG (Ölçeklenebilir Vektör Grafikleri) biçimine nasıl dönüştüreceğinizi açıklar.

## Prerequisites

*   .NET SDK installed
*   A KML file to convert
*   The .NET viewer library

    *   Install the necessary NuGet packages: `Net.Viewer`
        *   Yüklenen gerekli NuGet paketleri: `Net.Viewer`

## Conversion Process

1.  **Load the KML file:** Use the `KmlFile.FromFile()` method to load the KML file into a `KmlFile` object.  KML dosyasını yüklemek için: KML dosyasını bir `KmlFile` nesnesine yüklemek için `KmlFile.FromFile()` yöntemini kullanın.
2.  **Convert to SVG:** Use the `ConvertToSvg()` method on the `KmlFile` object to generate the SVG content.  SVG'ye dönüştürmek için: SVG içeriğini oluşturmak için `KmlFile` nesnesindeki `ConvertToSvg()` yöntemini kullanın.
3.  **Save the SVG file:** Save the generated SVG content to a file using standard file I/O methods.  SVG dosyasını kaydetmek için: Oluşturulan SVG içeriğini standart dosya G/Ç yöntemlerini kullanarak bir dosyaya kaydedin.

## Code Example

```csharp
// Load the KML file
KmlFile kml = KmlFile.FromFile("path/to/your/file.kml");

// Convert to SVG
string svgContent = kml.ConvertToSvg();

// Save the SVG file
File.WriteAllText("path/to/your/output.svg", svgContent);
```

## Customization Options

The `ConvertToSvg()` method accepts an optional `SvgOptions` object that allows you to customize the conversion process.  `ConvertToSvg()` yöntemi, dönüşüm sürecini özelleştirmenize olanak tanıyan isteğe bağlı bir `SvgOptions` nesnesi kabul eder.

*   **Scale:** Adjust the scale of the SVG output. Ölçeği ayarlayın: SVG çıktısının ölçeğini ayarlayın.
*   **Rotation:** Rotate the SVG output. Rotasyonu ayarlayın: SVG çıktısını döndürün.
*   **Simplify:** Simplify the geometry of the KML features. Geometriyi basitleştirin: KML özelliklerinin geometrisini basitleştirin.

## Troubleshooting

*   **Invalid KML file:** Ensure that the KML file is valid and well-formed. Geçersiz KML dosyası: KML dosyasının geçerli ve iyi biçimlendirilmiş olduğundan emin olun.
*   **Large KML files:** Converting very large KML files may take a significant amount of time and memory. Çok büyük KML dosyaları: Çok büyük KML dosyalarını dönüştürmek önemli miktarda zaman ve bellek alabilir. Consider simplifying the geometry or splitting the file into smaller chunks. Geometriyi basitleştirmeyi veya dosyayı daha küçük parçalara ayırmayı düşünün.
*   **Unsupported features:** Some KML features may not be supported in SVG format. Desteklenmeyen özellikler: Bazı KML özellikleri SVG biçiminde desteklenmeyebilir.

## Further Reading

*   [KML Reference](https://developers.google.com/kml/documentation/)
*   [SVG Specification](https://www.w3.org/TR/svg11/)
    *   [KML Referansı](https://developers.google.com/kml/documentation/)
    *   [SVG Özelliği](https://www.w3.org/TR/svg11/)

---
