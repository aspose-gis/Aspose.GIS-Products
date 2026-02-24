---
title: KML to PNG Conversion
linkTitle: KML을 PNG로 변환하기
weight: 10
url: /ko/net/viewer/kml-to-png/
aliases: [KML을 이미지로 변환, KML을 그림으로 저장]
description: Convert KML files to PNG images.
---

## Overview

This tool converts KML (Keyhole Markup Language) files into PNG image format. It's useful for visualizing geographic data and creating static maps from dynamic KML sources.

## Requirements

*   .NET runtime
*   GDAL library

## Usage

1.  **Input KML file:** Provide the path to your KML file.
2.  **Output PNG file:** Specify the desired filename for the output PNG image.
3.  **Map parameters:** Configure map settings such as center coordinates, zoom level, and image size.

## Parameters

*   `-i`, `--input`: Path to the input KML file.
*   `-o`, `--output`: Path to the output PNG file.
*   `--center-lat`: Latitude of the map center (default: 40.7128).
*   `--center-lon`: Longitude of the map center (default: -74.0060).
*   `--zoom`: Zoom level of the map (default: 10).
*   `--width`: Width of the output image in pixels (default: 800).
*   `--height`: Height of the output image in pixels (default: 600).

## Examples

### Basic Conversion

```bash
kml-to-png -i input.kml -o output.png
```

이 명령은 `input.kml` 파일을 `output.png`로 변환합니다. 기본 지도 설정이 사용됩니다.

### Custom Map Parameters

```bash
kml-to-png -i input.kml -o output.png --center-lat 37.7749 --center-lon -122.4194 --zoom 12 --width 1024 --height 768
```

이 명령은 `input.kml` 파일을 `output.png`로 변환하고, 지도 중심을 37.7749 위도와 -122.4194 경도로 설정하며, 확대 수준을 12로 설정하고, 이미지 크기를 1024x768 픽셀로 설정합니다.

## Troubleshooting

*   **GDAL library not found:** Ensure that the GDAL library is installed and accessible in your system's PATH environment variable.
*   **Invalid KML file:** Verify that the input KML file is valid and well-formed.
*   **Output file already exists:**  The tool will overwrite existing files by default. Consider using a unique filename or deleting the existing file before running the conversion.

## Notes

*   The quality of the output PNG image depends on the zoom level and image size parameters. Experiment with different settings to achieve the desired results.
*   Large KML files may take longer to convert.
*   This tool is intended for simple KML-to-PNG conversions. For more complex mapping tasks, consider using dedicated GIS software.

## License

[MIT License](LICENSE)

---
