---
title: Convert GeoJSON to PNG
url: /ko/viewer/geojson-to-png/
weight: 10
description: Convert GeoJSON data to PNG images using the NetViewer tool.
aliases: [geojson2png, geojson to png]
---

## Overview

NetViewer provides a simple and efficient way to convert GeoJSON data into PNG images. This allows you to visualize geospatial data without needing complex mapping software or libraries.  The conversion process is straightforward and customizable, enabling you to generate maps tailored to your specific needs.

## Prerequisites

*   **NetViewer Installation:** Ensure that NetViewer is installed and accessible on your system.
*   **GeoJSON File:** Have a valid GeoJSON file ready for conversion.
*   **Map Styles (Optional):**  Prepare any custom map styles or configurations you want to apply during the conversion process.

## Usage

The basic command structure for converting GeoJSON to PNG is as follows:

```bash
netviewer geojson-to-png -i <input_geojson_file> -o <output_png_file> [options]
```

### Parameters

*   `-i` or `--input`: Specifies the path to the input GeoJSON file.  (필수)
*   `-o` or `--output`: Specifies the path and filename for the output PNG image. (필수)
*   `-s` or `--scale`: Sets the scale of the map. Default is 1.
*   `-w` or `--width`: Defines the width of the output PNG image in pixels. Default is 500.
*   `-h` or `--height`: Defines the height of the output PNG image in pixels. Default is 300.
*   `-m` or `--map-style`:  Applies a custom map style configuration file.
*   `-t` or `--tile-server`: Specifies a tile server URL for background maps.
*   `-z` or `--zoom`: Sets the zoom level of the map. Default is 10.
*   `-b` or `--bounds`: Defines the bounding box coordinates [minLon, minLat, maxLon, maxLat].

### Examples

**Basic Conversion:**

```bash
netviewer geojson-to-png -i my_data.geojson -o output.png
```

이 명령어는 `my_data.geojson` 파일을 `output.png`로 변환합니다.

**Custom Width and Height:**

```bash
netviewer geojson-to-png -i my_data.geojson -o output.png -w 800 -h 600
```

이 명령어는 GeoJSON 데이터를 사용하여 너비가 800픽셀이고 높이가 600픽셀인 PNG 이미지를 생성합니다.

**Applying a Map Style:**

```bash
netviewer geojson-to-png -i my_data.geojson -o output.png -m custom_style.json
```

이 명령어는 `custom_style.json`에 정의된 스타일을 적용하여 GeoJSON 데이터를 PNG 이미지로 변환합니다.

**Using a Tile Server:**

```bash
netviewer geojson-to-png -i my_data.geojson -o output.png -t https://tileprovider.com/tiles/{z}/{x}/{y}.png
```

이 명령어는 지정된 타일 서버에서 배경 지도를 사용하여 GeoJSON 데이터를 PNG 이미지로 변환합니다.

## Advanced Options

### Map Styles

Map styles allow you to customize the visual appearance of your map, including colors, fonts, and labels. You can create custom style files in JSON format to define these settings.  Refer to the NetViewer documentation for detailed information on creating and using map styles.

### Tile Servers

NetViewer supports various tile servers, such as OpenStreetMap, Mapbox, and Google Maps. By specifying a tile server URL, you can overlay your GeoJSON data onto a pre-rendered basemap.

## Troubleshooting

*   **Invalid GeoJSON:** Ensure that your GeoJSON file is valid and well-formed.  Use a GeoJSON validator to check for errors.
*   **File Permissions:** Verify that NetViewer has the necessary permissions to read the input GeoJSON file and write the output PNG image.
*   **Tile Server Errors:** If you are using a tile server, ensure that the URL is correct and accessible.  Check for any network connectivity issues.

## Support

For further assistance or to report bugs, please consult the NetViewer documentation or contact our support team.
---
