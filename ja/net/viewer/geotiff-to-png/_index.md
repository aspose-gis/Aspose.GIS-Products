---
title: GeoTIFF to PNG Conversion
url: /ja/viewer/geotiff-to-png/
weight: 10
layout: ""
---

## Converting GeoTIFF to PNG with the NetViewer

The NetViewer provides a simple and efficient way to convert GeoTIFF files into PNG images. This process is crucial for displaying raster data on web maps and other applications where PNG format is preferred.

### Prerequisites

*   A valid GeoTIFF file.
*   Access to the NetViewer application.

### Conversion Process

1.  **Upload GeoTIFF:** Upload your GeoTIFF file through the NetViewer interface.
2.  **Configure Parameters:** Specify the desired output parameters, such as:
    *   **Resolution:** Adjust the resolution of the PNG image. Higher resolutions result in larger files but more detail.
    *   **Color Palette:** Select a color palette for converting the GeoTIFF's raster values into colors.
    *   **Contrast Stretching:** Apply contrast stretching to enhance the visual clarity of the data.
3.  **Initiate Conversion:** Start the conversion process by clicking the "Convert" button.
4.  **Download PNG:** Once the conversion is complete, download the resulting PNG image.

### Code Example (Python)

```python
# This script demonstrates how to convert a GeoTIFF file to a PNG image using Python and GDAL.
# 変換スクリプトの例（Python）
# このスクリプトは、PythonとGDALを使用してGeoTIFFファイルをPNG画像に変換する方法を示しています。

import gdal

def geotiff_to_png(geotiff_path, png_path):
    """Converts a GeoTIFF file to a PNG image.

    Args:
        geotiff_path (str): Path to the input GeoTIFF file.
        png_path (str): Path to the output PNG file.
    """
    try:
        dataset = gdal.Open(geotiff_path)
        if dataset is None:
            raise Exception("Could not open {}".format(geotiff_path))

        band = dataset.GetRasterBand(1)  # Assuming single-band GeoTIFF
        array = band.ReadAsArray()

        driver = gdal.GetDriverByName('PNG')
        if driver is None:
            raise Exception("Could not create PNG driver")

        dataset_png = driver.Create(png_path, array.shape[1], array.shape[0], 1, gdal.GDT_Byte)
        if dataset_png is None:
            raise Exception("Could not create {}".format(png_path))

        band_png = dataset_png.GetRasterBand(1)
        band_png.WriteArray(array)

        dataset_png = None
        dataset = None

        print("Successfully converted {} to {}".format(geotiff_path, png_path))

    except Exception as e:
        print("Error converting GeoTIFF to PNG: {}".format(e))

# Example usage:
# 例：
# geotiff_to_png('input.tif', 'output.png')
```

### Troubleshooting

*   **File Size:** Large GeoTIFF files may result in very large PNG images. Consider reducing the resolution or using compression techniques.
*   **Color Palette Issues:** If the color palette doesn't accurately represent the data, adjust the contrast stretching parameters.
*   **Conversion Errors:** Check for file corruption or unsupported GeoTIFF formats.

### Additional Resources

*   [GDAL Documentation](http://gdal.org/en/index.html)
*   [NetViewer User Guide](linkTitle: NetViewer ユーザーガイド link /ja/user-guide/)
