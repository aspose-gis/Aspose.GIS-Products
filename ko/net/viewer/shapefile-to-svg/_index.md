---
title: Shapefile to SVG Conversion
linkTitle: 도형 파일에서 SVG로 변환하기
weight: 10
url: /ko/net/viewer/shapefile-to-svg/
description: Learn how to convert shapefiles to scalable vector graphics (SVG) format using the NetViewer.
aliases: [shapefile, svg, conversion, netviewer]
---

## Converting Shapefiles to SVG with NetViewer

This guide explains how to convert shapefiles (.shp) into Scalable Vector Graphics (.svg) format using the NetViewer application.  SVG is a versatile vector image format suitable for web display and further editing.

### Prerequisites

*   **NetViewer Installation:** Ensure you have the NetViewer application installed on your system. You can download it from [link to download].
*   **Shapefile (.shp):** Have the shapefile you want to convert readily available.

### Conversion Steps

1.  **Open NetViewer:** Launch the NetViewer application.
2.  **Load Shapefile:** Use the "File" -> "Open" menu option to load your shapefile. Navigate to the directory containing your .shp file and select it.
3.  **SVG Export:** Once the shapefile is loaded, go to "File" -> "Export" -> "Export as SVG".
4.  **Save SVG File:** A dialog box will appear prompting you to choose a location and filename for your exported SVG file. Select a suitable location and provide a name (e.g., "output.svg"). Click the "Save" button.

### Customization Options (if available)

NetViewer may offer options to customize the SVG export process, such as:

*   **Simplify Geometry:** Reduce the complexity of the geometry for smaller file sizes.
*   **Attribute Mapping:** Control how shapefile attributes are represented in the SVG.
*   **Styling:** Apply specific styles (colors, line widths, etc.) to the features in the SVG.  /* 스타일 옵션은 사용 가능한 경우에만 적용됩니다.*/

### Troubleshooting

*   **File Not Found:** Double-check that the shapefile exists at the specified path.
*   **Corrupted Shapefile:** If you encounter errors during loading or export, the shapefile might be corrupted. Try opening it in another GIS application to verify its integrity.
*   **NetViewer Errors:** Consult the NetViewer documentation or support resources for specific error messages.

### Further Resources

*   [NetViewer Documentation](link to netviewer docs)
*   [Shapefile Format Specification](link to shapefile spec)
*   [Scalable Vector Graphics (SVG)](link to svg info)

