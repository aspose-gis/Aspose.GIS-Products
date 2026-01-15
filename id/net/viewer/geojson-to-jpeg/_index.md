---
title: GeoJSON ke JPEG
linkTitle: GeoJSON ke JPEG
weight: 10
description: Konversi file GeoJSON menjadi gambar JPEG.
url: /id/viewer/geojson-to-jpeg/
aliases: [geojson2jpeg, geojson to jpeg]
---

## Tentang

Konverter GeoJSON ke JPEG memungkinkan Anda mengubah data GeoJSON menjadi gambar JPEG. Ini berguna untuk memvisualisasikan data geospasial dalam format yang mudah dibagikan dan dipahami.

## Cara Menggunakan

1.  Unggah file GeoJSON Anda.
2.  Tentukan parameter konversi, seperti skala, warna, dan resolusi.
3.  Klik tombol "Konversi".
4.  Unduh gambar JPEG yang dihasilkan.

## Parameter

*   **Skala:** Menentukan skala data geospasial.
*   **Warna:** Menentukan warna fitur dalam gambar.
*   **Resolusi:** Menentukan resolusi gambar.
*   **Format:** Pilih format output, dalam kasus ini JPEG.

## Contoh

Berikut adalah contoh penggunaan konverter GeoJSON ke JPEG:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Point",
        "coordinates": [10.45, 52.52]
      },
      "properties": {
        "name": "Berlin"
      }
    }
  ]
}
```

Dengan skala 1:1000, warna biru, dan resolusi 300 DPI, konverter akan menghasilkan gambar JPEG yang menunjukkan lokasi Berlin.

## Catatan

*   Pastikan file GeoJSON Anda valid.
*   Parameter konversi memengaruhi tampilan gambar yang dihasilkan.
*   Gambar JPEG yang dihasilkan dapat diunduh dalam berbagai resolusi.
*   Konverter ini mendukung format output lainnya, seperti PNG dan SVG.
---
