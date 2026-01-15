---
title: GPX to JPEG Conversion
url: /uk/net/viewer/gpx-to-jpeg/
weight: 10
layout: ""
---

## Convert GPX data to JPEGs

This tool allows you to convert GPX (GPS Exchange Format) data into a series of JPEG images. Each image represents a segment of the GPS track, with markers indicating key points like waypoints or significant changes in direction.

### Prerequisites

*   [.NET](https://dotnet.microsoft.com/en-us/) 6.0 or later
*   [ImageSharp](https://imageSharp.github.io/) library (included as a dependency)

### Usage

1.  **Input GPX File:** Provide the path to your GPX file.
2.  **Output Directory:** Specify the directory where the generated JPEG images will be saved.
3.  **Image Width and Height:** Define the desired width and height of the output images in pixels.
4.  **Distance per Image:** Set the distance (in meters) that should be represented by each image. Shorter distances result in more detailed images, while longer distances provide a broader overview.

### Command-Line Arguments

The tool accepts the following command-line arguments:

*   `-i` or `--input`: Path to the input GPX file.
*   `-o` or `--output`: Directory for output JPEG files.
*   `-w` or `--width`: Width of the output images in pixels.
*   `-h` or `--height`: Height of the output images in pixels.
*   `-d` or `--distance`: Distance per image in meters.

### Example

```bash
gpx-to-jpeg -i "path/to/your/file.gpx" -o "output_images" -w 800 -h 600 -d 100
```

This command will convert `file.gpx` into JPEG images, saving them to the `output_images` directory. Each image will be 800 pixels wide and 600 pixels high, representing a distance of 100 meters along the GPS track.

### Configuration Options (appsettings.json)

The tool's behavior can be further customized through an `appsettings.json` file.  Here are some key configuration options:

*   `MapTileServerUrl`: URL of the map tile server to use for background imagery.
*   `DefaultDistancePerImage`: Default distance per image if not specified on the command line.
*   `DefaultWidth`: Default width of output images.
*   `DefaultHeight`: Default height of output images.

### Output Images

The generated JPEG images will include:

*   A map background (using the configured `MapTileServerUrl`).
*   GPS track overlaid on the map.
*   Markers indicating waypoints and significant changes in direction.
*   Metadata embedded in the image file, including start time, end time, total distance, and maximum elevation.

### Error Handling

The tool provides informative error messages for common issues such as:

*   Invalid input GPX file format.
*   Insufficient permissions to write to the output directory.
*   Invalid command-line arguments.

### Known Issues

*   Performance may be slow for very large GPX files.
*   Map tile server availability can affect image generation.

---
