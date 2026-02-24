---
title: C# GIS 데이터 변환
url: /ko/net/conversion/
description: GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM과 같은 다양한 형식의 GIS 데이터를 .NET 라이브러리를 통해 몇 줄의 C# 코드로 변환합니다.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="C#을 통한 GIS 데이터 변환" h2="GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM 데이터를 사용하여 교차 플랫폼 .NET 매핑 애플리케이션 구축." >}}

{{% blocks/products/pf/feature-page-summary %}}


공간 및 지리적 데이터를 분석하려면 .NET GIS API는 캡처, 저장, 관리, 조작, 분석 및 모든 유형의 지리적 데이터 표현을 위한 솔루션 구축을 용이하게 합니다. 다양한 벡터 및 래스터 데이터 형식을 로드할 뿐만 아니라 다른 형식으로 쉽게 렌더링합니다. **GeoJSON에서 Shapefile로**, **GeoJSON에서 topojson으로**, **GeoJSON에서 kml로**, **Shapefile에서 GeoJSON으로**와 같은 몇 가지 렌더링 시나리오가 있습니다. .NET GIS API는 추가 도구나 소프트웨어 없이도 간단하거나 복잡한 수많은 기하학적 특징과 함께 작동할 수 있습니다.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="GeoJSON에서 Shapefile SHP로 변환" %}}

몇 줄의 코드로 개발자는 GeoJSON 데이터를 Shapefile SHP 파일로 변환할 수 있습니다. API는 [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON 데이터 파일 Path, GeoJson, destination Shapefile Path, Shapefile)를 제공합니다.


{{% blocks/products/pf/feature-page-code h3="GeoJSON에서 Shapefile로 변환하기 위한 C# 코드" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Shapefile에서 GeoJSON으로 변환" %}}

Shapefile을 GeoJSON으로 변환하는 프로세스는 VectorLayer를 사용하고 관련 매개변수로 [Convert method](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2)를 호출하는 것과 동일합니다.


{{% blocks/products/pf/feature-page-code h3="Shapefile 데이터를 GeoJSON으로 변환하기 위한 C# 코드" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="KML에서 GeoJSON으로 변환" %}}

적절한 매개변수, 소스 KML 파일, [Drivers class](https://apireference.aspose.com/gis/net/aspose.gis/drivers)의 KML 드라이버, GeoJSON 파일 경로 및 GeoJSON 드라이버를 사용하여 VectorLayer.Convert 메서드를 사용하면 개발자는 KML을 GeoJSON 데이터로 쉽게 변환할 수 있습니다.

{{% blocks/products/pf/feature-page-code h3="KML에서 GeoJSON으로 변환하기 위한 C# 코드" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
