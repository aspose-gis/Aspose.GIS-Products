
---
title: การแปลงข้อมูล GIS ด้วย C#
url: /th/net/conversion/
description: แปลงข้อมูล GIS ในรูปแบบต่างๆ รวมถึง GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM ด้วยโค้ด C# เพียงไม่กี่บรรทัดผ่านไลบรารี .NET
---

{{< blocks/products/pf/feature-page-wrap >}}
{{< blocks/products/pf/feature-page-header h1="การแปลงข้อมูล GIS ด้วย C#" h2="แปลง GeoJSON, ESRI Shapefile SHX, TopoJSON, FIleGDB, GML, KML, MIF, OSM เป็นข้อมูลเพื่อสร้างแอปพลิเคชัน .NET ข้ามแพลตฟอร์ม" >}}

{{% blocks/products/pf/feature-page-summary %}}


ในการวิเคราะห์ข้อมูลเชิงพื้นที่และภูมิศาสตร์ API GIS ของ .NET ช่วยอำนวยความสะดวกในการสร้างโซลูชันเพื่อจับเก็บ จัดการ ปรับเปลี่ยน วิเคราะห์ และนำเสนอข้อมูลทางภูมิศาสตร์ทุกประเภท ไม่เพียงแต่โหลดรูปแบบเวกเตอร์และแรสเตอร์ที่แตกต่างกันเท่านั้น แต่ยังแปลงเป็นรูปแบบอื่นได้อย่างง่ายดายอีกด้วย สถานการณ์การเรนเดอร์บางส่วน เช่น **GeoJSON เป็น Shapefile** , **GeoJSON เป็น topojson**, **GeoJSON เป็น kml**, **Shapefile เป็น GeoJSON** และอื่นๆ สำหรับแอปพลิเคชันการเรนเดอร์ข้อมูลทางภูมิศาสตร์ใดๆ โดยไม่ต้องใช้เครื่องมือหรือซอฟต์แวร์เพิ่มเติม API GIS ของ .NET มีความสามารถในการทำงานกับคุณสมบัติทางเรขาคณิตจำนวนมาก ไม่ว่าจะเรียบง่ายหรือซับซ้อน

{{% /blocks/products/pf/feature-page-summary  %}}

{{% blocks/products/pf/feature-page-section  h2="การแปลง GeoJSON เป็น Shapefile SHP" %}}

ด้วยโค้ดเพียงไม่กี่บรรทัด นักพัฒนาสามารถแปลงข้อมูล GeoJSON เป็นไฟล์ Shapefile SHP ได้ API จัดเตรียม [VectorLayer](https://apireference.aspose.com/gis/net/aspose.gis/vectorlayer).Convert(source GeoJSON data file Path, GeoJson, destination Shapefile Path, Shapefile)

{{% blocks/products/pf/feature-page-code h3="โค้ด C# สำหรับการแปลง GeoJSON เป็น Shapefile" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-geojson-to-shapefile.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="geojson-to-json geojson-to-kml geojson-to-shx geojson-to-topojson" >}}

{{% blocks/products/pf/feature-page-section  h2="แปลง Shapefile เป็น GeoJSON" %}}

กระบวนการแปลง Shapefile เป็น GeoJSON เหมือนกับข้างต้นโดยใช้ VectorLayer และเรียกใช้เมธอด [Convert](https://apireference.aspose.com/gis/net/aspose.gis.vectorlayer/convert/methods/2) ด้วยพารามิเตอร์ที่เกี่ยวข้อง

{{% blocks/products/pf/feature-page-code h3="โค้ด C# สำหรับการแปลงข้อมูล Shapefile เป็น GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-shapefile-data-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="shx-to-geojson shx-to-json shx-to-kml" >}}

{{% blocks/products/pf/feature-page-section  h2="แปลง KML เป็น GeoJSON" %}}

ด้วยการใช้เมธอด VectorLayer.Convert พร้อมพารามิเตอร์ที่เหมาะสม ไฟล์แหล่ง KML, ไดรเวอร์ KML จาก [Drivers class](https://apireference.aspose.com/gis/net/aspose.gis/drivers), เส้นทางไฟล์ GeoJSON และไดรเวอร์ GeoJSON นักพัฒนาสามารถแปลง KML เป็นข้อมูล GeoJSON ได้อย่างง่ายดาย

{{% blocks/products/pf/feature-page-code h3="โค้ด C# สำหรับการแปลง KML เป็น GeoJSON" %}}

{{< gist "aspose-com-gists" "e73b120af8fce9c18feb963d5f3a16a2" "convert-kml-to-geojson.cs" >}}

{{% /blocks/products/pf/feature-page-code  %}}

{{% /blocks/products/pf/feature-page-section %}}
{{< blocks/products/pf/feature-page-options pairs="kml-to-json kml-to-shx kml-to-geojson" >}}

{{< /blocks/products/pf/feature-page-wrap >}}
