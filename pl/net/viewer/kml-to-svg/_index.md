---
title: KML to SVG Conversion
linkTitle: Konwersja KML na SVG
weight: 10
url: /pl/net/viewer/kml-to-svg/
aliases: [KML2SVG, KML do SVG]
description: Convert KML files to SVG format using .NET.
---

## Overview
## Przegląd

This viewer allows you to convert KML (Keyhole Markup Language) files into SVG (Scalable Vector Graphics) format. This conversion enables easier manipulation and styling of geographic data within web browsers and other applications that support SVG.
Ten widok umożliwia konwersję plików KML (Keyhole Markup Language, Język Oznaczeń Keyhole) do formatu SVG (Scalable Vector Graphics, Grafika Wektorowa Skalowalna). Ta konwersja umożliwia łatwiejszą manipulację i stylizację danych geograficznych w przeglądarkach internetowych i innych aplikacjach obsługujących SVG.

## Features
## Funkcje

*   **KML to SVG Conversion:** Converts KML files into SVG format. Konwertuje pliki KML do formatu SVG.
*   **Customizable Styles:** Apply custom styles and themes to the generated SVG output. Zastosuj niestandardowe style i motywy do wygenerowanego wyniku SVG.
*   **Geographic Data Visualization:** Visualize geographic data from KML files in a scalable vector graphic format. Wizualizuj dane geograficzne z plików KML w formacie skalowalnej grafiki wektorowej.
*   **.NET Integration:** Seamlessly integrates with .NET applications and workflows. Bezproblemowa integracja z aplikacjami i przepływami pracy .NET.

## Usage
## Użycie

1.  **Input KML File:** Provide a valid KML file as input. Podaj prawidłowy plik KML jako dane wejściowe.
2.  **Conversion Process:** The viewer processes the KML data and converts it into SVG format. Widok przetwarza dane KML i konwertuje je do formatu SVG.
3.  **Output SVG File:** Download the generated SVG file for further use or integration. Pobierz wygenerowany plik SVG do dalszego użytku lub integracji.

## Example
## Przykład

```csharp
// Sample code demonstrating KML to SVG conversion
// Przykładowy kod demonstrujący konwersję KML na SVG
using Net.Viewer.KmlToSvg;

public class Example
{
    public static void Main(string[] args)
    {
        KmlConverter converter = new KmlConverter();
        string kmlFilePath = "path/to/your/file.kml";
        string svgFilePath = "path/to/output/file.svg";

        converter.Convert(kmlFilePath, svgFilePath);
    }
}
```

## Supported KML Features
## Obsługiwane funkcje KML

*   Placemarks (Znaczniki)
*   NetworkLinks (Połączenia sieciowe)
*   GroundOverlays (Nakładki na powierzchnię)
*   Folders (Foldery)
*   Document Metadata (Metadane dokumentu)

## Limitations
## Ograniczenia

*   Complex KML structures may not be fully supported. Złożone struktury KML mogą nie być w pełni obsługiwane.
*   Large KML files may require significant processing time. Duże pliki KML mogą wymagać znacznego czasu przetwarzania.
*   The accuracy of the conversion depends on the validity and structure of the input KML file. Dokładność konwersji zależy od ważności i struktury pliku KML wejściowego.

---
