---
title: GeoTIFF to SVG Conversion
url: /ja/viewer/geotiff-to-svg/
weight: 10
layout: ""
---

## Converting GeoTIFFs to SVGs

This tool allows you to convert GeoTIFF images into scalable vector graphics (SVGs).  SVGs are ideal for web mapping applications and other scenarios where crisp, resolution-independent imagery is required.

### Input Requirements

*   **GeoTIFF File:** A valid GeoTIFF file containing raster data.
*   **Resolution:** The desired resolution of the output SVG in dots per inch (DPI).  Higher resolutions result in larger file sizes but more detail.
*   **Color Map (Optional):** If your GeoTIFF uses a color map, you can provide a CSV file that defines the color mapping between data values and RGB colors.

### Conversion Process

1.  **Upload GeoTIFF:** Upload your GeoTIFF file using the file selection control.
2.  **Set Resolution:** Specify the desired resolution (DPI) for the output SVG. A default value is provided, but you can adjust it as needed.
3.  **Provide Color Map (Optional):** If applicable, upload a CSV file containing your color map data. The CSV should have three columns: `value`, `r`, and `g`. The third column `b` is optional.
4.  **Convert:** Click the "Convert" button to start the conversion process.
5.  **Download SVG:** Once the conversion is complete, a link will appear allowing you to download the resulting SVG file.

### Example Color Map CSV

```csv
value,r,g,b
0,255,0,0
1,0,255,0
2,0,0,255
```

### Troubleshooting

*   **Invalid GeoTIFF:** Ensure that the uploaded file is a valid GeoTIFF.  Check for corruption or unsupported data types.
*   **Resolution Errors:** If you encounter errors related to resolution, try adjusting the DPI value. Very high resolutions can lead to memory issues.
*   **Color Map Issues:** Verify that your color map CSV file is properly formatted and contains accurate color mappings.

### Limitations

*   The conversion process may be slow for very large GeoTIFF files.
*   Complex GeoTIFFs with many bands or unusual data types may not convert correctly.

