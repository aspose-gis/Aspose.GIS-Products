
---
title: Konversi Data GIS C#
url: /id/net/conversion/
description: Konversikan data GIS dalam berbagai format termasuk GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM dengan beberapa baris kode C# melalui .NET library.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Konversi Data GIS Melalui C#" h2="Konversikan GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Data untuk membangun aplikasi .NET pemetaan lintas platform." >}}

{{% blocks/products/pf/feature-page-summary %}}


Untuk menganalisis data spasial dan geografis, .NET GIS API memfasilitasi pembangunan solusi untuk menangkap, menyimpan, mengelola, memanipulasi, menganalisis, dan menyajikan semua jenis data geografis. Ia tidak hanya memuat berbagai format data vektor dan raster tetapi juga merender ke format lain dengan mudah. Beberapa skenario rendering seperti **GeoJSON ke Shapefile** , **GeoJSON ke topojson**, **GeoJSON ke kml**, **Shapefile ke GeoJSON** dan lainnya. Untuk aplikasi rendering informasi geografis apa pun tanpa memerlukan alat atau perangkat lunak tambahan, .NET GIS API memiliki kemampuan untuk bekerja dengan sejumlah fitur geometris baik sederhana maupun kompleks.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Konversi GeoJSON ke Shapefile SHP" %}}

Dengan hanya beberapa baris kode, pengembang dapat mengonversi data GeoJSON ke file Shapefile SHP. API menyediakan [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)


{{% blocks/products/pf/feature-page-code h3="Kode C# untuk Konversi GeoJSON ke Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Konversikan Shapefile ke GeoJSON" %}}

Proses konversi Shapefile ke GeoJSON sama dengan di atas dengan menggunakan VectorLayer dan memanggil metode [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) dengan parameter yang relevan.


{{% blocks/products/pf/feature-page-code h3="Kode C# untuk Mengonversi Data Shapefile ke GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Konversikan KML ke GeoJSON" %}}

Dengan menggunakan metode VectorLayer.Convert dengan parameter yang sesuai, file sumber KML, Driver KML dari [kelas Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), jalur file GeoJSON dan driver GeoJSON, pengembang dapat dengan mudah mengonversi KML ke data GeoJSON.

{{% blocks/products/pf/feature-page-code h3="Kode C# untuk Konversi KML ke GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
