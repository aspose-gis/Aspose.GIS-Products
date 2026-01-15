---
title: GPX Dosyaları
linkTitle: GPX Dosyaları
weight: 10
url: /tr/gpx/
description: GPX dosyası nedir ve nasıl kullanılır?
---

## GPX Nedir?

GPX (GPS Exchange Format) bir XML dosya formatıdır. GPS verilerini, coğrafi konumları, rotaları, yolları ve noktaları depolamak için kullanılır. Genellikle yürüyüşler, bisiklet sürüşleri, araba yolculukları ve diğer açık hava etkinlikleri sırasında kaydedilen verileri paylaşmak için kullanılır.

## GPX Dosyası Formatı

GPX dosyaları XML formatındadır, bu da onları okunabilir ve ayrıştırılabilir hale getirir. Bir GPX dosyasında aşağıdaki öğeler bulunabilir:

*   **way:** Bir dizi nokta içeren bir yol tanımlar.
*   **route:** Bir dizi nokta içeren bir rota tanımlar.
*   **track:** Zaman damgaları ile birlikte bir dizi nokta içeren bir iz tanımlar.
*   **wpt:** Bir coğrafi konumun koordinatlarını ve ek bilgilerini (ad, açıklama vb.) tanımlayan bir nokta tanımlar.

## GPX Dosyası Nasıl Kullanılır?

GPX dosyaları çeşitli GPS cihazlarında, harita yazılımlarında ve diğer uygulamalarda kullanılabilir. Örneğin:

*   GPS cihazlarına GPX dosyalarını yükleyerek navigasyon için kullanabilirsiniz.
*   Harita yazılımlarında GPX dosyalarını açarak rotalarınızı, yollarınızı ve noktalarınızı görüntüleyebilirsiniz.
*   GPX dosyalarını diğer formatlara (örneğin, KML) dönüştürebilirsiniz.

## GPX Dosyası Örneği

Aşağıda basit bir GPX dosyasının örneği verilmiştir:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<gpx version="1.1">
  <trk>
    <name>Yürüyüş Rotası</name>
    <trkseg>
      <wpt lat="37.7749" lon="-122.4194">
        <name>Başlangıç Noktası</name>
        <desc>Yürüyüşün başlangıç noktası.</desc>
      </wpt>
      <pt lat="37.7833" lon="-122.4065"/>
    </trkseg>
  </trk>
</gpx>
```

Bu örnekte, "Yürüyüş Rotası" adlı bir iz tanımlanmıştır. İz, başlangıç noktası ve başka bir nokta olmak üzere iki nokta içerir. Başlangıç noktasının adı "Başlangıç Noktası"dır ve açıklaması "Yürüyüşün başlangıç noktası." şeklindedir.

## GPX Dosyalarını İndirme ve Yükleme

Çeşitli web sitelerinden GPX dosyaları indirebilirsiniz. Örneğin:

*   [AllTrails](https://www.alltrails.com/)
*   [GPXMania](https://www.gpxmania.com/)

GPX dosyalarını indirdikten sonra, bunları GPS cihazınıza veya harita yazılımınıza yükleyebilirsiniz.

---
