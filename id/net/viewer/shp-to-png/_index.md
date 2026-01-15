---
title: Konversi SHP ke PNG
url: /id/viewer/shp-to-png/
weight: 10
layout: single
start: true
toc: true
draft: false
description: Cara mengonversi file SHP menjadi gambar PNG menggunakan pemirsa GIS.
---

## Konversi SHP ke PNG

Pemirsa GIS memungkinkan Anda untuk mengonversi file shapefile (SHP) menjadi gambar Portable Network Graphics (PNG). Ini berguna untuk membuat peta atau visualisasi yang dapat dengan mudah dibagikan dan dimasukkan ke dalam dokumen lain.

### Langkah-langkah

1.  Buka Pemirsa GIS.
2.  Muat file SHP yang ingin Anda konversi.
3.  Tentukan area yang ingin Anda tangkap sebagai gambar PNG.
4.  Atur opsi ekspor, seperti resolusi dan format warna.
5.  Simpan gambar PNG ke lokasi yang diinginkan.

### Opsi Ekspor

Saat mengekspor file SHP menjadi gambar PNG, Anda dapat menyesuaikan beberapa opsi:

*   **Resolusi:** Resolusi gambar PNG dalam titik per inci (DPI). Semakin tinggi resolusinya, semakin detail gambarnya, tetapi ukurannya juga akan lebih besar.
*   **Format Warna:** Format warna gambar PNG. Pilihan termasuk RGB, CMYK, dan skala abu-abu.
*   **Transparansi:** Apakah akan menyertakan transparansi dalam gambar PNG. Jika diaktifkan, area transparan pada shapefile akan ditampilkan sebagai transparan dalam gambar PNG.

### Contoh

Untuk mengonversi file SHP bernama "states.shp" menjadi gambar PNG dengan resolusi 300 DPI dan format warna RGB, Anda dapat menggunakan perintah berikut:

```
gisserver -o png -r 300 -c rgb states.shp
```

Perintah ini akan membuat gambar PNG bernama "states.png" di direktori yang sama dengan file SHP.

### Catatan

*   Pastikan Anda memiliki Pemirsa GIS terinstal dan dikonfigurasi dengan benar sebelum mencoba mengonversi file SHP menjadi gambar PNG.
*   Ukuran gambar PNG yang dihasilkan akan bergantung pada resolusi, format warna, dan ukuran shapefile.
*   Anda dapat menyesuaikan opsi ekspor untuk mencapai hasil yang diinginkan.

---
