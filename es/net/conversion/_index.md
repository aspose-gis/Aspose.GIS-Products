---
title: Conversión de Datos GIS en C#
url: /es/net/conversion/
description: Convierta datos GIS en diferentes formatos incluyendo GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM con pocas líneas de código C# a través de una biblioteca .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Conversión de Datos GIS Via C#" h2="Convierta datos GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM para construir aplicaciones .NET de mapeo multiplataforma." >}}

{{% blocks/products/pf/feature-page-summary %}}


Para analizar datos espaciales y geográficos, la API GIS de .NET facilita la construcción de soluciones para capturar, almacenar, administrar, manipular, analizar y presentar todo tipo de datos geográficos. No solo carga diferentes formatos de datos vectoriales y ráster, sino que también se renderiza a otros formatos con facilidad. Algunos escenarios de renderizado como **GeoJSON a Shapefile** , **GeoJSON a topojson**, **GeoJSON a kml**, **Shapefile a GeoJSON** y más. Para cualquier aplicación de renderizado de información geográfica sin requerir herramientas o software adicional, la API GIS de .NET tiene la capacidad de trabajar con una serie de características geométricas ya sean simples o complejas.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Conversión de GeoJSON a Shapefile SHP" %}}

Con solo unas pocas líneas de código, los desarrolladores pueden convertir datos GeoJSON a un archivo Shapefile SHP. La API proporciona [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(ruta del archivo de datos GeoJSON fuente, GeoJson, ruta del Shapefile de destino, Shapefile)


{{% blocks/products/pf/feature-page-code h3="Código C# para la Conversión de GeoJSON a Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Convertir Shapefile a GeoJSON" %}}

El proceso de conversión de Shapefile a GeoJSON es el mismo que el anterior utilizando VectorLayer e invocando el método [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) con los parámetros relevantes.


{{% blocks/products/pf/feature-page-code h3="Código C# para la Conversión de Datos Shapefile a GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Convertir KML a GeoJSON" %}}

Al utilizar el método VectorLayer.Convert con los parámetros apropiados, archivo KML fuente, controlador KML de la clase [Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), ruta del archivo GeoJSON y controlador GeoJSON, los desarrolladores pueden convertir fácilmente KML a datos GeoJSON.

{{% blocks/products/pf/feature-page-code h3="Código C# para la Conversión de KML a GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
