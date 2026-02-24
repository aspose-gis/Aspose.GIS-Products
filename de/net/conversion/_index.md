---
title: C# GIS Datenkonvertierung
url: /de/net/conversion/
description: Konvertieren Sie GIS-Daten in verschiedenen Formaten, einschließlich GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM mit wenigen Zeilen C#-Code über .NET-Bibliothek.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="GIS Datenkonvertierung Via C#" h2="Konvertieren Sie GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Daten, um plattformübergreifende .NET Mapping-Anwendungen zu erstellen." >}}

{{% blocks/products/pf/feature-page-summary %}}


Um räumliche und geografische Daten zu analysieren, erleichtert die .NET GIS API den Aufbau von Lösungen zur Erfassung, Speicherung, Verwaltung, Manipulation, Analyse und Präsentation aller Arten von geografischen Daten. Es lädt nicht nur verschiedene Vektor- und Rasterdatenformate, sondern wandelt sie auch einfach in andere Formate um. Einige Rendering-Szenarien wie **GeoJSON zu Shapefile** , **GeoJSON zu topojson**, **GeoJSON zu kml**, **Shapefile zu GeoJSON** und mehr. Für jede geografische Informationsrendering-Anwendung ohne zusätzliche Tools oder Software verfügt die .NET GIS API über die Fähigkeit, mit einer Reihe von geometrischen Features entweder einfach oder komplex zu arbeiten.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON zu Shapefile SHP Konvertierung" %}}

Mit nur wenigen Codezeilen können Entwickler GeoJSON-Daten in eine Shapefile SHP-Datei konvertieren. Die API bietet [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)

{{% blocks/products/pf/feature-page-code h3="C# Code für GeoJSON zu Shapefile Konvertierung" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Shapefile zu GeoJSON konvertieren" %}}

Der Prozess der Konvertierung von Shapefile in GeoJSON ist derselbe wie oben beschrieben, indem VectorLayer verwendet und die [Convert Methode](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) mit den entsprechenden Parametern aufgerufen wird.

{{% blocks/products/pf/feature-page-code h3="C# Code zum Konvertieren von Shapefile Daten in GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="KML zu GeoJSON konvertieren" %}}

Durch die Verwendung der VectorLayer.Convert Methode mit geeigneten Parametern, Quell-KML-Datei, KML Driver aus [Drivers Klasse](https://apireference.aspose.com/gis/net/aspose.gis/drivers), GeoJSON Dateipfad und GeoJSON Driver können Entwickler KML einfach in GeoJSON Daten konvertieren.

{{% blocks/products/pf/feature-page-code h3="C# Code für KML zu GeoJSON Konvertierung" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
