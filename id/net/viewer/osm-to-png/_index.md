---
title: Konversi OSM ke PNG
url: /id/viewer/osm-to-png/
weight: 10
layout: single
draft: false
toc: true
---

## Deskripsi

Alat ini mengonversi data OpenStreetMap (OSM) menjadi gambar PNG. Anda dapat menentukan area yang akan diekspor, gaya tampilan, dan opsi lainnya untuk menghasilkan peta khusus sesuai kebutuhan Anda.

## Persyaratan

*   [NetViewer](https://netviewer.org/) terinstal
*   Data OSM dalam format `.osm` atau `.pbf`

## Penggunaan

1.  **Buka NetViewer.**
2.  **Muat data OSM:** Pilih file `.osm` atau `.pbf` yang ingin Anda konversi.
3.  **Tentukan area ekspor:** Tentukan kotak pembatas (bounding box) area peta yang akan diekspor.
4.  **Konfigurasi gaya tampilan:** Sesuaikan lapisan, warna, dan simbol untuk mewakili berbagai fitur OSM.
5.  **Atur opsi ekspor:** Pilih resolusi, format file (PNG), dan opsi lainnya.
6.  **Hasilkan gambar PNG:** Klik tombol "Eksport" atau yang serupa untuk menghasilkan gambar PNG dari data OSM yang telah dikonfigurasi.

## Opsi Konfigurasi

*   **File Data OSM:** Lokasi file `.osm` atau `.pbf`.
*   **Kotak Pembatas (Bounding Box):** Koordinat sudut kiri atas dan kanan bawah area peta yang akan diekspor.
*   **Resolusi:** Lebar dan tinggi gambar PNG dalam piksel. Resolusi lebih tinggi menghasilkan gambar dengan detail lebih baik, tetapi juga ukuran file yang lebih besar.
*   **Gaya Tampilan (Rendering Styles):** Aturan untuk mewakili berbagai fitur OSM, seperti jalan, bangunan, dan sungai. Anda dapat menyesuaikan warna, ketebalan garis, simbol, dan label untuk setiap fitur.
*   **Format File:** Format gambar yang akan dihasilkan (dalam kasus ini, PNG).
*   **Opsi Tambahan:** Opsi lain seperti transparansi latar belakang, skala peta, dan orientasi utara.

## Contoh

Untuk mengonversi area di sekitar Jakarta dengan resolusi 512x512 piksel:

1.  Muat file data OSM untuk Indonesia.
2.  Atur kotak pembatas ke koordinat yang mencakup Jakarta (misalnya, -6.9083° S, 106.8456° E hingga -6.2357° S, 107.0775° E).
3.  Sesuaikan gaya tampilan untuk menampilkan jalan dan bangunan dengan jelas.
4.  Atur resolusi ke 512x512 piksel.
5.  Hasilkan gambar PNG.

## Catatan

*   Ukuran file data OSM dapat sangat besar. Pastikan Anda memiliki cukup memori dan ruang disk sebelum memulai konversi.
*   Gaya tampilan yang kompleks dapat memperlambat proses rendering. Sederhanakan gaya jika perlu untuk meningkatkan kinerja.
*   Eksperimen dengan berbagai opsi konfigurasi untuk mendapatkan hasil terbaik sesuai kebutuhan Anda.

---
