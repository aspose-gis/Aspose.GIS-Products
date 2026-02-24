---
title: SHP to JPEG Conversion
linkTitle: SHP’den JPEG’e Dönüştürme
weight: 10
url: /tr/net/viewer/shp-to-jpeg/
aliases: [shp2jpg, shp to jpg]
description: Convert shapefiles (.shp) to JPEG images.
açıklama: Şekil dosyalarını (.shp) JPEG resimlerine dönüştürün.
---

## Overview
## Genel Bakış

This tool converts shapefiles (.shp) into JPEG images. You can control the output resolution, background color, and other parameters.
Bu araç, şekil dosyalarını (.shp) JPEG resimlerine dönüştürür. Çıkış çözünürlüğü, arka plan rengi ve diğer parametreleri kontrol edebilirsiniz.

## Usage
## Kullanım

1.  **Input Shapefile:** Select the `.shp` file you want to convert.
    **Girdi Şekil Dosyası:** Dönüştürmek istediğiniz `.shp` dosyasını seçin.
2.  **Output JPEG File:** Specify the name and location for the resulting JPEG image.
    **Çıkış JPEG Dosyası:** Sonuç JPEG görüntüsü için ad ve konumu belirtin.
3.  **Resolution:** Set the desired resolution (DPI) for the output image. Higher DPI means better quality but larger file size.
    **Çözünürlük:** Çıkış görüntüsü için istenen çözünürlüğü (DPI) ayarlayın. Daha yüksek DPI, daha iyi kalite ancak daha büyük dosya boyutu anlamına gelir.
4.  **Background Color:** Choose a background color for the image. Options include white, black, and custom colors.
    **Arka Plan Rengi:** Görüntü için bir arka plan rengi seçin. Seçenekler arasında beyaz, siyah ve özel renkler bulunur.
5.  **Convert:** Click the "Convert" button to start the conversion process.
    **Dönüştür:** Dönüşüm işlemini başlatmak için "Dönüştür" düğmesine tıklayın.

## Parameters
## Parametreler

*   `inputShapefile`: The path to the input shapefile (.shp).
    `inputShapefile`: Girdi şekil dosyasının (.shp) yolu.
*   `outputJpegFile`: The path to save the output JPEG image.
    `outputJpegFile`: Çıkış JPEG görüntüsünü kaydetmek için yol.
*   `resolution`: The resolution (DPI) of the output image. Default is 300.
    `resolution`: Çıkış görüntüsünün çözünürlüğü (DPI). Varsayılan değer 300'dür.
*   `backgroundColor`: The background color for the image.  Can be "white", "black", or a custom hex code (e.g., "#FF0000" for red).
    `backgroundColor`: Görüntü için arka plan rengi. "beyaz", "siyah" veya özel bir onaltılık kod olabilir (örneğin, kırmızı için "#FF0000").

## Example
## Örnek

```java
// Convert shapefile to JPEG with default settings
ShapefileToJpegConverter converter = new ShapefileToJpegConverter();
converter.setInputShapefile("path/to/input.shp");
converter.setOutputJpegFile("path/to/output.jpg");
converter.convert();

// Convert shapefile to JPEG with custom resolution and background color
ShapefileToJpegConverter converter = new ShapefileToJpegConverter();
converter.setInputShapefile("path/to/input.shp");
converter.setOutputJpegFile("path/to/output.jpg");
converter.setResolution(600);
converter.setBackgroundColor("#00FF00"); // Green background
converter.convert();
```

## Troubleshooting
## Sorun Giderme

*   **Error: Invalid Shapefile:** Make sure the input file is a valid shapefile (.shp).
    **Hata: Geçersiz Şekil Dosyası:** Girdi dosyasının geçerli bir şekil dosyası (.shp) olduğundan emin olun.
*   **Error: Could not write to output file:** Check if you have write permissions to the specified output location.
    **Hata: Çıkış dosyasına yazılamadı:** Belirtilen çıkış konumuna yazma izinleriniz olup olmadığını kontrol edin.
*   **Output image is blurry:** Increase the resolution (DPI) setting.
    **Çıkış görüntüsü bulanıktır:** Çözünürlük (DPI) ayarını artırın.

---
