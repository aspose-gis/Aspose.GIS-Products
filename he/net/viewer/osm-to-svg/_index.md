---
title: osm-to-svg
url: /he/osm-to-svg/
weight: 10
layout: ""
---

## osm-to-svg

### Description

The `osm-to-svg` tool converts OpenStreetMap (OSM) data to Scalable Vector Graphics (SVG) format. This allows for easy visualization and manipulation of OSM data within vector graphics editors or web browsers.

### Usage

```bash
osm-to-svg [options] <input_file> > <output_file>.svg
```

#### Options

*   `-k`: Key to filter by.  For example, `-k amenity` would only include features with the `amenity` tag.
*   `-a`: Attribute to filter by. Used in conjunction with `-k`. For example, `-k amenity -a restaurant` would only include restaurants.
*   `-b`: Bounding box (minx, miny, maxx, maxy).  Limits the area extracted from the OSM data.
*   `-o`: Output file name prefix.
*   `-s`: Scale factor. Adjusts the size of the SVG output.
*   `-l`: Layer name. Specifies a layer name for the SVG elements.
*   `--verbose`: Enables verbose output, showing the progress and details of the conversion process.

### Example

To convert an OSM file to SVG, filtering by restaurants:

```bash
osm-to-svg -k amenity -a restaurant input.osm > restaurants.svg
```

This command reads `input.osm`, filters for features with the tag `amenity=restaurant`, and saves the result as `restaurants.svg`.

### Notes

*   The input file should be a valid OSM XML file.
*   The output SVG file will contain vector data representing the selected OSM features.
*   Consider using a large scale factor to ensure sufficient detail in the resulting SVG.
*   Filtering by key and attribute can significantly reduce the size of the output SVG, especially for large OSM datasets.

### תיאור

הכלי `osm-to-svg` ממיר נתוני OpenStreetMap (OSM) לפורמט Scalable Vector Graphics (SVG). זה מאפשר הדמיה ושינוי קלים של נתוני OSM בעורך גרפיקה וקטורית או בדפדפן אינטרנט.

### שימוש

```bash
osm-to-svg [אפשרויות] <קובץ_קלט> > <קובץ_פלט>.svg
```

#### אפשרויות

*   `-k`: מפתח לסנן לפי. לדוגמה, `-k amenity` יכלול רק תכונות עם התג `amenity`.
*   `-a`: מאפיין לסנן לפי. משמש בשילוב עם `-k`. לדוגמה, `-k amenity -a restaurant` יכלול רק מסעדות.
*   `-b`: תיבת גבול (minx, miny, maxx, maxy). מגבילה את האזור המופק מנתוני ה-OSM.
*   `-o`: קידומת שם קובץ פלט.
*   `-s`: גורם קנה מידה. משנה את גודל הפלט של ה-SVG.
*   `-l`: שם שכבה. מציין שם שכבה עבור אלמנטי ה-SVG.
*   `--verbose`: מאפשר פלט מפורט, המציג את התקדמות ותהליך ההמרה.

### דוגמה

כדי להמיר קובץ OSM ל-SVG, תוך סינון לפי מסעדות:

```bash
osm-to-svg -k amenity -a restaurant input.osm > restaurants.svg
```

פקודה זו קוראת את `input.osm`, מסננת תכונות עם התג `amenity=restaurant` ושומרת את התוצאה כ-`restaurants.svg`.

### הערות

*   קובץ הקלט צריך להיות קובץ XML OSM תקף.
*   קובץ ה-SVG הפלט יכיל נתוני וקטור המייצגים את תכונות ה-OSM הנבחרות.
*   שקול להשתמש בגורם קנה מידה גדול כדי להבטיח מספיק פרטים בפלט ה-SVG המתקבל.
*   סינון לפי מפתח ומאפיין יכול להפחית משמעותית את גודל קובץ ה-SVG, במיוחד עבור מערכי נתונים גדולים של OSM.
---
