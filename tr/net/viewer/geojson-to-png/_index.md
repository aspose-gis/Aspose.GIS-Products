---
title: GeoJSON'dan PNG'ye Dönüştürücü
linkTitle: GeoJSON'dan PNG'ye
weight: 10
url: /tr/net/viewer/geojson-to-png/
description: .NET Viewer ile GeoJSON verilerini görüntüleyin ve PNG olarak dışa aktarın.
---

## GeoJSON'dan PNG'ye Dönüştürme

Bu araç, bir GeoJSON dosyasını alır ve onu bir PNG görüntüsüne dönüştürür. Bu, haritaları veya diğer coğrafi verileri görüntülemek için kullanışlıdır.

### Gereksinimler

*   .NET 6.0 veya üzeri
*   [GeoJSON.Net](https://www.nuget.org/packages/GeoJSON.Net/)
*   [ImageSharp](https://www.nuget.org/packages/SixLabors.ImageSharp/)

### Kurulum

1.  Bu depoyu klonlayın veya indirin.
2.  Çözüm dosyasını (.sln) bir geliştirme ortamında açın (örneğin, Visual Studio).
3.  Projeyi derleyin.

### Kullanım

Araç satır komutundan çalıştırılabilir.

```bash
geojson-to-png --input input.geojson --output output.png --width 512 --height 512
```

Bu, `input.geojson` dosyasını okur ve onu `output.png` dosyasına dönüştürür. Görüntünün genişliği 512 piksel ve yüksekliği 512 piksel olacaktır.

### Seçenekler

*   `--input`: GeoJSON dosyasının yolu.
*   `--output`: PNG görüntüsünün yolu.
*   `--width`: Görüntünün genişliği (piksel cinsinden).
*   `--height`: Görüntünün yüksekliği (piksel cinsinden).

### Notlar

*   GeoJSON dosyası geçerli olmalıdır.
*   Görüntü, GeoJSON dosyasındaki özelliklerin sayısına bağlı olarak büyük olabilir.
*   Bu araç, haritaları veya diğer coğrafi verileri görüntülemek için kullanışlıdır.

