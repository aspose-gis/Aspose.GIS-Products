---
title: MapInfo Tab
linkTitle: Tab MapInfo
weight: 10
url: /id/net/viewer/mapinfo-tab/
aliases: [mapinfo, tab]
[source](https://github.com/NetMapStudio/net.viewer/blob/master/src/net/viewer/mapinfo-tab.cpp)
---

## MapInfo Tab

Tab ini memungkinkan Anda untuk mengimpor dan bekerja dengan data dari file MapInfo.

### Format yang Didukung

Format berikut didukung:

*   `.tab` - File tab standar MapInfo.

### Mengimpor Data

Untuk mengimpor data, lakukan hal berikut:

1.  Buka menu "File" -> "Import".
2.  Pilih format file "MapInfo Tab".
3.  Telusuri dan pilih file `.tab`.
4.  Klik tombol "Open".

### Opsi Impor

Saat mengimpor data, Anda dapat menentukan opsi berikut:

*   **Encoding:** Pilih encoding karakter yang digunakan dalam file. Jika Anda tidak yakin, coba gunakan "UTF-8".
*   **Koordinat Geografis:** Tentukan apakah file berisi koordinat geografis. Jika ya, tentukan sistem koordinat yang digunakan.
*   **Proyeksi:** Tentukan proyeksi yang digunakan untuk data.

### Bekerja dengan Data

Setelah mengimpor data, Anda dapat bekerja dengannya seperti halnya data lainnya di NetMapStudio. Anda dapat:

*   Melihat dan menavigasi data.
*   Melakukan kueri pada data.
*   Membuat peta dan grafik dari data.
*   Mengekspor data ke format lain.

### Catatan

*   File `.tab` biasanya sangat besar, jadi impor mungkin membutuhkan waktu beberapa saat.
*   Pastikan Anda memiliki cukup memori untuk memuat file `.tab`.
*   Jika Anda mengalami masalah saat mengimpor data, coba gunakan encoding karakter yang berbeda.

