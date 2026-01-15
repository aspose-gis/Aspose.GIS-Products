---
title: Convert OSM to PNG
url: /ru/net/viewer/osm-to-png/
weight: 10
layout: single
draft: false
description: Convert OpenStreetMap data to PNG images.
---

## Overview

This tool converts OpenStreetMap (OSM) data to PNG images. It allows you to specify the area of interest, zoom level, and other rendering options.

## Usage

The tool can be used from the command line or as a web service.

### Command Line Usage

```bash
osm-to-png --bbox="37.7,-122.4,37.8,-122.3" --zoom=12 --output="san_francisco.png"
# Преобразует данные OpenStreetMap в PNG изображение для заданной области и уровня масштабирования.
```

### Web Service Usage

The web service exposes a REST API for converting OSM data to PNG images.

#### Parameters

*   `bbox`: The bounding box of the area to render, in the format "southWestLat,southWestLng,northEastLat,northEastLng".
*   `zoom`: The zoom level of the map.
*   `output`: The name of the output PNG file.

#### Example Request

```bash
curl "http://localhost:8080/convert?bbox=37.7,-122.4,37.8,-122.3&zoom=12&output=san_francisco.png"
# Отправляет запрос к веб-сервису для преобразования данных OpenStreetMap в PNG изображение.
```

## Options

The tool supports the following options:

*   `--bbox`: The bounding box of the area to render.
*   `--zoom`: The zoom level of the map.
*   `--output`: The name of the output PNG file.
*   `--width`: The width of the output image in pixels.
*   `--height`: The height of the output image in pixels.
*   `--format`: The output format (png, jpg, gif).

## Configuration

The tool can be configured using a configuration file. The configuration file should be located at `/etc/osm-to-png/config.ini`.

### Example Configuration File

```ini
[OsmToPng]
bbox = "37.7,-122.4,37.8,-122.3"
zoom = 12
output = "san_francisco.png"
width = 512
height = 512
format = png
# Пример конфигурационного файла для настройки параметров преобразования данных OpenStreetMap в PNG изображение.
```

## Troubleshooting

If you encounter any problems, please consult the following resources:

*   [FAQ](https://example.com/faq)
*   [Documentation](https://example.com/documentation)
*   [Support Forum](https://example.com/forum)

---
