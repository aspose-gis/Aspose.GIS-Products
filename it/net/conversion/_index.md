---
title: Conversione di dati GIS C#
url: /it/net/conversion/
description: Converti dati GIS in diversi formati tra cui GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM con poche righe di codice C# tramite libreria .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Conversione di dati GIS tramite C#" h2="Converti dati GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM per creare applicazioni .NET di mappatura multipiattaforma." >}}

{{% blocks/products/pf/feature-page-summary %}}


Per analizzare dati spaziali e geografici, l'API GIS .NET facilita la creazione di soluzioni per acquisire, archiviare, gestire, manipolare, analizzare e presentare tutti i tipi di dati geografici. Non solo carica diversi formati di dati vettoriali e raster, ma li converte anche in altri formati con facilità. Alcuni scenari di rendering come **GeoJSON to Shapefile** , **GeoJSON to topojson**, **GeoJSON to kml**, **Shapefile to GeoJSON** e altro ancora. Per qualsiasi applicazione di rendering di informazioni geografiche senza la necessità di strumenti o software aggiuntivi, l'API GIS .NET ha la capacità di lavorare con un numero di funzionalità geometriche sia semplici che complesse.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Conversione da GeoJSON a Shapefile SHP" %}}

Con solo poche righe di codice, gli sviluppatori possono convertire i dati GeoJSON in un file Shapefile SHP. L'API fornisce [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(percorso del file di dati GeoJSON sorgente, GeoJson, percorso Shapefile di destinazione, Shapefile)


{{% blocks/products/pf/feature-page-code h3="Codice C# per la conversione da GeoJSON a Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Converti Shapefile in GeoJSON" %}}

Il processo di conversione da Shapefile a GeoJSON è lo stesso del precedente utilizzando VectorLayer e invocando il metodo [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) con i parametri appropriati.


{{% blocks/products/pf/feature-page-code h3="Codice C# per la conversione di dati Shapefile in GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Converti KML in GeoJSON" %}}

Utilizzando il metodo VectorLayer.Convert con i parametri appropriati, file KML di origine, driver KML dalla [classe Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), percorso del file GeoJSON e driver GeoJSON, gli sviluppatori possono facilmente convertire KML in dati GeoJSON.

{{% blocks/products/pf/feature-page-code h3="Codice C# per la conversione da KML a GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
