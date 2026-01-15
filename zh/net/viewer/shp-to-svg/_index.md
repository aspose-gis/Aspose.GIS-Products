---
title: SHP to SVG Conversion
url: /zh/shp-to-svg/
weight: 10
layout: ""
---

## Overview

This tool converts shapefiles (.shp) into scalable vector graphics (.svg).  SVG is a versatile format suitable for web display and further editing.

## Usage

1.  **Input:** Provide a valid shapefile (.shp).
2.  **Output:** The tool generates an SVG file representing the geometry of the input shapefile.

## Parameters

*   `--input`: Path to the input shapefile. (Required)
*   `--output`: Path to the output SVG file. If not specified, the output will be written to a file with the same name as the input file but with a .svg extension. (Optional)
*   `--simplify`:  A factor for simplifying the geometry. Values between 0 and 1 are recommended. Lower values result in more simplification. (Optional)

## Example

```bash
shp-to-svg --input my_shapefile.shp --output my_shapefile.svg --simplify 0.5
```

This command converts `my_shapefile.shp` to `my_shapefile.svg`, simplifying the geometry by a factor of 0.5.

## Error Handling

The tool will exit with an error message if:

*   The input file is not a valid shapefile.
*   The output directory does not exist.
*   Any other unexpected errors occur during processing.

## Notes

*   The accuracy of the conversion depends on the complexity of the shapefile and the simplification factor used.
*   Large shapefiles may take a significant amount of time to convert.
*   Ensure that all necessary files for the shapefile (e.g., .dbf, .shx) are present in the same directory as the .shp file.

## 转换概述

该工具将形状文件 (.shp) 转换为可缩放矢量图形 (.svg)。 SVG 是一种通用的格式，适用于网页显示和进一步编辑。

## 用法

1.  **输入：** 提供有效的形状文件 (.shp)。
2.  **输出：** 该工具生成一个表示输入形状文件的几何图形的 SVG 文件。

## 参数

*   `--input`: 输入形状文件的路径。（必需）
*   `--output`: 输出 SVG 文件的路径。 如果未指定，则将输出写入与输入文件同名但扩展名为 .svg 的文件。（可选）
*   `--simplify`: 用于简化几何图形的因子。建议使用介于 0 和 1 之间的值。较低的值会导致更多简化。（可选）

## 示例

```bash
shp-to-svg --input my_shapefile.shp --output my_shapefile.svg --simplify 0.5
```

此命令将 `my_shapefile.shp` 转换为 `my_shapefile.svg`，并将几何图形简化因子为 0.5。

## 错误处理

如果出现以下情况，该工具将显示错误消息并退出：

*   输入文件不是有效的形状文件。
*   输出目录不存在。
*   在处理过程中发生任何其他意外错误。

## 注意事项

*   转换的准确性取决于形状文件的复杂性和使用的简化因子。
*   大型形状文件可能需要相当长的时间才能转换。
*   确保所有必要的形状文件（例如，.dbf、.shx）都存在于与 .shp 文件相同的目录中。

---
