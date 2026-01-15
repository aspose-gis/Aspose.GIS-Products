---
title: Shapefile to PNG Conversion
url: /zh/shapefile-to-png/
weight: 10
layout: ""
---

## Converting Shapefiles to PNG Images

This guide explains how to convert shapefiles (.shp) into Portable Network Graphics (.png) images using Python and the `ogr` library (part of GDAL).  Shapefiles are a common format for storing geospatial vector data, while PNG is a widely used image format. This process allows you to create raster representations of your spatial data for use in reports, presentations, or web applications.

### Prerequisites

Before you begin, ensure you have the following installed:

*   **Python:**  Version 3.6 or higher is recommended.
*   **GDAL (with `ogr`):** GDAL provides geospatial data abstraction library functionality. The `ogr` module specifically handles vector data operations. You can install it using pip:

    ```bash
    pip install gdal
    ```

### Python Script

Here's a Python script that performs the conversion:

```python
# This script converts a shapefile to a PNG image.
import os
from osgeo import ogr, gdal

def shapefile_to_png(shapefile_path, output_image_path):
    """
    Converts a shapefile to a PNG image.

    Args:
        shapefile_path (str): Path to the input shapefile (.shp).
        output_image_path (str): Path to save the output PNG image.
    """
    try:
        # Open the shapefile
        datasource = ogr.Open(shapefile_path)
        if datasource is None:
            raise Exception("Could not open {}".format(shapefile_path))

        layer = datasource.GetLayer()
        geom_type = layer.GetGeometryType()

        # Determine extent and resolution based on shapefile bounds
        minx, miny, maxx, maxy = layer.GetExtent()
        width = maxx - minx
        height = maxy - miny
        resolution = width / 256  # Adjust as needed for desired image size

        # Create the output raster dataset
        driver = gdal.GetDriverByName('PNG')
        if driver is None:
            raise Exception("Could not create PNG driver")

        dataset = driver.Create(output_image_path, int(width / resolution), int(height / resolution), 1, gdal.GDT_Byte)
        if dataset is None:
            raise Exception("Could not create {}".format(output_image_path))

        # Set geotransform and projection
        geotransform = (minx, resolution, 0, maxy, 0, -resolution)
        dataset.SetGeoTransform(geotransform)
        projection = layer.GetProjection()
        dataset.SetProjection(projection)

        # Create a color table for single band raster
        color_table = gdal.ColorTable()
        color_table.CreateColorRamp(0, 255, (0, 0, 0), (255, 255, 255))  # Black to White
        dataset.GetRasterBand(1).SetColorInterpretation(gdal.GCI_PaletteIndex)
        dataset.GetRasterBand(1).SetColorTable(color_table)

        # Rasterize the shapefile features
        band = dataset.GetRasterBand(1)
        band.WriteArray(rasterize_shapefile(layer, resolution))

        # Set metadata (optional)
        dataset.SetMetadataItem('STATISTICS_MIN', '0')
        dataset.SetMetadataItem('STATISTICS_MAX', '255')

        # Flush cache and close the dataset
        band.FlushCache()
        dataset = None  # Close the file

    except Exception as e:
        print(e)


def rasterize_shapefile(layer, resolution):
    """
    Rasterizes a shapefile layer to a numpy array.

    Args:
        layer (ogr.Layer): The OGR layer to rasterize.
        resolution (float): The pixel size for rasterization.

    Returns:
        numpy.ndarray: A 2D numpy array representing the rasterized image.
    """
    # Create an empty raster band
    width = int(layer.GetExtent()[2] - layer.GetExtent()[0]) // resolution
    height = int(layer.GetExtent()[3] - layer.GetExtent()[1]) // resolution
    raster_array = [[0 for _ in range(width)] for _ in range(height)]

    # Iterate through features and rasterize them
    for feature in layer:
        geometry = feature.GetGeometry()
        if geometry is not None:
            x, y = geometry.ExportToWkt().split(',')
            x = float(x)
            y = float(y)

            # Calculate pixel coordinates
            px = int((x - layer.GetExtent()[0]) // resolution)
            py = int((y - layer.GetExtent()[1]) // resolution)

            # Set the pixel value to 1 (or any other desired value)
            if px >= 0 and px < width and py >= 0 and py < height:
                raster_array[py][px] = 255  # Assign a value for visualization

    return raster_array


# Example usage:
shapefile_path = "path/to/your/shapefile.shp" # Replace with your shapefile path
output_image_path = "output.png" # Replace with desired output path
shapefile_to_png(shapefile_path, output_image_path)
```

### Explanation

1.  **Import Libraries:** Imports necessary modules from `osgeo` (GDAL/OGR).
2.  **`shapefile_to_png()` Function:** This function encapsulates the entire conversion process. It takes the shapefile path and desired output image path as input.
3.  **Open Shapefile:** Opens the specified shapefile using `ogr.Open()`. Error handling is included to check if the file can be opened successfully.
4.  **Determine Extent & Resolution:** Calculates the extent (bounding box) of the shapefile and determines an appropriate resolution for the output image. The resolution controls the level of detail in the resulting PNG.
5.  **Create Output Raster:** Creates a new raster dataset using `gdal.GetDriverByName('PNG')`. This creates the empty PNG file that will be populated with pixel data.
6.  **Set Geotransform & Projection:** Sets the geotransform and projection information for the output raster, ensuring it is properly associated with its geographic location.
7.  **Create Color Table:** Creates a color table to map pixel values to colors. In this example, it creates a simple black-to-white ramp.
8.  **Rasterize Shapefile Features:** The `rasterize_shapefile()` function iterates through each feature in the shapefile and assigns a pixel value based on its geometry. This effectively "burns" the vector data into the raster image.
9.  **Set Metadata (Optional):** Sets metadata items for the raster, such as statistics about the pixel values.
10. **Flush Cache & Close:** Flushes the cache to write any remaining data to disk and closes the dataset.

### Running the Script

1.  **Save the script:** Save the Python code above as a `.py` file (e.g., `shapefile_to_png.py`).
2.  **Modify paths:** Update the `shapefile_path` and `output_image_path` variables in the script to reflect the actual location of your shapefile and desired output PNG image.
3.  **Execute the script:** Run the script from your terminal using:

    ```bash
    python shapefile_to_png.py
    ```

### Considerations

*   **Resolution:** Adjust the `resolution` variable to control the size and detail of the output image. Smaller values result in higher resolution images but also larger file sizes.
*   **Color Table:** Customize the color table to change the appearance of the rasterized features.  You can use different colors or create more complex ramps.
*   **Feature Attributes:** The script currently assigns a single pixel value (255) to each feature. You could modify it to map attribute values from the shapefile to different pixel values, creating thematic maps.
*   **Large Shapefiles:** For very large shapefiles, rasterization can be memory-intensive. Consider processing the data in smaller chunks or using a more efficient rasterization algorithm.

---

