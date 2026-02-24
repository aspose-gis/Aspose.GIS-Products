---
title: Konwertuj MIF do KML GIS Data przez .NET 
weight: 50
url: /pl/net/conversion/mif-to-kml/ 
description: Wypróbuj nasze API On-Premise do konwersji danych GIS w .NET Framework, .NET Core.
---

{{< blocks/products/pf/upper-banner h1="Konwertuj MIF do KML w C#" h2="Eksportuj MIF do KML używając API po stronie serwera, bez potrzeby oprogramowania takiego jak ArcGIS, ArcMap, QGIS lub Google Earth." logoImageSrc="https://www.aspose.cloud/templates/aspose/img/products/gis/aspose_gis-for-net.svg" sourceAdditionalConversionTag="" additionalConversionTag="KML" pfName="Aspose.GIS" subTitlepfName="dla .NET" downloadUrl="#" fileiconsmall1="PNG" fileiconsmall2="JPG" fileiconsmall3="BMP" fileiconsmall4="TIFF" fileiconsmall5="MIF" >}}

{{% blocks/products/pf/agp/content h2="Jak przekonwertować MIF do KML używając C#" %}}
Aby przekonwertować MIF do KML, użyjemy
[Aspose.GIS for .NET](https://products.aspose.com/gis/net) 
API, które jest bogate w funkcje, potężne i łatwe w użyciu API GIS dla platformy C#. Otwórz
[NuGet](https://www.nuget.org/packages/aspose.gis) 
menedżer pakietów, wyszukaj
**Aspose.GIS** 
i zainstaluj. Możesz również użyć następującego polecenia z Konsoli Menedżera Pakietów.

{{% blocks/products/pf/agp/code-block title="Polecenie" offSpacer="true" %}}
```cs
PM> Install-Package Aspose.GIS
```
{{% /blocks/products/pf/agp/code-block %}}
{{% /blocks/products/pf/agp/content %}}

{{< blocks/products/pf/agp/feature-section isGrey="true" >}}

{{% blocks/products/pf/agp/feature-section-col title="Kroki konwersji MIF do KML w C#" %}}
{{% blocks/products/pf/agp/text %}}
Konwersja może być wykonana za pomocą jednej linii kodu, używając
*VectorLayer.Convert* 
metody. Przyjmuje ona 4 parametry, jak opisano poniżej.
{{% /blocks/products/pf/agp/text %}}

1.  Ścieżka do pliku źródłowego MIF typu string
2.  Źródło sterownika, aby poinformować API o formacie wejściowym. Ustaw go na Drivers.MapInfoInterchange
3.  Ścieżka do pliku danych docelowych KML typu string
4.  Docelowy sterownik określający format wyjściowy. Ustaw go na Drivers.Kml
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/feature-section-col title="Wymagania systemowe" %}}
{{% blocks/products/pf/agp/text %}}
Nasze API są obsługiwane na wszystkich głównych platformach i systemach operacyjnych. Przed wykonaniem poniższego kodu upewnij się, że masz następujące wymagania wstępne w swoim systemie.
{{% /blocks/products/pf/agp/text %}}
{{% /blocks/products/pf/agp/feature-section-col %}}

{{% blocks/products/pf/agp/code-block title="Zapisz MIF jako KML - C#" offSpacer="" %}}
```cs
// Konwertuj dane GIS MIF na dane KML
VectorLayer.Convert(dir + "example.mif", Drivers.MapInfoInterchange, dir + "output.kml", Drivers.Kml);
```
{{% /blocks/products/pf/agp/code-block %}}

{{< /blocks/products/pf/agp/feature-section >}}

{{< blocks/products/pf/agp/faq-item question="" answer="" >}}

<!-- aboutfile Starts -->

{{< blocks/products/pf/agp/demobox sectionTitle="MIF do KML Live Demos" sectionDescription="Konwertuj MIF na KML już teraz, odwiedzając naszą [Live Demos website](https://products.aspose.app/gis/conversion/mif-to-kml). Demo na żywo ma następujące korzyści" >}}
    {{< blocks/products/pf/agp/democard icon="fa-cogs" text=" Nie musisz pobierać API Aspose GIS." >}}
    {{< blocks/products/pf/agp/democard icon="fa-edit" text=" Po prostu wybierz KML jako format wyjściowy i." >}}
    {{< blocks/products/pf/agp/democard icon="fa-file-text" text=" Prześlij swój plik MIF, zostanie natychmiast przekonwertowany na KML." >}}
    {{< blocks/products/pf/agp/democard icon="fa-download" text=" Otrzymasz link do pobrania." >}}

    {{% blocks/products/pf/agp/content h2=".NET GIS Library" %}}
    Aspose.GIS for .NET to API do manipulacji i konwersji danych GIS. W pełni obsługuje odczyt, zapis i konwersję znanych formatów danych GIS, takich jak pliki Shapefile ESRI, GeoJSON, TopoJSON, Baza Danych ESRI Geodatabase, Język Oznaczania Geografii, Google Earth, Format Wymiany GPS, Formaty MapInfo i OpenStreetMap. Jest to samodzielne API oparte na .NET i nie wymaga żadnego oprogramowania GIS takiego jak ArcGIS / ArcMap, QGIS itp. 
    {{% /blocks/products/pf/agp/content %}}

    {{< blocks/products/pf/agp/about-file-section >}}
        {{< blocks/products/pf/agp/about-file-text fileFormat="MIF" readMoreLink="https://docs.fileformat.com/gis/kml/" >}}
        {{mif}}
        Przeczytaj Więcej
        {{< /blocks/products/pf/agp/about-file-text >}}

        {{< blocks/products/pf/agp/about-file-text fileFormat="KML" readMoreLink="" >}}
        KML, (Keyhole Markup Language zawiera) informacje geograficzne w notacji XML. Pliki zapisane jako KML mogą być otwierane w aplikacjach Systemów Informacji Geograficznej (GIS), pod warunkiem że je obsługują. Wiele aplikacji zaczęło wspierać format plików KML po jego przyjęciu jako międzynarodowy standard. KML używa struktury opartej na tagach zagnieżdżonych elementach i atrybutach. Wszystkie tagi są rozróżniane wielkością liter, a kolejność tych tagów, zgodnie z Referencją KML, jest ważna do przestrzegania.
        Przeczytaj Więcej
        {{< /blocks/products/pf/agp/about-file-text >}}
    {{< /blocks/products/pf/agp/about-file-section >}}
{{< /blocks/products/pf/agp/demobox >}}

<!-- aboutfile Ends -->

{{< blocks/products/pf/agp/other-supported-section title="Inne obsługiwane konwersje" subTitle="Możesz również przekonwertować MIF do wielu innych formatów plików, w tym kilku wymienionych poniżej." >}}
    {{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/gis/net/conversion/mif-to-geojson" name="MIF DO GEOJSON" description="Format oparty na JSON" >}}
    {{< blocks/products/pf/agp/other-supported-section-item href="https://products.aspose.com/gis/net/conversion/mif-to-shx" name="MIF DO SHX" description="Rozszerzenie pliku Shapefile" >}}
{{< /blocks/products/pf/agp/other-supported-section >}}
