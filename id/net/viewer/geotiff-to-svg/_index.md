---
title: Konversi GeoTIFF ke SVG
linkTitle: Konversi GeoTIFF ke SVG
weight: 10
url: /id/net/viewer/geotiff-to-svg/
description: Cara mengonversi file GeoTIFF ke format SVG menggunakan pemirsa .NET.
---

## Pengantar

Pemirsa .NET memungkinkan Anda untuk mengonversi file GeoTIFF ke format SVG. Ini berguna untuk membuat gambar vektor dari data raster geospasial.

## Persyaratan

*   Pemirsa .NET terinstal
*   File GeoTIFF yang valid

## Langkah-langkah

1.  Buka Pemirsa .NET.
2.  Muat file GeoTIFF yang ingin Anda konversi.
3.  Pilih "Konversi" dari menu.
4.  Pilih "SVG" sebagai format output.
5.  Tentukan nama file dan lokasi untuk file SVG yang dihasilkan.
6.  Klik tombol "Konversi".

## Contoh Kode

```csharp
// Contoh kode untuk mengonversi GeoTIFF ke SVG
using NetViewer;
using System;
using System.IO;

public class GeotiffToSvgConverter
{
    public static void Main(string[] args)
    {
        // Tentukan jalur file input dan output
        string inputFile = "path/to/your/geotiff/file.tif";
        string outputFile = "path/to/your/output/svg/file.svg";

        // Muat file GeoTIFF
        GeoTiff raster = new GeoTiff(inputFile);

        // Konversi ke SVG
        raster.ConvertToSvg(outputFile);

        Console.WriteLine("Konversi selesai!");
    }
}
```

## Opsi Tambahan

*   Anda dapat menyesuaikan proses konversi dengan menentukan opsi tambahan, seperti resolusi dan skala.
*   Pemirsa .NET mendukung berbagai format file input dan output.

## Pemecahan Masalah

*   Jika Anda mengalami masalah saat mengonversi file GeoTIFF ke SVG, pastikan bahwa file tersebut valid dan tidak rusak.
*   Pastikan juga bahwa Anda memiliki izin yang diperlukan untuk menulis ke lokasi output.
*   Jika masalah berlanjut, hubungi dukungan teknis untuk mendapatkan bantuan lebih lanjut.
---
