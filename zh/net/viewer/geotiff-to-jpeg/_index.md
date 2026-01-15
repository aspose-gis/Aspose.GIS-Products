---
title: GeoTIFF to JPEG Conversion
url: /zh/geotiff-to-jpeg/
weight: 10
layout: ""
---

## Overview ##

This guide explains how to convert GeoTIFF files to JPEG format using various methods and tools.  GeoTIFF is a popular raster data format commonly used in geographic information systems (GIS) for storing georeferenced raster imagery. JPEGs, on the other hand, are widely used for displaying images due to their smaller file sizes.

## Why Convert GeoTIFF to JPEG? ##

*   **Smaller File Size:** JPEGs generally have smaller file sizes compared to GeoTIFFs, making them easier to share and store.
*   **Web Compatibility:** JPEGs are universally supported by web browsers, allowing for easy display of raster imagery online.
*   **Display Purposes:** For simple visualization purposes, a JPEG often suffices and avoids the overhead of carrying georeferencing information.

## Methods ##

Here are several methods to convert GeoTIFF files to JPEG format:

### 1. GDAL ###

GDAL (Geospatial Data Abstraction Library) is a powerful open-source library for working with geospatial data. It provides command-line tools that can be used to perform various conversions, including GeoTIFF to JPEG.

**Command:**

```bash
gdal_translate -of JPEG input.tif output.jpg
```

*   `-of JPEG`: Specifies the output format as JPEG.
*   `input.tif`: The name of the input GeoTIFF file.
*   `output.jpg`: The name of the output JPEG file.

**Options:**

*   `-co "QUALITY=value"`:  Sets the JPEG quality (0-100, higher is better). For example `-co "QUALITY=90"`.
*   `-ot BYTE`: Forces the output to be an 8-bit image. Useful for reducing file size further.

### 2. QGIS ###

QGIS is a free and open-source Geographic Information System that provides a graphical user interface for working with geospatial data. It can also be used to convert GeoTIFF files to JPEG format.

**Steps:**

1.  Open the GeoTIFF file in QGIS.
2.  Go to "Raster" -> "Export" -> "Save As...".
3.  Select "JPEG" as the output format.
4.  Specify the output filename and location.
5.  Adjust quality settings if desired.
6.  Click "OK" to start the conversion.

### 3. Online Converters ###

Several online converters can convert GeoTIFF files to JPEG format without requiring any software installation. However, be cautious when using online converters, especially with sensitive data.

**Example:**

*   CloudConvert ([https://cloudconvert.com/geotiff-to-jpg](https://cloudconvert.com/geotiff-to-jpg))

### 4. Python with Rasterio and Pillow ###

You can use the Rasterio library to read GeoTIFF files and the Pillow (PIL) library to save them as JPEGs in Python.

```python
import rasterio
from rasterio import plot
from pillow import Image

def geotiff_to_jpeg(input_path, output_path):
    """Converts a GeoTIFF file to JPEG format."""
    try:
        with rasterio.open(input_path) as src:
            image = src.read() # Read all bands into an array

        # Convert the NumPy array to a Pillow Image object
        img = Image.fromarray((image[0] * 255).astype('uint8'))  # Assuming single band, scale and convert

        img.save(output_path, "JPEG")
        print(f"Successfully converted {input_path} to {output_path}")

    except Exception as e:
        print(f"Error converting {input_path}: {e}")

# Example usage:
geotiff_to_jpeg("input.tif", "output.jpg")
```

## Considerations ##

*   **Georeferencing:** Converting to JPEG removes the georeferencing information embedded in the GeoTIFF file. If you need to preserve this information, consider using a different output format like PNG or TIFF.
*   **Quality:**  JPEG is a lossy compression format, meaning that some image data is lost during compression. Adjust the quality settings to balance file size and image quality.
*   **Color Depth:** GeoTIFFs can have varying color depths (e.g., 8-bit, 16-bit). Ensure that the output JPEG has an appropriate color depth for your needs.

## Troubleshooting ##

*   **Error: "Unsupported format"**:  Make sure you have the necessary libraries installed (e.g., GDAL, Rasterio).
*   **Large file size:** Try reducing the JPEG quality or using a different compression method.
*   **Image distortion:** Check that the input GeoTIFF is properly georeferenced and that the conversion process is not introducing any distortions.

---
