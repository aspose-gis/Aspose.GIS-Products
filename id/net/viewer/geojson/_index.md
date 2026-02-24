---
title: GeoJSON Viewer
linkTitle: Penampil GeoJSON
weight: 10
url: /id/viewer/geojson/
aliases: [geojson viewer, geojson display]
description: Tampilan interaktif untuk data GeoJSON.
---

## Tentang

Penampil GeoJSON adalah alat yang memungkinkan Anda melihat dan berinteraksi dengan data GeoJSON secara langsung di browser web Anda. Ini menyediakan cara visual untuk menjelajahi fitur-fitur geografis yang disimpan dalam format GeoJSON.

## Fitur Utama

*   **Tampilan Interaktif:** Zoom, pan, dan hover pada fitur untuk mendapatkan informasi lebih lanjut.
*   **Styling:** Sesuaikan tampilan fitur menggunakan berbagai gaya seperti warna, ketebalan garis, dan ikon.
*   **Informasi Fitur:** Tampilkan atribut terkait dengan setiap fitur saat Anda mengarahkan kursor di atasnya.
*   **Filter:** Filter fitur berdasarkan atribut untuk fokus pada subset data tertentu.
*   **Dukungan Berbagai Format:** Muat GeoJSON dari file lokal, URL, atau string JSON.

## Penggunaan

1.  **Muat Data GeoJSON:** Anda dapat memuat data GeoJSON dengan beberapa cara:
    *   **Dari File Lokal:** Pilih file GeoJSON dari komputer Anda menggunakan tombol "Pilih File".
    *   **Dari URL:** Masukkan URL langsung ke file GeoJSON di bidang yang disediakan.
    *   **Dari String JSON:** Tempel string JSON GeoJSON secara langsung ke dalam editor teks.

2.  **Jelajahi Data:** Setelah data dimuat, Anda dapat menggunakan kontrol peta untuk memperbesar, mengecil, dan menggeser tampilan. Arahkan kursor di atas fitur untuk melihat atribut terkaitnya.

3.  **Sesuaikan Tampilan (Opsional):** Gunakan opsi styling untuk mengubah warna, ketebalan garis, dan ikon fitur. Ini memungkinkan Anda untuk menyorot fitur tertentu atau membuat peta lebih mudah dibaca.

## Contoh Data GeoJSON

Berikut adalah contoh data GeoJSON yang dapat Anda gunakan untuk menguji penampil:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [-73.9857, 40.7484]
      },
      "properties": {
        "name": "New York City",
        "population": 8419000
      }
    },
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [-74.0060, 40.7128]
      },
      "properties": {
        "name": "Brooklyn",
        "population": 2586000
      }
    }
  ]
}
```

## Catatan Tambahan

*   Penampil GeoJSON menggunakan pustaka peta sumber terbuka seperti Leaflet atau Mapbox GL JS untuk rendering peta.
*   Pastikan data GeoJSON Anda valid sebelum memuatnya ke dalam penampil. Anda dapat menggunakan validator GeoJSON online untuk memeriksa validitas data Anda.
*   Jika Anda mengalami masalah, periksa konsol browser Anda untuk pesan kesalahan.

---
