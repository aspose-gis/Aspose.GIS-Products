---
title: Shapefile to SVG Conversion
linkTitle: การแปลง Shapefile เป็น SVG
weight: 10
url: /th/net/viewer/shapefile-to-svg/
description: Learn how to convert shapefiles to scalable vector graphics (SVG) format using .NET.
source: "https://github.com/Geometria/ShapefileToSvg"
---

## Introduction
## การนำเสนอ

This guide explains how to convert Shapefiles to SVG files using a .NET application.  
คำแนะนำนี้อธิบายวิธีการแปลงไฟล์ Shapefile เป็นไฟล์ SVG โดยใช้แอปพลิเคชัน .NET

## Prerequisites
## ข้อกำหนดเบื้องต้น

*   .NET SDK
*   Shapefile library for .NET (e.g., SharpMap, GeoSharp)
*   SVG generation library for .NET (e.g., SVGDotNet)
*   A Shapefile to convert
*   SDK .NET
*   ไลบรารี Shapefile สำหรับ .NET (เช่น SharpMap, GeoSharp)
*   ไลบรารีสร้าง SVG สำหรับ .NET (เช่น SVGDotNet)
*   ไฟล์ Shapefile ที่จะแปลง

## Steps
## ขั้นตอน

1.  **Install necessary libraries:**  
    ติดตั้งไลบรารีที่จำเป็น:

    ```bash
    dotnet add package SharpMap
    dotnet add package SVGDotNet
    ```

2.  **Create a new .NET project:**  
    สร้างโปรเจ็กต์ .NET ใหม่:

3.  **Write the code to read the Shapefile and convert it to SVG:**  
    เขียนโค้ดเพื่ออ่านไฟล์ Shapefile และแปลงเป็น SVG:

    ```csharp
    using SharpMap;
    using SharpMap.Layers;
    using SharpMap.Rendering;
    using SVGDotNet;
    using System.Drawing;
    using System.IO;

    public class ShapefileToSvgConverter
    {
        public static void ConvertShapefileToSvg(string shapefilePath, string svgFilePath)
        {
            // Load the Shapefile
            var stream = new FileStream(shapefilePath, FileMode.Open);
            var shapefileLayer = LayerFactory.CreateShapefileLayer(stream, "shp");

            // Create an SVG document
            SvgDocument svgDoc = new SvgDocument();

            // Render the layer to the SVG document
            using (Graphics g = Graphics.FromImage(svgDoc.RootVisual))
            {
                shapefileLayer.Render(g, new SimpleRenderingConfiguration());
            }

            // Save the SVG document to a file
            svgDoc.Save(svgFilePath);
        }
    }
    ```

4.  **Run the application:**  
    เรียกใช้แอปพลิเคชัน:

## Explanation
## คำอธิบาย

The code reads the Shapefile using SharpMap, creates an SVG document using SVGDotNet, renders the layer to the SVG document, and saves the SVG document to a file.  
โค้ดอ่านไฟล์ Shapefile โดยใช้ SharpMap สร้างเอกสาร SVG โดยใช้ SVGDotNet แสดงผลเลเยอร์ลงในเอกสาร SVG และบันทึกเอกสาร SVG ลงในไฟล์

## Troubleshooting
## การแก้ไขปัญหา

*   **Shapefile not found:**  Make sure the path to the Shapefile is correct.  
    ไฟล์ Shapefile ไม่พบ ตรวจสอบให้แน่ใจว่าพาธไปยังไฟล์ Shapefile ถูกต้อง
*   **Error loading Shapefile:**  The Shapefile may be corrupted or in an unsupported format.  
    ข้อผิดพลาดในการโหลดไฟล์ Shapefile ไฟล์ Shapefile อาจเสียหายหรือไม่รองรับรูปแบบ
*   **SVG generation error:**  There may be a problem with the SVG generation library.  
    ข้อผิดพลาดในการสร้าง SVG อาจมีปัญหากับไลบรารีการสร้าง SVG

## Conclusion
## สรุป

This guide provides a basic example of how to convert Shapefiles to SVG files using .NET. You can customize this code further to meet your specific needs.  
คำแนะนำนี้ให้ตัวอย่างพื้นฐานเกี่ยวกับวิธีการแปลงไฟล์ Shapefile เป็นไฟล์ SVG โดยใช้ .NET คุณสามารถปรับแต่งโค้ดนี้เพิ่มเติมเพื่อให้ตรงกับความต้องการเฉพาะของคุณ
