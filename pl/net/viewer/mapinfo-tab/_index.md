---
title: "MapInfo Tab"
linkTitle: "Zakładka MapInfo"
weight: 10
url: "/pl/net/viewer/mapinfo-tab/"
aliases:
  - "mapinfo"
  - "map info"
source: "https://github.com/Esri/arcgis-js-api-samples/blob/master/4.x/webmaps/MapInfoTab/"
---

## MapInfo Tab

The MapInfo tab provides access to the MapInfo table view within the viewer.

## Funkcje

Zakładka MapInfo zapewnia dostęp do widoku tabeli MapInfo w przeglądarce.

### Displaying a Table

Aby wyświetlić tabelę, należy najpierw załadować ją do przeglądarki. Można to zrobić na kilka sposobów:

* Using the `addTable` method of the `MapInfo` class.
* Using the `openTable` method of the `MapInfo` class.
* By dragging a table file onto the viewer canvas.

Aby wyświetlić tabelę, należy najpierw załadować ją do przeglądarki. Można to zrobić na kilka sposobów:

* Używając metody `addTable` klasy `MapInfo`.
* Używając metody `openTable` klasy `MapInfo`.
* Przeciągając plik tabeli na płótno przeglądarki.

### Table View

The table view displays the data in a tabular format. The user can sort, filter, and paginate the data.

Widok tabeli wyświetla dane w formacie tabelarycznym. Użytkownik może sortować, filtrować i paginować dane.

### Selecting Features

The user can select features in the table view by clicking on a row. The selected features will be highlighted on the map.

Użytkownik może wybrać obiekty w widoku tabeli, klikając w wiersz. Wybrane obiekty zostaną wyróżnione na mapie.

### Editing Features

The user can edit features in the table view by double-clicking on a row. The edited features will be updated on the map.

Użytkownik może edytować obiekty w widoku tabeli, klikając dwukrotnie w wiersz. Edytowane obiekty zostaną zaktualizowane na mapie.

### Exporting Data

The user can export data from the table view to a CSV file.

Użytkownik może eksportować dane z widoku tabeli do pliku CSV.
