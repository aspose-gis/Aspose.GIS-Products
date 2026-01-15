---
title: GeoJSON to JPEG Conversion
url: /it/viewer/geojson-to-jpeg/
weight: 10
layout: single
draft: false

---

## Converting GeoJSON to JPEG Images

This tool allows you to convert GeoJSON data into JPEG images. You can customize the appearance of the generated image by adjusting various parameters.

### Input Parameters

*   **GeoJSON Data:** The GeoJSON data you want to visualize. This can be a URL pointing to a GeoJSON file or the raw GeoJSON data itself.
*   **Map Style:**  The style applied to the map visualization. Choose from predefined styles or create your own custom style.
*   **Image Width:** The width of the output JPEG image in pixels.
*   **Image Height:** The height of the output JPEG image in pixels.
*   **Zoom Level:** The zoom level of the map displayed in the image.
*   **Center Coordinates:**  The latitude and longitude coordinates to center the map view.

### Usage Examples

1.  **Using a URL for GeoJSON Data:**

    ```
    https://example.com/geojson-to-jpeg?url=https%3A%2F%2Fexample.com%2Fdata.geojson&width=800&height=600&zoom=12&center=-34%2C56
    ```

2.  **Providing Raw GeoJSON Data:**

    ```
    https://example.com/geojson-to-jpeg?geojson=%7B%22type%22%3A%22FeatureCollection%22%2C%22features%22%3A%5B%7B%22type%22%3A%22Feature%22%2C%22geometry%22%3A%7B%22type%22%3A%22Point%22%2C%22coordinates%22%3A%5B-122.4194%2C37.7749%5D%7D%2C%22properties%22%3A%7B%22name%22%3A%22San+Francisco%22%7D%7D%5D%7D&width=800&height=600&zoom=12&center=-34%2C56
    ```

### Output

The tool will generate a JPEG image based on the provided GeoJSON data and parameters. The image will be available for download.

### Error Handling

*   **Invalid GeoJSON Data:** If the provided GeoJSON data is invalid, an error message will be displayed.
*   **Invalid Parameters:**  If any of the input parameters are invalid (e.g., negative width or height), an error message will be displayed.
*   **Service Unavailable:** If the service is temporarily unavailable, an error message will be displayed.

### Customization

You can customize the appearance of the generated image by modifying the map style and other visual parameters.  Refer to the [Map Style Guide](https://example.com/map-style-guide) for more information on available styles and customization options.

---

