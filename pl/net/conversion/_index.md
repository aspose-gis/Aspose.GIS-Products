---
title: Konwersja danych GIS w C#
url: /pl/conversion/
description: Konwertuj dane GIS w różnych formatach, w tym GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM za pomocą kilku linijek kodu C# poprzez bibliotekę .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="Konwersja danych GIS w C#" h2="Konwertuj dane GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM do budowy międzyplatformowych aplikacji .NET mapujących." >}}

{{% blocks/products/pf/feature-page-summary %}}


Do analizy danych przestrzennych i geograficznych, .NET GIS API ułatwia tworzenie rozwiązań do przechwytywania, przechowywania, zarządzania, manipulowania, analizowania i prezentowania wszystkich rodzajów danych geograficznych. Ładuje nie tylko różne formaty danych wektorowych i rastrowych, ale także z łatwością renderuje je do innych formatów. Kilka scenariuszy renderowania, takich jak **GeoJSON do Shapefile** , **GeoJSON do topojson**, **GeoJSON do kml**, **Shapefile do GeoJSON** i wiele innych. Dla każdej aplikacji renderującej informacje geograficzne, bez konieczności stosowania dodatkowych narzędzi lub oprogramowania, .NET GIS API ma możliwość pracy z wieloma cechami geometrycznymi, prostymi lub złożonymi.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="Konwersja GeoJSON do Shapefile SHP" %}}

Wystarczy kilka linijek kodu, aby przekonwertować dane GeoJSON na plik Shapefile SHP. API zapewnia [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(ścieżka do źródłowego pliku danych GeoJSON, GeoJson, ścieżka docelowego Shapefile, Shapefile)


{{% blocks/products/pf/feature-page-code h3="Kod C# do konwersji GeoJSON na Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="Konwertuj Shapefile do GeoJSON" %}}

Proces konwersji Shapefile do GeoJSON jest taki sam, jak opisany powyżej, przy użyciu VectorLayer i wywołaniu metody [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) z odpowiednimi parametrami.


{{% blocks/products/pf/feature-page-code h3="Kod C# do konwersji danych Shapefile na GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="Konwertuj KML do GeoJSON" %}}

Korzystając z metody VectorLayer.Convert z odpowiednimi parametrami, źródłowego pliku KML, sterownika KML z klasy [Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), ścieżki do pliku GeoJSON i sterownika GeoJSON, programiści mogą łatwo konwertować KML na dane GeoJSON.

{{% blocks/products/pf/feature-page-code h3="Kod C# do konwersji KML na GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
