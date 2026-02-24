---
title: Shapefile to SVG Conversion
linkTitle: Şekil Dosyasını SVG'ye Dönüştürme
weight: 10
url: /tr/net/viewer/shapefile-to-svg/
description: Learn how to convert shapefiles to scalable vector graphics (SVG) using .NET.
açıklama: .NET kullanarak şekil dosyalarını ölçeklenebilir vektör grafiklerine (SVG) nasıl dönüştüreceğinizi öğrenin.
---

## Introduction
Giriş

This guide explains how to convert Shapefile data into SVG format using a .NET application. This allows for easy viewing and manipulation of geospatial data within web browsers or other applications that support SVG.

Bu kılavuz, bir .NET uygulaması kullanarak Şekil dosyası verilerini SVG biçimine nasıl dönüştüreceğinizi açıklar. Bu, coğrafi verilerin web tarayıcılarında veya SVG'yi destekleyen diğer uygulamalarda kolayca görüntülenebilmesini ve işlenebilmesini sağlar.

## Prerequisites
Ön Koşullar

*   A .NET development environment (e.g., Visual Studio)
    Bir .NET geliştirme ortamı (örneğin, Visual Studio)
*   The NetTopologySuite library installed via NuGet
    NuGet aracılığıyla NetTopologySuite kütüphanesinin kurulu olması
*   Shapefile data to convert
    Dönüştürülecek şekil dosyası verisi

## Installation
Kurulum

1.  Create a new .NET console application or web project.
    Yeni bir .NET konsol uygulaması veya web projesi oluşturun.
2.  Install the NetTopologySuite NuGet package:
    NetTopologySuite NuGet paketini kurun:

```bash
Install-Package NetTopologySuite
```

## Code Example
Kod Örneği

Here's a basic example of how to convert a Shapefile to SVG using .NET:

İşte .NET kullanarak bir Şekil dosyasını SVG'ye dönüştürmenin temel bir örneği:

```csharp
// This code snippet demonstrates the conversion process.
// Bu kod parçacığı dönüşüm sürecini göstermektedir.
using NetTopologySuite.Shapefile;
using System;
using System.IO;
using System.Xml;

public class ShapefileToSvgConverter
{
    public static void Convert(string shapefilePath, string svgFilePath)
    {
        try
        {
            // Open the Shapefile
            var factory = new ShapefileReaderFactory();
            using (Shapefile stream = factory.Open(shapefilePath))
            {
                // Create an XML document for the SVG
                XmlDocument doc = new XmlDocument();
                XmlElement svgElement = doc.CreateElement("svg");
                svgElement.SetAttribute("xmlns", "http://www.w3.org/2000/svg");
                doc.AppendChild(svgElement);

                // Iterate through the Shapefile records
                foreach (ShapefileFeatureClass feature in stream.ShapeType)
                {
                    if (feature is Polygon polygon)
                    {
                        XmlElement pathElement = doc.CreateElement("path");
                        string dAttribute = "M" + string.Join(" L", polygon.Points.Select(p => $"{p.X} {p.Y}"));
                        pathElement.SetAttribute("d", dAttribute);
                        svgElement.AppendChild(pathElement);
                    }
                }

                // Save the SVG to a file
                doc.Save(svgFilePath);
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Error: {ex.Message}");
        }
    }

    public static void Main(string[] args)
    {
        Convert("path/to/your/shapefile.shp", "output.svg");
    }
}
```

## Explanation
Açıklama

*   The code opens the specified Shapefile using `ShapefileReaderFactory`.
    Kod, `ShapefileReaderFactory` kullanarak belirtilen Şekil dosyasını açar.
*   It creates an XML document to represent the SVG file.
    SVG dosyasını temsil etmek için bir XML belgesi oluşturur.
*   The code iterates through each feature in the Shapefile and converts polygon geometries into SVG path data.
    Kod, Şekil dosyasındaki her özellik üzerinde yineleme yapar ve çokgen geometrilerini SVG yol verilerine dönüştürür.
*   Finally, it saves the generated XML document as an SVG file.
    Son olarak, oluşturulan XML belgesini bir SVG dosyası olarak kaydeder.

## Customization
Özelleştirme

You can customize this code to handle different Shapefile feature types (points, lines, polygons) and add attributes to the SVG elements.  Consider adding error handling for invalid shapefiles or unsupported geometries.

Bu kodu farklı Şekil dosyası özellik türlerini (noktalar, çizgiler, çokgenler) işleyecek ve SVG öğelerine öznitelikler ekleyecek şekilde özelleştirebilirsiniz. Geçersiz şekil dosyaları veya desteklenmeyen geometriler için hata işlemeyi de düşünün.

## Conclusion
Sonuç

This guide provides a basic framework for converting Shapefiles to SVG using .NET.  By extending this example, you can create more sophisticated tools for visualizing and manipulating geospatial data.

Bu kılavuz, Şekil dosyalarını SVG'ye dönüştürmek için .NET kullanarak temel bir çerçeve sağlar. Bu örneği genişleterek coğrafi verileri görselleştirmek ve işlemek için daha karmaşık araçlar oluşturabilirsiniz.
---
