---
title: MapInfo MIF
linkTitle: 地図情報MIF
weight: 10
url: /ja/net/viewer/mapinfo-mif/
aliases: [mif, mapinfo]
---

## What is MIF?
MIF (Map Info Format) is a text file format used by MapInfo to store geographic data. It's often paired with an ATB (Attribute Table Binary) file which contains the attribute information for each feature in the MIF file.

## Supported Versions
The viewer supports the following versions of MIF:

*   ESRI MIF
*   MapInfo MIF

## Usage
To use a MIF file, you need both the MIF and ATB files. The viewer will automatically load both files if they are in the same directory and have the same base name (e.g., "mydata.mif" and "mydata.atb").

## Example
Here's an example of a simple MIF file:

```
0
100 100 0 1 1 0 0 0 255 255 255
1 10 10
```

This file defines a single polygon with the following properties:

*   Type: Polygon (0)
*   X coordinates: 100, 100
*   Y coordinates: 0, 1, 1, 0
*   Description: "My Polygon"

## Notes
*   The viewer assumes that the X and Y coordinates are in the same units.
*   The viewer does not support all features of the MIF format.
*   If you encounter any issues, please refer to the MapInfo documentation for more information.

## 補足
*   ビューアはXおよびY座標が同じ単位であることを前提としています。
*   ビューアはMIF形式のすべての機能に対応していません。
*   問題が発生した場合は、詳細についてはMapInfoドキュメントを参照してください。
---
