---
title: KML to JPEG Conversion
linkTitle: Konwersja KML do JPEG
weight: 10
url: /pl/net/viewer/kml-to-jpeg/
aliases: [KML2JPEG, kml2jpeg]
description: Convert KML files to JPEGs using the .NET viewer.
---

## Overview
## Przegląd

This document outlines how to convert KML (Keyhole Markup Language) files to JPEG images using the .NET viewer. This process is useful for generating thumbnails, previews, or static imagery from your KML data.
Ten dokument opisuje sposób konwersji plików KML (Keyhole Markup Language) do obrazów JPEG za pomocą przeglądarki .NET. Ten proces jest przydatny do generowania miniatur, podglądów lub statycznych obrazów z danych KML.

## Prerequisites
## Wymagania wstępne

*   **.NET SDK:** You need the .NET SDK installed on your system.
    **Zestaw SDK .NET:** Musisz mieć zainstalowany zestaw SDK .NET na swoim systemie.
*   **Viewer Library:**  The .NET viewer library must be available in your project.
    **Biblioteka przeglądarki:** Biblioteka przeglądarki .NET musi być dostępna w Twoim projekcie.

## Conversion Process
## Proces konwersji

1.  **Load the KML File:** Load the KML file into the viewer.
    **Załaduj plik KML:** Załaduj plik KML do przeglądarki.
2.  **Configure Rendering Options:** Set up rendering options such as viewport size, zoom level, and background color.
    **Skonfiguruj opcje renderowania:** Skonfiguruj opcje renderowania, takie jak rozmiar okna widoku, poziom powiększenia i kolor tła.
3.  **Render to JPEG:** Render the KML data as a JPEG image.
    **Wyrenderuj do JPEG:** Wyrenderuj dane KML jako obraz JPEG.
4.  **Save the JPEG File:** Save the rendered JPEG image to a file.
    **Zapisz plik JPEG:** Zapisz wyrenderowany obraz JPEG do pliku.

## Code Example
## Przykład kodu

```csharp
// Load the KML file
KmlFile kml = new KmlFile(new FileInfo("path/to/your/file.kml"));

// Configure rendering options
Viewport viewport = new Viewport() { Width = 800, Height = 600 };
RenderingOptions options = new RenderingOptions() { Viewport = viewport, BackgroundColor = Color.White };

// Render to JPEG
using (Bitmap bitmap = viewer.Render(kml, options)) {
    // Save the JPEG file
    bitmap.Save("path/to/output/image.jpeg", ImageFormat.Jpeg);
}
```

## Considerations
## Uwagi

*   **Performance:** Rendering complex KML files can be computationally intensive. Optimize your rendering options and consider using asynchronous operations to improve performance.
    **Wydajność:** Renderowanie złożonych plików KML może być kosztowne obliczeniowo. Zoptymalizuj opcje renderowania i rozważ użycie operacji asynchronicznych, aby poprawić wydajność.
*   **Error Handling:** Implement robust error handling to gracefully handle invalid KML files or rendering errors.
    **Obsługa błędów:** Wdróż solidną obsługę błędów, aby elegancko obsługiwać nieprawidłowe pliki KML lub błędy renderowania.
*   **Dependencies:** Ensure that all necessary dependencies are included in your project.
    **Zależności:** Upewnij się, że wszystkie niezbędne zależności są dołączone do Twojego projektu.

---
