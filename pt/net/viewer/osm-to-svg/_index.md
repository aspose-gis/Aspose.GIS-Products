---
title: OSM to SVG Viewer
linkTitle: Visualizador de OSM para SVG
weight: 10
url: /pt/net/viewer/osm-to-svg/
description: A viewer for converting OpenStreetMap data to Scalable Vector Graphics (SVG).
---

## Overview

Um visualizador para converter dados do OpenStreetMap em Gráficos Vetoriais Escaláveis (SVG).

## Features

*   Convert OpenStreetMap data to SVG format.
*   Zoom and pan the map.
*   View individual features with detailed information.
*   Filter features by type.
*   Download the generated SVG file.

## Usage

1.  Enter an OpenStreetMap URL or a bounding box.
2.  Specify the desired output resolution.
3.  Click "Convert".
4.  Zoom and pan the map to view the converted data.
5.  Download the SVG file.

## Configuration

The viewer can be configured using the following options:

*   `osmUrl`: The URL of the OpenStreetMap data source.
*   `resolution`: The resolution of the output SVG file (in pixels).
*   `minZoom`: The minimum zoom level for the map.
*   `maxZoom`: The maximum zoom level for the map.

## Example

```javascript
// Exemplo de configuração
const config = {
  osmUrl: "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
  resolution: 512,
  minZoom: 0,
  maxZoom: 18,
};
```

## Troubleshooting

If you encounter any issues, please check the following:

*   Make sure that the OpenStreetMap URL is valid.
*   Verify that the resolution setting is appropriate for your needs.
*   Ensure that your browser supports SVG files.

## Support

If you need assistance, please contact us at [support email address].
---
