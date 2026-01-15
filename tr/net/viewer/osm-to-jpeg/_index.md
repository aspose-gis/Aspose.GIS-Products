---
title: OSM'yi JPEG'e Dönüştürme
linkTitle: OSM'yi JPEG'e Dönüştürme
weight: 10
url: /tr/net/viewer/osm-to-jpeg/
description: Açık Kaynak Harita Verilerini (OSM) JPEG Görüntülerine Dönüştürme Aracı.
---

## Açıklama

Bu araç, OpenStreetMap (OSM) verilerini JPEG görüntü formatına dönüştürmenizi sağlar.  Haritaları görselleştirmek ve paylaşmak için kullanışlıdır.

## Gereksinimler

*   .NET 6 SDK veya üzeri
*   Windows, Linux veya macOS işletim sistemi

## Kurulum

1.  Depoyu klonlayın:

    ```bash
    git clone [depo_url](https://github.com/your-username/osm-to-jpeg)
    cd osm-to-jpeg
    ```

2.  Bağımlılıkları yükleyin:

    ```bash
    dotnet restore
    ```

## Kullanım

1.  Bir yapılandırma dosyası oluşturun (`config.json`). Aşağıda bir örnek yapılandırma dosyası bulunmaktadır:

    ```json
    {
      "outputDirectory": "output",
      "osmSource": "https://overpass-api.de/api/overpass?bbox=-180,-90,180,90&data=full",
      "tileSize": 256,
      "zoomLevel": 10,
      "outputFormat": "jpeg"
    }
    ```

    *   `outputDirectory`: Çıktı JPEG dosyalarının kaydedileceği dizin.
    *   `osmSource`: OSM verilerini almak için kullanılacak Overpass API URL'si.
    *   `tileSize`: Oluşturulacak her bir kiremit görüntüsünün boyutu (piksel cinsinden).
    *   `zoomLevel`: Haritanın yakınlaştırma seviyesi.
    *   `outputFormat`: Çıktı dosya formatı (jpeg, png vb.).

2.  Aracı çalıştırın:

    ```bash
    dotnet run --config config.json
    ```

## Notlar

*   Overpass API'si yoğun kullanıma sahip olabilir. Daha hızlı sonuçlar için kendi Overpass API sunucunuzu ayarlamayı düşünebilirsiniz.
*   `osmSource` URL'sinin geçerli bir OSM veri kaynağına işaret ettiğinden emin olun.
*   Çıktı JPEG dosyaları, belirtilen `outputDirectory` dizinine kaydedilecektir.

## Lisans

[Lisans Bilgileri](LICENSE)
---
