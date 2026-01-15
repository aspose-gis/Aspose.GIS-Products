---
title: Convert to MGRS
url: /vi/coordinates/convert-to-mgrs/
linkTitle: Chuyển đổi sang MGRS
weight: 10
---

## What is MGRS?
MGRS stands for Military Grid Reference System. It is a global grid coordinate system used by military and civilian organizations to identify locations on the Earth's surface. The MGRS divides the world into squares, each with a unique identifier.

## How to convert coordinates to MGRS?
There are several ways to convert geographic coordinates (latitude and longitude) to MGRS:

*   **Online converters:** There are many online tools that can perform this conversion for you. Some popular options include:
    *   [https://home.apricot.org/mgrp/](https://home.apricot.org/mgrp/)
    *   [https://www.geodaten.de/en/mgrs-converter](https://www.geodaten.de/en/mgrs-converter)
*   **GIS software:** Most GIS software packages, such as QGIS and ArcGIS, have built-in tools for converting coordinates to MGRS.
*   **Programming libraries:** There are also programming libraries available in various languages that can perform this conversion programmatically.

## Understanding the MGRS code
An MGRS code is composed of several parts:

*   **Designator:** A three- or four-character string that identifies the grid square's location on the Earth. The first character indicates the zone number, which ranges from 0 to 9. The second character indicates the band number, which ranges from 1 to 9. The third and fourth characters indicate the row and column of the grid square within the zone and band.
*   **Alpha-numeric suffix:** A string of digits and letters that identifies the precise location within the grid square. The first digit represents the easting coordinate, and the second digit represents the northing coordinate.

## Example
For example, the coordinates 34°0'0"N, 118°30'0"W can be converted to the MGRS code `18QG34567`.

*   `18`: Zone number
*   `Q`: Band number
*   `34`: Row number
*   `567`: Column number
---
