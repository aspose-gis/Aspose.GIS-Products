---
title: GeoJSON to PNG Viewer
linkTitle: Przeglądarka GeoJSON do PNG
weight: 10
url: /pl/net/viewer/geojson-to-png/
description: Convert GeoJSON data to PNG images with custom styling options. Konwertuj dane GeoJSON na obrazy PNG z opcjami niestandardowego stylu.
---

## Overview Przegląd

This application allows you to convert GeoJSON data into PNG images. Możesz użyć go do wizualizacji danych geograficznych w prosty i wygodny sposób. Ta aplikacja umożliwia konwersję danych GeoJSON na obrazy PNG. Pozwala to na wizualizację danych geograficznych w prosty i wygodny sposób.

## Features Funkcje

*   **GeoJSON Input:** Supports various GeoJSON formats. Obsługuje różne formaty GeoJSON.
*   **Custom Styling:** Customize the appearance of your map with different colors, line widths, and fill patterns. Dostosuj wygląd swojej mapy za pomocą różnych kolorów, szerokości linii i wzorców wypełnienia.
*   **Image Export:** Export the resulting map as a PNG image. Eksportuj wynikową mapę jako obraz PNG.
*   **User-Friendly Interface:** Easy to use with clear instructions and controls. Łatwy w użyciu dzięki jasnym instrukcjom i sterowaniu.

## Usage Użycie

1.  **Input GeoJSON Data:** Provide a valid GeoJSON file or URL. Podaj prawidłowy plik GeoJSON lub adres URL.
2.  **Configure Styling Options:** Adjust the styling options to your liking. Dostosuj opcje stylu do swoich preferencji.
3.  **Generate PNG Image:** Click the "Generate" button to create the PNG image. Kliknij przycisk „Generuj”, aby utworzyć obraz PNG.
4.  **Download Image:** Download the generated PNG image. Pobierz wygenerowany obraz PNG.

## Styling Options Opcje stylu

*   **Color:** Set the fill color of polygons and markers. Ustaw kolor wypełnienia poligonów i znaczników.
*   **Line Width:** Adjust the width of lines for roads, rivers, and other linear features. Dostosuj szerokość linii dla dróg, rzek i innych liniowych elementów.
*   **Fill Pattern:** Choose a fill pattern for polygons. Wybierz wzór wypełnienia dla poligonów.
*   **Marker Size:** Set the size of markers. Ustaw rozmiar znaczników.

## Example Przykład

Here's an example GeoJSON file: Oto przykładowy plik GeoJSON:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [[[-122.4194, 37.7749], [-122.4068, 37.7749], [-122.4068, 37.7857], [-122.4194, 37.7857], [-122.4194, 37.7749]]]
      },
      "properties": {
        "name": "Golden Gate Park"
      }
    }
  ]
}
```

## Troubleshooting Rozwiązywanie problemów

*   **Invalid GeoJSON:** Make sure your GeoJSON file is valid. Upewnij się, że twój plik GeoJSON jest prawidłowy.
*   **Styling Issues:** Double-check your styling options to ensure they are correct. Sprawdź dwa razy swoje opcje stylu, aby upewnić się, że są poprawne.
*   **Image Generation Errors:** If you encounter any errors during image generation, try simplifying your GeoJSON data or reducing the number of features. Jeśli napotkasz jakiekolwiek błędy podczas generowania obrazu, spróbuj uprościć swoje dane GeoJSON lub zmniejszyć liczbę elementów.

---
