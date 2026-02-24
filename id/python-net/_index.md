---
title: Python .NET
url: /id/python-net/
weight: 10
layout: single
start: true
split: before

hero:
  image: ""
  content: "Pelajari cara menggunakan Python dengan .NET."
  buttons:
    - text: "Mulai"
      link: "/id/python-net/getting-started/"

---

## Apa itu Python .NET?
Ini adalah cara untuk menjalankan kode Python di lingkungan .NET. Ini memungkinkan Anda memanfaatkan ekosistem luas pustaka dan alat .NET sambil tetap menggunakan fleksibilitas dan kemudahan penggunaan Python.

## Manfaat Menggunakan Python .NET
*   **Integrasi:** Gabungkan kode Python dengan aplikasi C# atau VB.NET yang ada.
*   **Kinerja:** Dapatkan kinerja yang baik untuk tugas-tugas intensif komputasi.
*   **Fleksibilitas:** Gunakan pustaka Python dan alat tanpa meninggalkan lingkungan .NET.
*   **Produktivitas:** Tingkatkan produktivitas dengan menggunakan bahasa yang Anda kenal.

## Kasus Penggunaan Umum
Python .NET dapat digunakan untuk berbagai kasus penggunaan, termasuk:
*   **Analisis Data:** Gunakan pustaka Python seperti Pandas dan NumPy untuk analisis data.
*   **Pembelajaran Mesin:** Bangun model pembelajaran mesin menggunakan pustaka Python seperti Scikit-learn dan TensorFlow.
*   **Otomatisasi:** Otomatiskan tugas dengan skrip Python.
*   **Pengembangan Web:** Kembangkan aplikasi web dengan kerangka kerja Python seperti Django dan Flask.

## Memulai
Untuk memulai dengan Python .NET, Anda perlu menginstal:
*   **.NET SDK:** Unduh versi terbaru dari situs web Microsoft.
*   **IronPython:** Instal paket IronPython melalui NuGet.

Setelah Anda menginstal prasyaratnya, Anda dapat mulai menulis kode Python di lingkungan .NET.

## Contoh
Berikut adalah contoh sederhana cara menjalankan kode Python di aplikasi C#:

```csharp
// This is a comment in C#
using Microsoft.Scripting.Hosting;

public class Example
{
    public static void Main(string[] args)
    {
        ScriptEngine engine = IronPython.Hosting.IronPython.CreateEngine();
        // This is a comment in Python
        string script = "print('Hello, world!')";
        ScriptScope scope = engine.CreateScope();
        engine.Execute(script, scope);
    }
}
```

Contoh ini membuat mesin skrip IronPython dan menjalankan kode Python sederhana yang mencetak "Halo, dunia!" ke konsol.

## Sumber Daya Tambahan
*   [Microsoft .NET](https://dotnet.microsoft.com/en-us/)
*   [IronPython](https://ironpython.net/)
*   [NuGet](https://www.nuget.org/)

---
