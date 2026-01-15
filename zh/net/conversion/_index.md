---
title: C# GIS 数据转换
url: /zh/net/conversion/
description: 通过 .NET 库，使用几行 C# 代码将不同格式的 GIS 数据（包括 GeoJSON、ESRI Shapefile SHX、TopoJSON、FIleGDB、GML、KML、MIF、OSM）进行转换。
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="通过 C# 进行 GIS 数据转换" h2="将 GeoJSON、ESRI Shapefile SHX、TopoJSON、FIleGDB、GML、KML、MIF、OSM 数据转换为构建跨平台 .NET 映射应用程序。" >}}

{{% blocks/products/pf/feature-page-summary %}}


为了分析空间和地理数据，.NET GIS API 有助于构建解决方案以捕获、存储、管理、操作、分析和呈现所有类型的地理数据。它不仅加载不同的矢量和栅格数据格式，而且可以轻松地渲染为其他格式。一些渲染场景，例如 **GeoJSON 到 Shapefile** 、 **GeoJSON 到 topojson** 、 **GeoJSON 到 kml** 、 **Shapefile 到 GeoJSON** 等等。对于任何地理信息渲染应用程序，而无需任何额外的工具或软件，.NET GIS API 能够处理许多几何特征，无论是简单还是复杂。

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON 到 Shapefile SHP 转换" %}}

只需几行代码，开发人员就可以将 GeoJSON 数据转换为 Shapefile SHP 文件。API 提供了 [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer)。Convert(源 GeoJSON 数据文件路径, GeoJson, 目标 Shapefile 路径, Shapefile)

{{% blocks/products/pf/feature-page-code h3="GeoJSON 到 Shapefile 转换的 C# 代码" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="将 Shapefile 转换为 GeoJSON" %}}

将 Shapefile 转换为 GeoJSON 的过程与上述过程相同，使用 VectorLayer 并调用 [Convert 方法](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) 以及相关参数。


{{% blocks/products/pf/feature-page-code h3="将 Shapefile 数据转换为 GeoJSON 的 C# 代码" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="将 KML 转换为 GeoJSON" %}}

通过使用带有适当参数的 VectorLayer.Convert 方法，源 KML 文件、[Drivers 类](https://apireference.aspose.com/gis/net/aspose.gis/drivers) 中的 KML 驱动程序、GeoJSON 文件路径和 GeoJSON 驱动程序，开发人员可以轻松地将 KML 转换为 GeoJSON 数据。

{{% blocks/products/pf/feature-page-code h3="KML 到 GeoJSON 转换的 C# 代码" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
