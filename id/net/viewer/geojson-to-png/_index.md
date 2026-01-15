---
title: Konversi GeoJSON ke PNG
url: /id/viewer/geojson-to-png/
linkTitle: Konversi GeoJSON ke PNG
weight: 10
description: Ubah data GeoJSON menjadi gambar PNG dengan mudah menggunakan alat online kami.
---

## Tentang

Alat ini memungkinkan Anda mengonversi file GeoJSON menjadi gambar PNG. Ini berguna untuk membuat peta statis, visualisasi data, dan berbagi data geospasial dalam format yang ramah pengguna.

## Cara Menggunakan

1.  Unggah file GeoJSON Anda atau masukkan data GeoJSON secara langsung.
2.  Tentukan opsi tampilan seperti warna, ketebalan garis, dan gaya lainnya.
3.  Klik tombol "Konversi" untuk menghasilkan gambar PNG.
4.  Unduh gambar PNG yang dihasilkan.

## Contoh

Berikut adalah contoh file GeoJSON:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [10.45, 59.93]
      },
      "properties": {
        "name": "Oslo"
      }
    },
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [11.57, 59.92]
      },
      "properties": {
        "name": "Bergen"
      }
    }
  ]
}
```

## Opsi

*   **Warna:** Warna poligon atau titik.
*   **Ketebalan Garis:** Ketebalan garis batas poligon.
*   **Radius Titik:** Radius titik data.
*   **Skala:** Skala peta.
*   **Proyeksi:** Proyeksi peta.

## Catatan

*   Ukuran file GeoJSON yang diunggah dibatasi hingga 10MB.
*   Gambar PNG yang dihasilkan memiliki resolusi maksimum 2048x2048 piksel.
*   Alat ini menggunakan pustaka Leaflet untuk merender peta.

## Dukungan

Jika Anda mengalami masalah atau memiliki pertanyaan, silakan hubungi kami di [email protected]

---
