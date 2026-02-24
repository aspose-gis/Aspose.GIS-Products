---
title: C# GIS Data Conversion
url: /nl/conversion/
description: Converteer GIS data in verschillende formaten waaronder GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM met een paar regels C# code via .NET library.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="GIS Data Conversion Via C#" h2="Converteer GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Data om cross-platform .NET mapping applicaties te bouwen." >}}

{{% blocks/products/pf/feature-page-summary %}}


Om ruimtelijke en geografische data te analyseren, vergemakkelijkt de .NET GIS API het bouwen van oplossingen voor het vastleggen, opslaan, beheren, manipuleren, analyseren en presenteren van alle soorten geografische data. Het laadt niet alleen verschillende vector- en rasterdataformaten maar rendert ze ook eenvoudig naar andere formaten. Enkele rendering scenario's zoals **GeoJSON to Shapefile** , **GeoJSON to topojson**, **GeoJSON to kml**, **Shapefile to GeoJSON** en meer. Voor elke geografische informatie rendering applicatie zonder extra tools of software, heeft de .NET GIS API de mogelijkheid om met een aantal geometrische features te werken, zowel eenvoudig als complex.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON to Shapefile SHP Conversion" %}}

Met slechts een paar regels code kunnen ontwikkelaars GeoJSON data converteren naar Shapefile SHP bestand. API biedt [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)


{{% blocks/products/pf/feature-page-code h3="C# Code voor GeoJSON to Shapefile Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert Shapefile to GeoJSON" %}}

Het proces van het converteren van Shapefile naar GeoJSON is hetzelfde als hierboven door VectorLayer te gebruiken en de [Convert method](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) aan te roepen met relevante parameters.


{{% blocks/products/pf/feature-page-code h3="C# Code voor het converteren van Shapefile Data naar GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Convert KML to GeoJSON" %}}

Door de VectorLayer.Convert methode te gebruiken met geschikte parameters, bron KML bestand, KML Driver van [Drivers class](https://apireference.aspose.com/gis/net/aspose.gis/drivers), GeoJSON bestands pad en GeoJSON driver, kunnen ontwikkelaars eenvoudig KML naar GeoJSON data converteren.

{{% blocks/products/pf/feature-page-code h3="C# Code voor KML to GeoJSON Conversion" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
