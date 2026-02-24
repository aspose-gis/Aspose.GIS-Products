---
title: تبدیل داده‌های GIS در C#
url: /fa/net/conversion/
description: تبدیل داده‌های GIS در فرمت‌های مختلف از جمله GeoJSON، ESRI Shapefile SHX، TopoJSON، FIleGDB، GML، KML، MIF، OSM با چند خط کد C# از طریق کتابخانه .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="تبدیل داده‌های GIS از طریق C#" h2="تبدیل GeoJSON، ESRI Shapefile SHX، TopoJSON، FIleGDB، GML، KML، MIF، OSM به منظور ایجاد برنامه‌های .NET چند پلتفرمی." >}}

{{% blocks/products/pf/feature-page-summary %}}


برای تجزیه و تحلیل داده‌های مکانی و جغرافیایی، API GIS .NET امکان ساخت راه حل‌هایی را برای گرفتن، ذخیره، مدیریت، دستکاری، تجزیه و تحلیل و ارائه انواع مختلف داده‌های جغرافیایی فراهم می‌کند. این API نه تنها فرمت‌های برداری و رستری مختلف را بارگیری می‌کند، بلکه به راحتی آن‌ها را به سایر فرمت‌ها تبدیل می‌کند. چند سناریو از تبدیل مانند **GeoJSON به Shapefile** ، **GeoJSON به topojson** ، **GeoJSON به kml** ، **Shapefile به GeoJSON** و موارد بیشتر. برای هر برنامه رندر اطلاعات جغرافیایی بدون نیاز به ابزار یا نرم افزار اضافی، API GIS .NET قابلیت کار با تعداد زیادی از ویژگی‌های هندسی را چه ساده و چه پیچیده دارد.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="تبدیل GeoJSON به Shapefile SHP" %}}

با تنها چند خط کد، توسعه دهندگان می‌توانند داده‌های GeoJSON را به فایل Shapefile SHP تبدیل کنند. API [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(مسیر فایل داده GeoJSON منبع، GeoJson، مسیر Shapefile مقصد، Shapefile) را ارائه می‌دهد

{{% blocks/products/pf/feature-page-code h3="کد C# برای تبدیل GeoJSON به Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="تبدیل Shapefile به GeoJSON" %}}

فرآیند تبدیل Shapefile به GeoJSON همانند مورد بالا با استفاده از VectorLayer و فراخوانی متد [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) با پارامترهای مربوطه است.


{{% blocks/products/pf/feature-page-code h3="کد C# برای تبدیل داده‌های Shapefile به GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="تبدیل KML به GeoJSON" %}}

با استفاده از متد VectorLayer.Convert با پارامترهای مناسب، فایل منبع KML، درایور KML از [کلاس Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers)، مسیر فایل GeoJSON و درایور GeoJSON، توسعه دهندگان می‌توانند به راحتی KML را به داده‌های GeoJSON تبدیل کنند.

{{% blocks/products/pf/feature-page-code h3="کد C# برای تبدیل KML به GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
