---
title: Převod GIS dat v C#
url: /cs/net/conversion/
description: Převeďte GIS data v různých formátech včetně GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM s několika řádky kódu C# pomocí .NET knihovny.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Převod GIS dat v C#" h2="Převeďte data GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM pro sestavení multiplatformních .NET mapových aplikací." >}}

{{% blocks/products/pf/feature-page-summary %}}


Pro analýzu prostorových a geografických dat, .NET GIS API usnadňuje vytváření řešení pro zachycení, ukládání, správu, manipulaci, analýzu a prezentaci všech typů geografických dat. Nejenže načítá různé vektorové a rastrové formáty dat, ale také je snadno převádí do jiných formátů. Několik scénářů převodu, jako například **GeoJSON na Shapefile**, **GeoJSON na topojson**, **GeoJSON na kml**, **Shapefile na GeoJSON** a další. Pro jakoukoli aplikaci pro rendering geografických informací bez nutnosti dalších nástrojů nebo softwaru má .NET GIS API schopnost pracovat s řadou geometrických prvků, ať už jednoduchých nebo složitých.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Převod GeoJSON na Shapefile SHP" %}}

Pouze s několika řádky kódu mohou vývojáři převést data GeoJSON do souboru Shapefile SHP. API poskytuje [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(zdrojová cesta k datovému souboru GeoJSON, GeoJson, cílová cesta k Shapefilu, Shapefile)


{{% blocks/products/pf/feature-page-code h3="C# Kód pro převod GeoJSON na Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Převod Shapefile na GeoJSON" %}}

Proces převodu Shapefile na GeoJSON je stejný jako výše uvedený, pomocí VectorLayer a vyvoláním metody [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) s relevantními parametry.


{{% blocks/products/pf/feature-page-code h3="C# Kód pro převod dat Shapefile na GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Převod KML na GeoJSON" %}}

Pomocí metody VectorLayer.Convert s vhodnými parametry, zdrojový soubor KML, ovladač KML z [třídy Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), cesta k souboru GeoJSON a ovladač GeoJSON, mohou vývojáři snadno převést KML na data GeoJSON.

{{% blocks/products/pf/feature-page-code h3="C# Kód pro převod KML na GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
