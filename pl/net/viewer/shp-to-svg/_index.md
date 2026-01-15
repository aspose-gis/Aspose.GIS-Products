---
title: Konwersja SHP do SVG
url: /pl/viewer/shp-to-svg/
weight: 10
layout: single
start: true
toc: true
draft: false
description: Narzędzie konwertujące pliki SHP do formatu SVG.
---

## Konwersja plików SHP do SVG

Narzędzie `shp2svg` służy do konwersji plików Shapefile (SHP) do formatu Scalable Vector Graphics (SVG).  Pozwala to na łatwe wyświetlanie i manipulowanie danymi wektorowymi w przeglądarce internetowej lub innych aplikacjach obsługujących SVG.

### Wymagania

*   [Narzędzie `shp2svg`](https://github.com/terra-insight/shp2svg) zainstalowane i dostępne w ścieżce systemowej.
*   Plik SHP do konwersji.

### Użycie

Uruchom narzędzie z linii poleceń, podając ścieżkę do pliku SHP jako argument:

```bash
shp2svg input.shp output.svg
```

Gdzie:

*   `input.shp` to nazwa pliku Shapefile do konwersji.
*   `output.svg` to nazwa pliku SVG, który zostanie utworzony.

### Opcje

Narzędzie `shp2svg` oferuje kilka opcji konfiguracji:

*   `-s`: Określa system współrzędnych (CRS) dla danych wektorowych.
*   `-t`: Ustawia poziom szczegółowości renderowania SVG.
*   `-b`: Dodaje tło do pliku SVG.
*   `-l`:  Włącza etykiety dla obiektów w pliku SHP.

Pełna lista opcji dostępna jest za pomocą flagi `-h`:

```bash
shp2svg -h
```

### Przykłady

**Konwersja podstawowa:**

```bash
shp2svg dane/miejscowosci.shp wynik.svg
```

To polecenie przekonwertuje plik `dane/miejscowosci.shp` na plik SVG o nazwie `wynik.svg`.

**Konwersja z określeniem systemu współrzędnych:**

```bash
shp2svg -s EPSG:4326 dane/granice_panstwa.shp granice.svg
```

To polecenie przekonwertuje plik `dane/granice_panstwa.shp` na SVG, określając system współrzędnych jako EPSG:4326.

**Konwersja z etykietami:**

```bash
shp2svg -l dane/punkty_poi.shp punkty.svg
```

To polecenie przekonwertuje plik `dane/punkty_poi.shp` na SVG i doda etykiety do każdego punktu.

### Uwagi

*   Upewnij się, że masz odpowiednie uprawnienia do odczytu pliku SHP i zapisu pliku SVG.
*   Duże pliki SHP mogą wymagać znacznej ilości pamięci podczas konwersji.
*   Wynikowy plik SVG może być bardzo duży w zależności od złożoności danych wektorowych.

---
