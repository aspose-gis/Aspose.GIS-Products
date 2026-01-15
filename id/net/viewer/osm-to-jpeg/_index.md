---
title: Konversi OSM ke JPEG
url: /id/viewer/osm-to-jpeg/
weight: 10
layout: single
draft: false
toc: true
---

## Deskripsi

Alat ini mengonversi data OpenStreetMap (OSM) menjadi gambar JPEG. Ini memungkinkan Anda untuk membuat representasi visual dari data OSM, yang dapat berguna untuk berbagai tujuan seperti analisis, presentasi, atau berbagi.

## Persyaratan

*   [Node.js](https://nodejs.org/)
*   [npm](https://www.npmjs.com/)

## Instalasi

1.  Klon repositori ini ke komputer Anda:

    ```bash
    git clone <repository_url>
    cd osm-to-jpeg
    ```

2.  Instal dependensi:

    ```bash
    npm install
    ```

## Penggunaan

1.  Siapkan file konfigurasi. File konfigurasi menentukan parameter untuk konversi, seperti lokasi data OSM, area yang akan dikonversi, dan opsi output. Contoh file konfigurasi diberikan di direktori `config/`.

2.  Jalankan alat:

    ```bash
    node index.js
    ```

3.  Alat akan mengunduh data OSM, memprosesnya, dan menghasilkan gambar JPEG berdasarkan parameter yang ditentukan dalam file konfigurasi. Gambar JPEG akan disimpan di direktori output yang ditentukan dalam file konfigurasi.

## Konfigurasi

File konfigurasi adalah file JSON yang menentukan parameter untuk konversi. Berikut adalah contoh file konfigurasi:

```json
{
  "osm_url": "https://overpass-api.de/api/overpass",
  "bbox": [ -74.0060, 40.7128, -73.9352, 40.7922 ],
  "output_dir": "./output",
  "image_width": 800,
  "image_height": 600,
  "zoom": 14
}
```

*   `osm_url`: URL ke server Overpass API.
*   `bbox`: Batas kotak (bounding box) untuk area yang akan dikonversi. Koordinat harus dalam urutan [longitude minimum, latitude minimum, longitude maksimum, latitude maksimum].
*   `output_dir`: Direktori tempat gambar JPEG akan disimpan.
*   `image_width`: Lebar gambar output dalam piksel.
*   `image_height`: Tinggi gambar output dalam piksel.
*   `zoom`: Tingkat zoom untuk data OSM.

## Contoh

Untuk mengonversi area di sekitar New York City ke gambar JPEG, Anda dapat menggunakan file konfigurasi berikut:

```json
{
  "osm_url": "https://overpass-api.de/api/overpass",
  "bbox": [ -74.0060, 40.7128, -73.9352, 40.7922 ],
  "output_dir": "./output",
  "image_width": 800,
  "image_height": 600,
  "zoom": 14
}
```

Simpan file ini sebagai `config.json` dan jalankan alat menggunakan perintah berikut:

```bash
node index.js
```

Alat akan mengunduh data OSM untuk area di sekitar New York City, memprosesnya, dan menghasilkan gambar JPEG dengan lebar 800 piksel dan tinggi 600 piksel. Gambar JPEG akan disimpan di direktori `output/`.

## Catatan

*   Anda mungkin perlu menyesuaikan parameter dalam file konfigurasi agar sesuai dengan kebutuhan spesifik Anda.
*   Alat ini membutuhkan koneksi internet untuk mengunduh data OSM.
*   Ukuran gambar output dapat bervariasi tergantung pada tingkat zoom dan area yang dikonversi.
*   Pastikan server Overpass API tersedia dan merespons permintaan Anda. Jika tidak, Anda mungkin perlu menggunakan server Overpass API alternatif.

---
