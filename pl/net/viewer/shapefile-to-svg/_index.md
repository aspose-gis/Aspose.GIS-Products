---
title: Konwersja Shapefile do SVG
linkTitle: Konwersja Shapefile do SVG
weight: 10
description: Narzędzie do konwertowania plików shapefile na format SVG.
url: /pl/net/viewer/shapefile-to-svg/
---

## Konwersja Shapefile do SVG

To narzędzie umożliwia konwersję plików shapefile (*.shp) na obrazy w formacie Scalable Vector Graphics (*.svg).  SVG jest formatem grafiki wektorowej, co oznacza, że obrazy można powiększać bez utraty jakości. Jest to przydatne do tworzenia map i innych grafik, które muszą być wyświetlane w różnych rozmiarach.

### Wymagania

*   .NET Framework 4.7.2 lub nowsza wersja
*   Biblioteka Shapefile (ShapefileSharp)
*   Biblioteka SVG (SvgDotNet)

### Jak używać

1.  Upewnij się, że masz zainstalowane wymagane biblioteki. Możesz je pobrać z NuGet:

    ```powershell
    Install-Package ShapefileSharp
    Install-Package SvgDotNet
    ```

2.  Otwórz plik shapefile (*.shp) za pomocą klasy `ShapefileReader`.

3.  Przekształć dane shapefile na obiekty SVG za pomocą odpowiednich metod konwersji.

4.  Zapisz obrazy SVG do plików.

### Przykład kodu

```csharp
// Przykładowy kod konwertujący shapefile do SVG
using ShapefileSharp;
using SvgDotNet;

public class ShapefileToolToSvgConverter
{
    public static void Convert(string shapefilePath, string svgFilePath)
    {
        try
        {
            // Otwórz plik shapefile
            var shapefile = new ShapefileReader(shapefilePath);

            // Utwórz dokument SVG
            var svgDocument = new SvgDocument();

            // Przetwarzaj każdy rekord w shapefile
            foreach (var record in shapefile.Records)
            {
                // Konwertuj geometrię na obiekt SVG
                SvgElement svgElement = ConvertGeometryToSvg(record.Shape, shapefile);

                // Dodaj element SVG do dokumentu
                svgDocument.AddElement(svgElement);
            }

            // Zapisz dokument SVG do pliku
            svgDocument.Save(svgFilePath);
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Wystąpił błąd podczas konwersji: {ex.Message}");
        }
    }

    private static SvgElement ConvertGeometryToSvg(Shape shape, ShapefileReader shapefile)
    {
        // Implementacja konwersji geometrii na element SVG
        // ...
        return null; // Zastąp tym rzeczywistą implementacją
    }
}
```

### Opcje konfiguracyjne

*   **Skala:** Możesz dostosować skalę obrazu SVG, aby dopasować go do określonego rozmiaru.
*   **Kolory:** Możesz zmienić kolory elementów w obrazie SVG.
*   **Styl:** Możesz dodać style CSS do obrazu SVG, aby kontrolować jego wygląd.

### Rozwiązywanie problemów

*   Upewnij się, że masz zainstalowane wszystkie wymagane biblioteki.
*   Sprawdź, czy ścieżka do pliku shapefile jest poprawna.
*   Upewnij się, że format pliku shapefile jest prawidłowy.
*   Jeśli nadal masz problemy, skontaktuj się z nami.

### Dodatkowe informacje

*   [ShapefileSharp](https://github.com/NetCopilot/shapefile-sharp) - Biblioteka do odczytu i zapisu plików Shapefile.
*   [SvgDotNet](https://github.com/svgdotnet/SvgDotNet) - Biblioteka do tworzenia obrazów SVG.
---
