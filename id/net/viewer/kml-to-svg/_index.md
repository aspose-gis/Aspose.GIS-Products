---
title: KML ke SVG
linkTitle: KML ke SVG
weight: 10
url: /id/net/viewer/kml-to-svg/
description: Konversi berkas KML ke format SVG.
---

## KML ke SVG

Konversikan berkas KML Anda menjadi gambar vektor SVG yang dapat diskalakan menggunakan alat online gratis kami.

### Cara Menggunakan

1.  Unggah berkas KML Anda.
2.  Tentukan opsi konversi, seperti skala dan warna.
3.  Klik tombol "Konversi".
4.  Unduh berkas SVG yang dihasilkan.

### Opsi Konversi

*   **Skala:** Sesuaikan ukuran gambar SVG yang dihasilkan.
*   **Warna:** Ubah warna fitur dalam gambar SVG.
*   **Latar Belakang:** Tambahkan latar belakang ke gambar SVG.
*   **Simbol:** Gunakan simbol untuk mewakili fitur dalam gambar SVG.

### Contoh

Berikut adalah contoh berkas KML sebelum dan sesudah konversi:

**Berkas KML (sebelum):**

```xml
<kml xmlns="http://www.opengis.net/kml/2.2">
  <Placemark>
    <name>Lokasi 1</name>
    <description>Ini adalah lokasi pertama.</description>
    <Point>
      <coordinates>-73.985704,40.748439</coordinates>
    </Point>
  </Placemark>
  <Placemark>
    <name>Lokasi 2</name>
    <description>Ini adalah lokasi kedua.</description>
    <Point>
      <coordinates>-74.006032,40.712728</coordinates>
    </Point>
  </Placemark>
</kml>
```

**Berkas SVG (sesudah):**

```xml
<svg width="500" height="500">
  <circle cx="-73.985704" cy="40.748439" r="10" fill="red" />
  <circle cx="-74.006032" cy="40.712728" r="10" fill="blue" />
</svg>
```

### Catatan

*   Alat ini mendukung berkas KML hingga ukuran tertentu.
*   Berkas SVG yang dihasilkan mungkin tidak sepenuhnya akurat karena pembulatan dan kesalahan lainnya.
*   Jika Anda memiliki pertanyaan atau masalah, silakan hubungi kami.
---
