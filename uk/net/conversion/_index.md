---
title: C# GIS Data Conversion
url: /uk/net/conversion/
description: Convert GIS data in different formats including GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM with few lines of C# code via .NET library.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="GIS Data Conversion Via C#" h2="Convert GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Data to build cross-platform .NET mapping applications." >}}

{{% blocks/products/pf/feature-page-summary %}}


Для аналізу просторових та географічних даних, .NET GIS API полегшує створення рішень для захоплення, зберігання, управління, обробки, аналізу та представлення всіх типів географічних даних. Він не тільки завантажує різні векторні та растрові формати даних, але й легко перетворює їх в інші формати. Кілька сценаріїв рендерингу, таких як **GeoJSON to Shapefile** , **GeoJSON to topojson**, **GeoJSON to kml**, **Shapefile to GeoJSON** і багато інших. Для будь-якого застосунку географічної інформації без необхідності додаткових інструментів або програмного забезпечення, .NET GIS API має можливість працювати з великою кількістю геометричних об'єктів, простих чи складних.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON to Shapefile SHP Conversion" %}}

За допомогою лише кількох рядків коду розробники можуть конвертувати дані GeoJSON у файл Shapefile SHP. API надає [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)


{{% blocks/products/pf/feature-page-code h3="C# Code for GeoJSON to Shapefile Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert Shapefile to GeoJSON" %}}

Процес перетворення Shapefile в GeoJSON такий самий, як і описаний вище, за допомогою VectorLayer та викликаючи метод [Convert method](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) з відповідними параметрами.


{{% blocks/products/pf/feature-page-code h3="C# Code for Converting Shapefile Data to GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert KML to GeoJSON" %}}

Використовуючи метод VectorLayer.Convert з відповідними параметрами, вихідний файл KML, драйвер KML з [Drivers class](https://apireference.aspose.com/gis/net/aspose.gis/drivers), шлях до файлу GeoJSON та драйвер GeoJSON, розробники можуть легко конвертувати KML в дані GeoJSON.

{{% blocks/products/pf/feature-page-code h3="C# Code for KML to GeoJSON Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
