---
title: Konversi Shapefile ke SVG
linkTitle: Konversi Shapefile ke SVG
weight: 10
url: /id/net/viewer/shapefile-to-svg/
description: Cara mengonversi file shapefile menjadi format SVG menggunakan pemirsa .NET.
---

## Konversi Shapefile ke SVG dengan Pemirsa .NET

Pemirsa .NET memungkinkan Anda untuk mengonversi file shapefile menjadi format SVG (Scalable Vector Graphics). Ini berguna untuk membuat peta vektor yang dapat diskalakan dan digunakan dalam aplikasi web atau dokumen lain.

### Prasyarat

*   Instal Visual Studio
*   Buat proyek konsol .NET baru
*   Instal paket NuGet `Net.Viewer`

```csharp
dotnet add package Net.Viewer
```

### Contoh Kode

Berikut adalah contoh kode yang menunjukkan cara mengonversi file shapefile menjadi SVG:

```csharp
using System;
using Net.Viewer;

public class ShapefileToSvgConverter
{
    public static void Main(string[] args)
    {
        // Tentukan jalur ke file shapefile input dan file SVG output
        string inputFile = "path/to/your/shapefile.shp";
        string outputFile = "path/to/your/output.svg";

        // Buat objek konverter ShapefileToSvg
        ShapefileToSvg converter = new ShapefileToSvg();

        // Konversi file shapefile ke SVG
        try
        {
            converter.Convert(inputFile, outputFile);
            Console.WriteLine("Konversi berhasil!");
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Terjadi kesalahan: {ex.Message}");
        }
    }
}
```

### Penjelasan Kode

*   `using Net.Viewer;`: Ini mengimpor namespace `Net.Viewer`, yang berisi kelas-kelas yang diperlukan untuk konversi shapefile ke SVG.
*   `string inputFile = "path/to/your/shapefile.shp";`: Ini menentukan jalur ke file shapefile input. Ganti `"path/to/your/shapefile.shp"` dengan jalur sebenarnya ke file shapefile Anda.
*   `string outputFile = "path/to/your/output.svg";`: Ini menentukan jalur ke file SVG output. Ganti `"path/to/your/output.svg"` dengan jalur yang diinginkan untuk file SVG output.
*   `ShapefileToSvg converter = new ShapefileToSvg();`: Ini membuat instance kelas `ShapefileToSvg`, yang bertanggung jawab untuk melakukan konversi.
*   `converter.Convert(inputFile, outputFile);`: Ini memanggil metode `Convert` pada objek `ShapefileToSvg` untuk mengonversi file shapefile ke SVG.
*   `try...catch`: Blok ini menangani pengecualian apa pun yang mungkin terjadi selama proses konversi.

### Opsi Tambahan

Kelas `ShapefileToSvg` menyediakan beberapa opsi tambahan yang dapat Anda gunakan untuk menyesuaikan proses konversi:

*   `Scale`: Menentukan faktor skala untuk SVG output.
*   `Simplify`: Menentukan faktor penyederhanaan untuk geometri shapefile.
*   `Encoding`: Menentukan pengkodean karakter untuk file shapefile.

Anda dapat mengatur opsi-opsi ini dengan meneruskan nilai ke konstruktor kelas `ShapefileToSvg`.

### Kesimpulan

Dengan menggunakan Pemirsa .NET, Anda dapat dengan mudah mengonversi file shapefile menjadi format SVG. Ini memungkinkan Anda membuat peta vektor yang dapat diskalakan dan digunakan dalam berbagai aplikasi.
---
