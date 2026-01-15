---
title: המרת נתוני GIS ב-#C
url: /he/net/conversion/
description: המרת נתוני GIS בפורמטים שונים כולל GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM עם כמה שורות קוד #C באמצעות ספריית .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="המרת נתוני GIS באמצעות #C" h2="המרת GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM לבניית יישומי .NET מבוססי פלטפורמה." >}}

{{% blocks/products/pf/feature-page-summary %}}


כדי לנתח נתונים מרחביים וגיאוגרפיים, API של GIS ב-.NET מקל על בניית פתרונות לכידת, אחסון, ניהול, מניפולציה, ניתוח והצגה של כל סוגי הנתונים הגיאוגרפיים. הוא לא רק טוען פורמטים שונים של וקטור וראסטר אלא גם מעביר אותם לפורמטים אחרים בקלות. כמה מתרחישי העיבוד כגון **GeoJSON ל-Shapefile** , **GeoJSON ל-topojson**, **GeoJSON ל-kml**, **Shapefile ל-GeoJSON** ויותר. עבור כל יישום עיבוד מידע גיאוגרפי מבלי לדרוש כלים או תוכנה נוספים, API של GIS ב-.NET מסוגל לעבוד עם מספר מאפיינים גיאומטריים, פשוטים או מורכבים כאחד.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="המרת GeoJSON ל-Shapefile SHP" %}}

עם כמה שורות קוד בלבד, מפתחים יכולים להמיר נתוני GeoJSON לקובץ Shapefile SHP. ה-API מספק [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)

{{% blocks/products/pf/feature-page-code h3="קוד #C להמרת GeoJSON ל-Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="המרת Shapefile ל-GeoJSON" %}}

תהליך המרת Shapefile ל-GeoJSON זהה לקודם על ידי שימוש ב-VectorLayer והפעלת [שיטת ההמרה](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) עם פרמטרים רלוונטיים.

{{% blocks/products/pf/feature-page-code h3="קוד #C להמרת נתוני Shapefile ל-GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="המרת KML ל-GeoJSON" %}}

באמצעות שיטת VectorLayer.Convert עם פרמטרים מתאימים, קובץ מקור KML, מנהל התוכנית KML מתוך [מחלקת Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers), נתיב קובץ GeoJSON ומנהל התוכנית GeoJSON, מפתחים יכולים להמיר בקלות את KML לנתוני GeoJSON.

{{% blocks/products/pf/feature-page-code h3="קוד #C להמרת KML ל-GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
