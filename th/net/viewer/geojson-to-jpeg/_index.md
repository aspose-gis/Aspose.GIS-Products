---
title: GeoJSON to JPEG Conversion
linkTitle: การแปลง GeoJSON เป็น JPEG
weight: 10
url: /th/net/viewer/geojson-to-jpeg/
description: Learn how to convert GeoJSON data into JPEG images using .NET.
aliases: [geojson2jpeg, geojson to jpeg]
---

## Overview
## ภาพรวม

This guide explains how to convert GeoJSON data into JPEG images using .NET.  This process is useful for visualizing geospatial data and creating custom maps.
คำแนะนำนี้อธิบายวิธีการแปลงข้อมูล GeoJSON เป็นรูปภาพ JPEG โดยใช้ .NET กระบวนการนี้มีประโยชน์สำหรับการแสดงภาพข้อมูลภูมิสารสนเทศและการสร้างแผนที่แบบกำหนดเอง

## Prerequisites
## ข้อกำหนดเบื้องต้น

*   .NET SDK installed
*   A GeoJSON file to convert
*   Basic understanding of C# and .NET
*   ติดตั้ง .NET SDK แล้ว
*   ไฟล์ GeoJSON ที่จะแปลง
*   ความเข้าใจพื้นฐานเกี่ยวกับ C# และ .NET

## Steps
## ขั้นตอน

1.  **Create a new .NET project:** สร้างโปรเจ็กต์ .NET ใหม่
2.  **Install necessary packages:** ติดตั้งแพ็คเกจที่จำเป็น
3.  **Write the code:** เขียนโค้ด
4.  **Run the application:** รันแอปพลิเคชัน

## 1. Create a new .NET project
## 1. สร้างโปรเจ็กต์ .NET ใหม่

Create a new console application using the .NET CLI:
สร้างแอปพลิเคชันคอนโซลใหม่โดยใช้ .NET CLI:

```bash
dotnet new console -o GeoJsonToJpegConverter
cd GeoJsonToJpegConverter
```

## 2. Install necessary packages
## 2. ติดตั้งแพ็คเกจที่จำเป็น

You'll need the following NuGet packages:
คุณจะต้องมีแพ็กเกจ NuGet เหล่านี้:

*   `Newtonsoft.Json`: For parsing GeoJSON data. สำหรับการแยกวิเคราะห์ข้อมูล GeoJSON
*   `ImageSharp`: For image manipulation. สำหรับการจัดการรูปภาพ

Install them using the .NET CLI:
ติดตั้งโดยใช้ .NET CLI:

```bash
dotnet add package Newtonsoft.Json
dotnet add package ImageSharp
```

## 3. Write the code
## 3. เขียนโค้ด

Replace the contents of `Program.cs` with the following code:
แทนที่เนื้อหาของ `Program.cs` ด้วยโค้ดต่อไปนี้:

```csharp
using Newtonsoft.Json;
using SixLabors.ImageSharp;
using SixLabors.ImageSharp.Drawing;
using SixLabors.ImageSharp.PixelFormats;
using System;
using System.Collections.Generic;
using System.IO;

public class GeoJsonToJpegConverter
{
    public static void Main(string[] args)
    {
        // Replace with your GeoJSON file path
        // แทนที่ด้วยพาธไฟล์ GeoJSON ของคุณ
        string geoJsonFilePath = "path/to/your/file.geojson";

        // Replace with the desired output JPEG file path
        // แทนที่ด้วยพาธไฟล์ JPEG ที่ต้องการสำหรับผลลัพธ์
        string jpegOutputFilePath = "output.jpeg";

        try
        {
            var geoJsonData = File.ReadAllText(geojsonFilePath);
            var features = JsonConvert.DeserializeObject<List<Feature>>(geoJsonData);

            // Example: Create a simple image with one feature
            // ตัวอย่าง: สร้างรูปภาพง่ายๆ ด้วยฟีเจอร์หนึ่งรายการ
            if (features != null && features.Count > 0)
            {
                var feature = features[0]; // Get the first feature

                // Assuming the feature has coordinates
                // สมมติว่าฟีเจอร์มีพิกัด
                if (feature.Geometry is { Type: "Point", Coordinates: var coordinates } pointFeature)
                {
                    double x = pointFeature.Coordinates[0]; // Longitude
                    double y = pointFeature.Coordinates[1]; // Latitude

                    // Define image size and scale
                    // กำหนดขนาดรูปภาพและสเกล
                    int width = 200;
                    int height = 200;
                    float scale = 100000; // Adjust as needed

                    // Create a new ImageSharp image
                    using (Image<Rgba32> image = new Image<Rgba32>(width, height))
                    {
                        // Draw the point on the image
                        image.Draw(Pens.Black, PointF.Create(x / scale + width / 2f, y / scale + height / 2f));

                        // Save the image to a JPEG file
                        image.SaveAsJpeg(jpegOutputFilePath);
                    }

                    Console.WriteLine($"Successfully converted GeoJSON to JPEG: {jpegOutputFilePath}");
                }
                else
                {
                    Console.WriteLine("Feature does not have Point geometry.");
                }
            }
            else
            {
                Console.WriteLine("No features found in the GeoJSON file.");
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine($"An error occurred: {ex.Message}");
        }
    }

    public class Feature
    {
        public string Type { get; set; }
        public object Geometry { get; set; }
    }
}
```

