---
title: تحويل بيانات نظم المعلومات الجغرافية C#‎
url: /ar/net/conversion/
description: قم بتحويل بيانات نظم المعلومات الجغرافية بتنسيقات مختلفة بما في ذلك GeoJSON وESRI Shapefile SHX وTopoJSON وFIleGDB وGML وKML وMIF وOSM باستخدام بضعة أسطر من كود C#‎ عبر مكتبة .NET.
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="تحويل بيانات نظم المعلومات الجغرافية عبر C#" h2="قم بتحويل GeoJSON وESRI Shapefile SHX وTopoJSON وFIleGDB وGML وKML وMIF وOSM Data لإنشاء تطبيقات .NET متعددة المنصات." >}}

{{% blocks/products/pf/feature-page-summary %}}


لتحليل البيانات المكانية والجغرافية، تسهل واجهة برمجة تطبيقات GIS الخاصة بـ .NET بناء حلول لالتقاط وتخزين وإدارة ومعالجة وتحليل وعرض جميع أنواع البيانات الجغرافية. فهي لا تقوم بتحميل تنسيقات المتجهات والراستر المختلفة فحسب، بل تقوم أيضًا بعرضها بتنسيقات أخرى بسهولة. بعض سيناريوهات العرض مثل **GeoJSON إلى Shapefile** و **GeoJSON إلى topojson** و **GeoJSON إلى kml** و **Shapefile إلى GeoJSON** وأكثر من ذلك بكثير. لأي تطبيق عرض معلومات جغرافية دون الحاجة إلى أي أدوات أو برامج إضافية، تمتلك واجهة برمجة تطبيقات GIS الخاصة بـ .NET القدرة على العمل مع عدد من الميزات الهندسية سواء كانت بسيطة أو معقدة.

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="تحويل GeoJSON إلى Shapefile SHP" %}}

بمجرد بضعة أسطر من التعليمات البرمجية، يمكن للمطورين تحويل بيانات GeoJSON إلى ملف Shapefile SHP. توفر واجهة برمجة التطبيقات [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(مسار ملف مصدر بيانات GeoJSON ،GeoJson ، مسار ملف Shapefile الوجهة، Shapefile)

{{% blocks/products/pf/feature-page-code h3="كود C#‎ للتحويل من GeoJSON إلى Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="تحويل Shapefile إلى GeoJSON" %}}

تتم عملية تحويل Shapefile إلى GeoJSON بنفس طريقة ما سبق باستخدام VectorLayer واستدعاء [طريقة Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) بالمعلمات ذات الصلة.


{{% blocks/products/pf/feature-page-code h3="كود C#‎ لتحويل بيانات Shapefile إلى GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="تحويل KML إلى GeoJSON" %}}

باستخدام طريقة VectorLayer.Convert مع المعلمات المناسبة، ملف مصدر KML ، برنامج تشغيل KML من [فئة Drivers](https://apireference.aspose.com/gis/net/aspose.gis/drivers)، مسار ملف GeoJSON وبرنامج تشغيل GeoJSON ، يمكن للمطورين بسهولة تحويل KML إلى بيانات GeoJSON.

{{% blocks/products/pf/feature-page-code h3="كود C#‎ للتحويل من KML إلى GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
