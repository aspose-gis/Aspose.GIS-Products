
---
title: C# GIS データ変換
url: /ja/net/conversion/
description: GeoJSON、ESRI Shapefile SHX、TopoJSON、FIleGDB、GML、KML、MIF、OSMなど、さまざまな形式のGISデータを.NETライブラリを介して数行のC#コードで変換します。
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="C#によるGISデータ変換" h2="クロスプラットフォーム.NETマッピングアプリケーションを構築するために、GeoJSON、ESRI Shapefile SHX、TopoJSON、FIleGDB、GML、KML、MIF、OSMデータを変換します。" >}}

{{% blocks/products/pf/feature-page-summary %}}


空間および地理的データを分析するには、.NET GIS APIは、あらゆる種類の地理的データをキャプチャ、保存、管理、操作、分析、提示するためのソリューションの構築を促進します。 異なるベクトルおよびラスターデータ形式をロードするだけでなく、他の形式に簡単にレンダリングすることもできます。 **GeoJSONからShapefile** 、 **GeoJSONからtopojson** 、 **GeoJSONからkml** 、 **ShapefileからGeoJSON** などのいくつかのレンダリングシナリオがあります。 .NET GIS APIは、追加のツールやソフトウェアを必要とせずに、地理情報レンダリングアプリケーションで動作するために、単純または複雑な数の幾何学的フィーチャーを持っています。

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSONからShapefile SHPへの変換" %}}

わずか数行のコードで、開発者はGeoJSONデータをShapefile SHPファイルに変換できます。 APIは[VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(ソースGeoJSONデータファイルのパス、GeoJson、宛先Shapefileパス、Shapefile)を提供します。


{{% blocks/products/pf/feature-page-code h3="GeoJSONからShapefileへの変換のC#コード" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="ShapefileからGeoJSONへの変換" %}}

ShapefileからGeoJSONへの変換プロセスは、VectorLayerを使用して適切なパラメータで[Convertメソッド](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2)を呼び出すものと同じです。


{{% blocks/products/pf/feature-page-code h3="ShapefileデータをGeoJSONに変換するC#コード" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="KMLからGeoJSONへの変換" %}}

適切なパラメータでVectorLayer.Convertメソッド、ソースKMLファイル、[Driversクラス](https://apireference.aspose.com/gis/net/aspose.gis/drivers)からのKMLドライバー、GeoJSONファイルパスおよびGeoJSONドライバーを使用して、開発者は簡単にKMLをGeoJSONデータに変換できます。

{{% blocks/products/pf/feature-page-code h3="KMLからGeoJSONへの変換のC#コード" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