**Explanation:**
**คำอธิบาย:**

*   The code reads a GeoJSON file and parses it using `Newtonsoft.Json`.
*   It then takes the first feature from the parsed data.
*   If the feature is a point, it calculates its coordinates and draws a black dot on an ImageSharp image.
*   Finally, it saves the image as a JPEG file.
*   โค้ดอ่านไฟล์ GeoJSON และแยกวิเคราะห์โดยใช้ `Newtonsoft.Json`
*   จากนั้นจะนำฟีเจอร์แรกจากข้อมูลที่แยกวิเคราะห์มา
*   หากฟีเจอร์เป็นจุด จะคำนวณพิกัดและวาดจุดสีดำบนรูปภาพ ImageSharp
*   สุดท้าย จะบันทึกรูปภาพเป็นไฟล์ JPEG

## 4. Run the application
## 4. รันแอปพลิเคชัน

Run the application using the .NET CLI:
รันแอปพลิเคชันโดยใช้ .NET CLI:

```bash
dotnet run
```

This will convert the GeoJSON file to a JPEG image and save it as `output.jpeg` in the project directory.
สิ่งนี้จะแปลงไฟล์ GeoJSON เป็นรูปภาพ JPEG และบันทึกเป็น `output.jpeg` ในไดเรกทอรีโปรเจ็กต์

## Considerations
## ข้อควรพิจารณา

*   **Coordinate System:** Ensure that your GeoJSON data uses a coordinate system that is appropriate for the scale of your image.  You may need to perform transformations if necessary.
*   **Image Size and Scale:** Adjust the `width`, `height`, and `scale` variables in the code to control the size and resolution of the output JPEG image.
*   **Error Handling:** The provided code includes basic error handling, but you should add more robust error checking for production use.
*   **Geometry Types:** This example only handles point geometries.  You'll need to modify the code to handle other geometry types (e.g., lines, polygons).
*   **ระบบพิกัด:** ตรวจสอบให้แน่ใจว่าข้อมูล GeoJSON ของคุณใช้ระบบพิกัดที่เหมาะสมกับสเกลของรูปภาพของคุณ คุณอาจต้องทำการแปลงหากจำเป็น
*   **ขนาดและสเกลของรูปภาพ:** ปรับเปลี่ยนตัวแปร `width`, `height` และ `scale` ในโค้ดเพื่อควบคุมขนาดและความละเอียดของรูปภาพ JPEG ที่ได้
*   **การจัดการข้อผิดพลาด:** โค้ดที่ให้มามีระบบจัดการข้อผิดพลาดขั้นพื้นฐาน แต่คุณควรเพิ่มการตรวจสอบข้อผิดพลาดที่ครอบคลุมมากขึ้นสำหรับการใช้งานจริง
*   **ชนิดเรขาคณิต:** ตัวอย่างนี้จัดการเฉพาะเรขาคณิตแบบจุดเท่านั้น คุณจะต้องแก้ไขโค้ดเพื่อรองรับชนิดเรขาคณิตอื่นๆ (เช่น เส้น, พหุเหลี่ยม)

---
