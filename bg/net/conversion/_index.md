---
title: C# GIS Data Conversion
url: /bg/net/conversion/
description: Convert GIS data in different formats including GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM with few lines of C# code via .NET library.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="GIS Data Conversion Via C#" h2="Convert GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Data to build cross-platform .NET mapping applications." >}}

{{% blocks/products/pf/feature-page-summary %}}


За да анализирате пространствени и географски данни, .NET GIS API улеснява изграждането на решения за улавяне, съхранение, управление, манипулиране, анализ и представяне на всички видове географски данни. Той не само зарежда различни векторни и растерни формати на данни, но също така лесно ги преобразува в други формати. Някои от сценариите за рендиране са **GeoJSON към Shapefile** , **GeoJSON към topojson**, **GeoJSON към kml**, **Shapefile към GeoJSON** и много други. За всяко приложение за визуализиране на географска информация, без да се изискват допълнителни инструменти или софтуер, .NET GIS API има способността да работи с множество геометрични характеристики, независимо дали са прости или сложни.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON to Shapefile SHP Conversion" %}}

Само с няколко реда код разработчиците могат да преобразуват GeoJSON данни в Shapefile SHP файл. API предоставя [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)


{{% blocks/products/pf/feature-page-code h3="C# Code for GeoJSON to Shapefile Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert Shapefile to GeoJSON" %}}

Процесът на преобразуване на Shapefile в GeoJSON е същият като горния, чрез използване на VectorLayer и извикване на [Convert method](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) с подходящите параметри.


{{% blocks/products/pf/feature-page-code h3="C# Code for Converting Shapefile Data to GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert KML to GeoJSON" %}}

Чрез използване на метода VectorLayer.Convert с подходящи параметри, изходен KML файл, KML Driver от [Drivers class](https://apireference.aspose.com/gis/net/aspose.gis/drivers), път до GeoJSON файла и GeoJSON драйвер, разработчиците могат лесно да преобразуват KML в GeoJSON данни.

{{% blocks/products/pf/feature-page-code h3="C# Code for KML to GeoJSON Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
