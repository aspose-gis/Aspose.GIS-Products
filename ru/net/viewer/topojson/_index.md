---
title: TopoJSON Viewer
url: /ru/viewer/topojson/
weight: 10
aliases: [topojson, viewer]
---

## Overview

The TopoJSON Viewer is a tool for visualizing and interacting with TopoJSON data. It allows you to explore geographic features, zoom in on areas of interest, and query attributes associated with each feature.

## Features

*   **Interactive Map:** Pan and zoom around the map to explore different regions.
*   **Feature Highlighting:** Hover over features to see their attribute information.
*   **Attribute Display:** View a detailed breakdown of attributes for selected features.
*   **Data Filtering:** Filter features based on specific attribute values.
*   **Customizable Styling:** Adjust the appearance of features using various styling options.

## Usage

1.  **Load TopoJSON Data:** Provide the URL or file path to your TopoJSON data.
2.  **Configure Options:** Set any desired configuration options, such as initial zoom level and feature highlighting behavior.
3.  **Explore the Map:** Use the interactive map controls to navigate and explore the data.

## Example

```javascript
// Пример использования:
var viewer = new TopoJSONViewer({
    container: 'map', // ID элемента контейнера карты
    url: '/data/your_topojson_file.topojson', // URL файла TopoJSON
    highlightOnHover: true, // Подсвечивать при наведении
    initialZoom: 5 // Начальный уровень масштабирования
});
```

## Data Sources

*   [Natural Earth](https://www.naturalearthdata.com/)
*   [TopoJSON Collection](https://geojson.io/topojson)

## Support

If you encounter any issues or have suggestions for improvement, please contact us at [support@example.com](mailto:support@example.com).

---
