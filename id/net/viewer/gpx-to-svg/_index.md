---
title: GPX ke SVG
linkTitle: GPX ke SVG
weight: 10
description: Konversi berkas GPX menjadi gambar SVG.
url: /id/gpx-to-svg/
aliases: [GPX to SVG]
source: https://github.com/netviewer/gpx-to-svg
---

## Tentang

Konverter GPX ke SVG memungkinkan Anda mengonversi berkas GPX menjadi gambar SVG yang dapat digunakan dalam aplikasi web atau desktop. Alat ini ditulis dalam Rust dan dirancang untuk menjadi cepat, efisien, dan mudah digunakan.

## Fitur

*   Konversi berkas GPX menjadi gambar SVG
*   Dukungan untuk berbagai format GPX
*   Opsi untuk menyesuaikan tampilan SVG
*   Antarmuka baris perintah yang sederhana
*   Dapat digunakan sebagai pustaka dalam proyek Rust Anda sendiri

## Instalasi

Anda dapat menginstal `gpx-to-svg` dari [crates.io](https://crates.io/crates/gpx-to-svg).

```bash
cargo install gpx-to-svg
```

## Penggunaan

Setelah terinstal, Anda dapat menggunakan `gpx-to-svg` untuk mengonversi berkas GPX menjadi gambar SVG dengan perintah berikut:

```bash
gpx-to-svg input.gpx > output.svg
```

Ini akan mengonversi `input.gpx` menjadi gambar SVG dan menyimpannya ke `output.svg`.

## Opsi

`gpx-to-svg` mendukung sejumlah opsi untuk menyesuaikan tampilan SVG. Untuk melihat daftar lengkap opsi, gunakan perintah berikut:

```bash
gpx-to-svg --help
```

## Contoh

Berikut adalah beberapa contoh penggunaan `gpx-to-svg`:

*   Untuk mengonversi berkas GPX menjadi gambar SVG dengan resolusi yang lebih tinggi:

    ```bash
    gpx-to-svg --width 2048 --height 2048 input.gpx > output.svg
    ```

*   Untuk mengonversi berkas GPX menjadi gambar SVG dengan warna latar belakang putih:

    ```bash
    gpx-to-svg --background-color white input.gpx > output.svg
    ```

*   Untuk mengonversi berkas GPX menjadi gambar SVG dalam format PNG:

    ```bash
    gpx-to-svg -o output.png input.gpx
    ```

## Dokumentasi

Dokumentasi lengkap untuk `gpx-to-svg` dapat ditemukan di [https://netviewer.github.io/gpx-to-svg/](https://netviewer.github.io/gpx-to-svg/).

## Kontribusi

Kontribusi ke `gpx-to-svg` dipersilakan. Jika Anda menemukan bug atau memiliki saran untuk perbaikan, jangan ragu untuk membuka masalah di [GitHub](https://github.com/netviewer/gpx-to-svg).
