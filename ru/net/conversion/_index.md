---
title: Преобразование GIS данных на C#
url: /ru/net/conversion/
description: Преобразуйте GIS данные в различных форматах, включая GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM с помощью нескольких строк кода C# через .NET библиотеку.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Преобразование GIS данных на C#" h2="Преобразуйте GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM данные для создания кроссплатформенных .NET картографических приложений." >}}

{{% blocks/products/pf/feature-page-summary %}}


Для анализа пространственных и географических данных, .NET GIS API облегчает создание решений для захвата, хранения, управления, манипулирования, анализа и представления всех типов географических данных. Он не только загружает различные векторные и растровые форматы данных, но также легко преобразует их в другие форматы. Некоторые сценарии преобразования, такие как **GeoJSON в Shapefile** , **GeoJSON в topojson**, **GeoJSON в kml**, **Shapefile в GeoJSON** и многие другие. Для любого приложения для рендеринга географической информации без необходимости каких-либо дополнительных инструментов или программного обеспечения, .NET GIS API имеет возможность работать с множеством геометрических объектов, будь то простые или сложные.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Преобразование GeoJSON в Shapefile SHP" %}}

Всего за несколько строк кода разработчики могут преобразовывать данные GeoJSON в файл Shapefile SHP. API предоставляет [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(путь к исходному файлу данных GeoJSON, GeoJson, путь назначения Shapefile, Shapefile)

{{% blocks/products/pf/feature-page-code h3="C# код для преобразования GeoJSON в Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Преобразование Shapefile в GeoJSON" %}}

Процесс преобразования Shapefile в GeoJSON такой же, как и описанный выше, с использованием VectorLayer и вызовом метода [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) с соответствующими параметрами.

{{% blocks/products/pf/feature-page-code h3="C# код для преобразования данных Shapefile в GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Преобразование KML в GeoJSON" %}}

Используя метод VectorLayer.Convert с соответствующими параметрами, исходный файл KML, драйвер KML из [класса Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), путь к файлу GeoJSON и драйвер GeoJSON, разработчики могут легко преобразовывать KML в данные GeoJSON.

{{% blocks/products/pf/feature-page-code h3="C# код для преобразования KML в GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
