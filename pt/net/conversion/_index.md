---
title: Conversão de Dados GIS C#
url: /pt/conversion/
description: Converta dados GIS em diferentes formatos, incluindo GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM com poucas linhas de código C# via biblioteca .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Conversão de Dados GIS Via C#" h2="Converta GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM Data para construir aplicações .NET de mapeamento multiplataforma." >}}

{{% blocks/products/pf/feature-page-summary %}}


Para analisar dados espaciais e geográficos, a API GIS .NET facilita a construção de soluções para capturar, armazenar, gerenciar, manipular, analisar e apresentar todos os tipos de dados geográficos. Ela não apenas carrega diferentes formatos de dados vetoriais e raster, mas também renderiza para outros formatos com facilidade. Alguns cenários de renderização como **GeoJSON para Shapefile** , **GeoJSON para topojson**, **GeoJSON para kml**, **Shapefile para GeoJSON** e muito mais. Para qualquer aplicação de renderização de informações geográficas sem a necessidade de ferramentas ou softwares adicionais, a API GIS .NET tem a capacidade de trabalhar com vários recursos geométricos, simples ou complexos.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Conversão de GeoJSON para Shapefile SHP" %}}

Com apenas algumas linhas de código, os desenvolvedores podem converter dados GeoJSON para o arquivo Shapefile SHP. A API fornece [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(caminho do arquivo de dados GeoJSON de origem, GeoJson, caminho do Shapefile de destino, Shapefile)


{{% blocks/products/pf/feature-page-code h3="Código C# para Conversão de GeoJSON para Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Converter Shapefile para GeoJSON" %}}

O processo de conversão de Shapefile para GeoJSON é o mesmo do anterior, usando VectorLayer e invocando o método [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) com os parâmetros relevantes.


{{% blocks/products/pf/feature-page-code h3="Código C# para Converter Dados Shapefile para GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Converter KML para GeoJSON" %}}

Usando o método VectorLayer.Convert com os parâmetros apropriados, arquivo KML de origem, Driver KML da [classe Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), caminho do arquivo GeoJSON e driver GeoJSON, os desenvolvedores podem facilmente converter KML para dados GeoJSON.

{{% blocks/products/pf/feature-page-code h3="Código C# para Conversão de KML para GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
