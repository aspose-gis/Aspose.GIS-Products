---
title: Conversion de données SIG C#
url: /fr/net/conversion/
description: Convertissez des données SIG dans différents formats, y compris GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM avec quelques lignes de code C# via une bibliothèque .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Conversion de données SIG Via C#" h2="Convertissez les données GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM pour créer des applications .NET de cartographie multiplateformes." >}}

{{% blocks/products/pf/feature-page-summary %}}


Pour analyser les données spatiales et géographiques, l'API SIG .NET facilite la création de solutions pour capturer, stocker, gérer, manipuler, analyser et présenter tous types de données géographiques. Elle ne charge pas seulement différents formats de données vectorielles et raster, mais les convertit également vers d'autres formats avec facilité. Quelques scénarios de rendu tels que **GeoJSON to Shapefile** , **GeoJSON to topojson**, **GeoJSON to kml**, **Shapefile to GeoJSON** et bien d'autres. Pour toute application de rendu d'informations géographiques sans nécessiter d'outils ou de logiciels supplémentaires, l'API SIG .NET a la capacité de travailler avec un certain nombre de caractéristiques géométriques, qu'elles soient simples ou complexes.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Conversion GeoJSON vers Shapefile SHP" %}}

Avec seulement quelques lignes de code, les développeurs peuvent convertir des données GeoJSON en fichier Shapefile SHP. L'API fournit [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)


{{% blocks/products/pf/feature-page-code h3="Code C# pour la conversion GeoJSON vers Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Convertir Shapefile vers GeoJSON" %}}

Le processus de conversion de Shapefile vers GeoJSON est le même que celui ci-dessus en utilisant VectorLayer et en invoquant la [méthode Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) avec les paramètres appropriés.


{{% blocks/products/pf/feature-page-code h3="Code C# pour convertir des données Shapefile en GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Convertir KML vers GeoJSON" %}}

En utilisant la méthode VectorLayer.Convert avec les paramètres appropriés, le fichier source KML, le pilote KML de [la classe Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), le chemin du fichier GeoJSON et le pilote GeoJSON, les développeurs peuvent facilement convertir KML en données GeoJSON.

{{% blocks/products/pf/feature-page-code h3="Code C# pour la conversion KML vers GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
