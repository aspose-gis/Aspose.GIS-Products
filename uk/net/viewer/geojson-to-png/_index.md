---
title: GeoJSON to PNG Viewer
url: /uk/geojson-to-png/
weight: 10
layout: single
draft: false

---

## GeoJSON to PNG Viewer

This application allows you to convert GeoJSON data into a PNG image. You can upload your own GeoJSON file or use the example provided. The viewer also allows you to customize the appearance of the map, such as changing the color scheme and zoom level.

### Features

*   Upload GeoJSON files
*   View GeoJSON data on a map
*   Customize map appearance (color scheme, zoom level)
*   Generate PNG image from the map view
*   Download generated PNG image

### Usage

1.  **Upload GeoJSON file:** Click the "Choose File" button to upload your GeoJSON file. Alternatively, you can use the example GeoJSON data provided by clicking the "Example" button.
2.  **Customize Map Appearance:** Adjust the color scheme and zoom level using the controls provided.
3.  **Generate PNG Image:** Once you are satisfied with the map view, click the "Generate PNG" button to create a PNG image of the map.
4.  **Download PNG Image:** After the PNG image is generated, click the "Download" button to save it to your computer.

### Example GeoJSON Data

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {},
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [-122.4194, 37.7749],
            [-122.4194, 37.7857],
            [-122.4067, 37.7857],
            [-122.4067, 37.7749],
            [-122.4194, 37.7749]
          ]
        ]
      }
    }
  ]
}
```

### Troubleshooting

*   **Error loading GeoJSON file:** Make sure the GeoJSON file is valid and properly formatted.
*   **Map not displaying correctly:** Check your internet connection and make sure the map tiles are loading correctly.
*   **PNG image generation failed:** Try reducing the zoom level or simplifying the GeoJSON data.

### Support

If you have any questions or encounter any issues, please contact us at [support email address].
---
