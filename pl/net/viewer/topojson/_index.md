---
title: TopoJSON Viewer
linkTitle: Przeglądarka TopoJSON
weight: 10
url: /pl/net/viewer/topojson/
description: View and interact with TopoJSON data.
---

## Introduction

TopoJSON is a format for representing geographic features as JSON objects. It's a compressed version of GeoJSON, which makes it more efficient to store and transmit. This viewer allows you to visualize and interact with TopoJSON data on a map.

## Features

*   Display TopoJSON data on an interactive map
*   Zoom and pan the map
*   View feature properties as popups
*   Support for various color schemes and styling options
*   Ability to filter features based on their properties

## Usage

1.  Load a TopoJSON file using the "Load" button.
2.  The map will automatically zoom to the extent of the data.
3.  Click on a feature to view its properties in a popup.
4.  Use the controls in the top-left corner to adjust the color scheme and styling options.

## Example

Here's an example of how to use the TopoJSON viewer:

```javascript
// Load the TopoJSON data
fetch('your_topojson_file.json')
    .then(response => response.json())
    .then(data => {
        // Create a map object
        const map = new Map({
            container: 'map', // The ID of the HTML element where the map will be rendered
            center: [0, 0],   // Initial map center coordinates
            zoom: 2           // Initial zoom level
        });

        // Add the TopoJSON data to the map
        map.addLayer({
            type: 'topojson',
            source: data,
            layerOptions: {
                getProperty: d => ({
                    name: d.properties.name
                })
            }
        });
    });
```

## Customization

The TopoJSON viewer can be customized using a variety of options. See the documentation for more details.

## Troubleshooting

If you encounter any problems with the TopoJSON viewer, please consult the troubleshooting guide or contact support.

---
