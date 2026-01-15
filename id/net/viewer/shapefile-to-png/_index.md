---
title: Konversi Shapefile ke PNG
url: /id/net/viewer/shapefile-to-png/
linkTitle: Konversi Shapefile ke PNG
weight: 10
description: Cara mengonversi file shapefile menjadi gambar PNG menggunakan pembaca shapefile .NET.
---

## Konversi Shapefile ke PNG dengan Pembaca Shapefile .NET

Pembaca Shapefile .NET memungkinkan Anda untuk mengonversi file shapefile menjadi gambar PNG. Ini berguna untuk membuat peta atau visualisasi lainnya yang perlu disimpan dalam format gambar.

### Prasyarat

*   Instal Visual Studio
*   Buat proyek konsol .NET baru
*   Instal paket NuGet `Net.Kgis`

```csharp
dotnet add package Net.Kgis
```

### Contoh Kode

Berikut adalah contoh kode yang menunjukkan cara mengonversi file shapefile menjadi gambar PNG:

```csharp
using System;
using System.Drawing;
using System.IO;
using Net.Kgis;

public class ShapefileToolToPngConverter
{
    public static void Main(string[] args)
    {
        // Tentukan jalur ke file shapefile input dan gambar PNG output
        string inputFile = "path/to/your/shapefile.shp";
        string outputFile = "path/to/your/output.png";

        // Buat objek ShapefileReader baru
        ShapefileReader reader = new ShapefileReader(inputFile);

        // Baca file shapefile
        reader.Read();

        // Dapatkan jumlah fitur dalam file shapefile
        int featureCount = reader.FeatureCount;

        Console.WriteLine($"Jumlah fitur: {featureCount}");

        // Buat objek Bitmap baru
        Bitmap bitmap = new Bitmap(256, 256);

        // Buat objek Graphics baru
        Graphics graphics = Graphics.FromImage(bitmap);

        // Gambar setiap fitur ke bitmap
        foreach (ShapefileFeature feature in reader.Features)
        {
            // Dapatkan geometri fitur
            Geometry geometry = feature.Geometry;

            // Gambar geometri ke bitmap
            graphics.DrawGeometry(Pens.Black, geometry);
        }

        // Simpan bitmap ke file PNG
        bitmap.Save(outputFile, System.Drawing.Imaging.ImageFormat.Png);

        Console.WriteLine($"Gambar disimpan ke {outputFile}");
    }
}
```

### Penjelasan Kode

*   Baris pertama mengimpor namespace yang diperlukan.
*   Baris kedua menentukan jalur ke file shapefile input dan gambar PNG output.
*   Baris ketiga membuat objek `ShapefileReader` baru.
*   Baris keempat membaca file shapefile.
*   Baris kelima mendapatkan jumlah fitur dalam file shapefile.
*   Baris keenam membuat objek `Bitmap` baru.
*   Baris ketujuh membuat objek `Graphics` baru.
*   Baris kedelapan menggambar setiap fitur ke bitmap.
*   Baris kesembilan menyimpan bitmap ke file PNG.

### Kesimpulan

Ini adalah contoh sederhana tentang cara mengonversi file shapefile menjadi gambar PNG menggunakan pembaca shapefile .NET. Anda dapat memodifikasi kode ini untuk memenuhi kebutuhan spesifik Anda. Misalnya, Anda dapat mengubah ukuran gambar, menambahkan legenda, atau menggambar fitur dengan warna yang berbeda.
---
