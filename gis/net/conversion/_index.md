---
title: C# GIS Data Conversion
url: /net/conversion/
description: Convert GIS data in different formats including GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM with few lines of C# code via .NET library.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="GIS Data Conversion Via C#" h2="Convert GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Data to build cross-platform .NET mapping applications." >}}

{{% blocks/products/pf/feature-page-summary %}}


To analyse spatial and geographic data, .NET GIS API facilitates for building solutions to capture, store, manage, manipulate, analyze and present all type of geographic data. It not only loads different vector and raster data formats but also renders to other formats with ease. Few of rendering scenarios such as **GeoJSON to Shapefile** , **GeoJSON to topojson**, **GeoJSON to kml**, **Shapefile to GeoJSON** and more. For any geographic information rendering application without requiring any additional tools or software, .NET GIS API has the capability to work with a number of geometrical features either simple or complex.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON to Shapefile SHP Conversion" %}}

With just few lines of code, developers can convert GeoJSON data to Shapefile SHP file. API provides [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)


{{% blocks/products/pf/feature-page-code h3="C# Code for GeoJSON to Shapefile Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert Shapefile to GeoJSON" %}}

Process of converting Shapefile to GeoJSON is same as of the above one by using the VectorLayer and invoking the [Convert method](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) with relevant parameters.


{{% blocks/products/pf/feature-page-code h3="C# Code for Converting Shapefile Data to GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert KML to GeoJSON" %}}

By using the VectorLayer.Convert method with appropriate parameters, source KML file, KML Driver from [Drivers class](https://apireference.aspose.com/gis/net/aspose.gis/drivers), GeoJSON file path and GeoJSON driver, devlopers can easily convert KML to GeoJSON data.

{{% blocks/products/pf/feature-page-code h3="C# Code for KML to GeoJSON Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}