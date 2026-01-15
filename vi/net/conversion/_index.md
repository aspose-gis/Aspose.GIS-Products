---
title: Chuyển đổi Dữ liệu GIS C#
url: /vi/net/conversion/
description: Chuyển đổi dữ liệu GIS ở các định dạng khác nhau bao gồm GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM bằng một vài dòng mã C# thông qua thư viện .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Chuyển đổi Dữ liệu GIS Qua C#" h2="Chuyển đổi GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Data để xây dựng các ứng dụng .NET đa nền tảng." >}}

{{% blocks/products/pf/feature-page-summary %}}


Để phân tích dữ liệu không gian và địa lý, API GIS .NET tạo điều kiện thuận lợi cho việc xây dựng các giải pháp để thu thập, lưu trữ, quản lý, thao tác, phân tích và trình bày tất cả các loại dữ liệu địa lý. Nó không chỉ tải các định dạng vector và raster khác nhau mà còn dễ dàng chuyển đổi sang các định dạng khác. Một số kịch bản hiển thị như **GeoJSON thành Shapefile** , **GeoJSON thành topojson**, **GeoJSON thành kml**, **Shapefile thành GeoJSON** và hơn thế nữa. Đối với bất kỳ ứng dụng hiển thị thông tin địa lý nào mà không cần thêm công cụ hoặc phần mềm, API GIS .NET có khả năng làm việc với một số tính năng hình học đơn giản hoặc phức tạp.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Chuyển đổi GeoJSON thành Shapefile SHP" %}}

Chỉ với một vài dòng mã, các nhà phát triển có thể chuyển đổi dữ liệu GeoJSON thành tệp Shapefile SHP. API cung cấp [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(đường dẫn tệp dữ liệu GeoJSON nguồn, GeoJson, đường dẫn Shapefile đích, Shapefile)


{{% blocks/products/pf/feature-page-code h3="Mã C# để Chuyển đổi GeoJSON thành Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Chuyển đổi Shapefile thành GeoJSON" %}}

Quá trình chuyển đổi Shapefile thành GeoJSON giống như quá trình trên bằng cách sử dụng VectorLayer và gọi phương thức [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) với các tham số liên quan.


{{% blocks/products/pf/feature-page-code h3="Mã C# để Chuyển đổi Dữ liệu Shapefile thành GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Chuyển đổi KML thành GeoJSON" %}}

Bằng cách sử dụng phương thức VectorLayer.Convert với các tham số thích hợp, tệp nguồn KML, Trình điều khiển KML từ [lớp Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), đường dẫn tệp GeoJSON và trình điều khiển GeoJSON, nhà phát triển có thể dễ dàng chuyển đổi KML thành dữ liệu GeoJSON.

{{% blocks/products/pf/feature-page-code h3="Mã C# để Chuyển đổi KML thành GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
