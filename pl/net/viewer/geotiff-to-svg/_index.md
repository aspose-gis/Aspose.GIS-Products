---
title: GeoTIFF to SVG Conversion
linkTitle: Konwersja GeoTIFF do SVG
weight: 10
url: /pl/net/viewer/geotiff-to-svg/
description: Learn how to convert GeoTIFF images to scalable vector graphics (SVG) format using the .NET viewer.
---

## Introduction
## Wprowadzenie

This guide explains how to convert GeoTIFF images to SVG format using our .NET viewer. This process allows you to vectorize raster data, making it suitable for various applications like web mapping and graphic design.
Ten przewodnik wyjaśnia, jak konwertować obrazy GeoTIFF do formatu SVG przy użyciu naszego przeglądarki .NET. Ten proces umożliwia wektoryzację danych rastrowych, dzięki czemu nadają się do różnych zastosowań, takich jak mapowanie internetowe i projektowanie graficzne.

## Prerequisites
## Wymagania wstępne

*   **.NET SDK:** You need the .NET SDK installed on your system.
    **Zestaw SDK .NET:** Musisz mieć zainstalowany zestaw SDK .NET na swoim systemie.
*   **GeoTIFF Image:** Have a GeoTIFF image file ready for conversion.
    **Obraz GeoTIFF:** Przygotuj plik obrazu GeoTIFF do konwersji.
*   **.NET Viewer Library:** Include the .NET viewer library in your project.
    **Biblioteka przeglądarki .NET:** Dodaj bibliotekę przeglądarki .NET do swojego projektu.

## Conversion Steps
## Kroki konwersji

1.  **Load GeoTIFF Image:** Load the GeoTIFF image into the viewer.
    **Załaduj obraz GeoTIFF:** Załaduj obraz GeoTIFF do przeglądarki.
2.  **Configure SVG Options:** Set up the desired options for the SVG conversion, such as resolution and color palette.
    **Skonfiguruj opcje SVG:** Skonfiguruj pożądane opcje konwersji SVG, takie jak rozdzielczość i paleta kolorów.
3.  **Convert to SVG:** Perform the conversion from GeoTIFF to SVG.
    **Konwertuj do SVG:** Wykonaj konwersję z GeoTIFF do SVG.
4.  **Save SVG File:** Save the resulting SVG file to your desired location.
    **Zapisz plik SVG:** Zapisz wynikowy plik SVG w żądanym miejscu.

## Code Example
## Przykład kodu

```csharp
// Load GeoTIFF image
RasterImage image = new RasterImage("path/to/your/image.tif");

// Configure SVG options
SvgOptions svgOptions = new SvgOptions();
svgOptions.Resolution = 300;
svgOptions.ColorPalette = ColorPalette.TrueColor;

// Convert to SVG
string svgString = image.ConvertToSvg(svgOptions);

// Save SVG file
File.WriteAllText("path/to/your/output.svg", svgString);
```

## Troubleshooting
## Rozwiązywanie problemów

*   **Image Loading Errors:** Ensure the GeoTIFF file is valid and accessible.
    **Błędy ładowania obrazu:** Upewnij się, że plik GeoTIFF jest prawidłowy i dostępny.
*   **Conversion Issues:** Adjust SVG options to optimize for image complexity and desired output quality.
    **Problemy z konwersją:** Dostosuj opcje SVG, aby zoptymalizować złożoność obrazu i pożądaną jakość wyjściową.
*   **File Saving Errors:** Verify write permissions to the target directory.
    **Błędy zapisywania plików:** Sprawdź uprawnienia do zapisu w katalogu docelowym.

## Further Reading
## Dalsza lektura

*   [GeoTIFF Specification](https://www.geo-tiff.org/)
    [Specyfikacja GeoTIFF](https://www.geo-tiff.org/)
*   [SVG Specification](https://www.w3.org/TR/svg11/)
    [Specyfikacja SVG](https://www.w3.org/TR/svg11/)
---
