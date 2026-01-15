---
title: C# GIS Veri Dönüşümü
url: /tr/net/conversion/
description: GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM gibi farklı formatlardaki GIS verilerini .NET kütüphanesi aracılığıyla birkaç C# kodu satırıyla dönüştürün.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="C# ile GIS Veri Dönüşümü" h2="Çapraz platform .NET haritalama uygulamaları oluşturmak için GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM verilerini dönüştürün." >}}

{{% blocks/products/pf/feature-page-summary %}}


Uzamsal ve coğrafi verileri analiz etmek için .NET GIS API'si, yakalamak, depolamak, yönetmek, değiştirmek, analiz etmek ve her tür coğrafi veriyi sunmak için çözümler oluşturmayı kolaylaştırır. Sadece farklı vektör ve raster veri formatlarını yüklemekle kalmaz, aynı zamanda diğer formatlara da kolayca dönüştürür. Örneğin **GeoJSON'dan Shapefile'a**, **GeoJSON'dan topojson'a**, **GeoJSON'dan kml'ye**, **Shapefile'dan GeoJSON'a** ve daha fazlası gibi birçok dönüşüm senaryosu mevcuttur. .NET GIS API'si, herhangi bir ek araç veya yazılım gerektirmeden coğrafi bilgi işleme uygulamaları için basit veya karmaşık olabilecek çok sayıda geometrik özellik ile çalışabilme yeteneğine sahiptir.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON'dan Shapefile SHP Dönüşümü" %}}

Sadece birkaç satır kodla geliştiriciler GeoJSON verilerini Shapefile SHP dosyasına dönüştürebilir. API, [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(kaynak GeoJSON veri dosyası Yolu, GeoJson, hedef Shapefile Yolu, Shapefile) fonksiyonunu sağlar.


{{% blocks/products/pf/feature-page-code h3="GeoJSON'dan Shapefile Dönüşümü için C# Kodu" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Shapefile'dan GeoJSON'a Dönüştürme" %}}

Shapefile'dan GeoJSON'a dönüştürme işlemi, VectorLayer'ı kullanarak ve ilgili parametrelerle [Convert method](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) fonksiyonunu çağırarak yukarıdakiyle aynıdır.


{{% blocks/products/pf/feature-page-code h3="Shapefile Verilerini GeoJSON'a Dönüştürmek için C# Kodu" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="KML'den GeoJSON'a Dönüştürme" %}}

Uygun parametrelerle VectorLayer.Convert methodunu kullanarak, kaynak KML dosyası, [Drivers class](https://apireference.aspose.com/gis/net/aspose.gis/drivers) içindeki KML Sürücüsü, GeoJSON dosya yolu ve GeoJSON sürücüsü ile geliştiriciler KML'yi kolayca GeoJSON verisine dönüştürebilirler.

{{% blocks/products/pf/feature-page-code h3="KML'den GeoJSON'a Dönüşüm için C# Kodu" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
