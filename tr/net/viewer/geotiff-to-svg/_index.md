---
title: GeoTIFF to SVG Conversion
linkTitle: GeoTIFF’ı SVG’ye Dönüştürme
weight: 10
url: /tr/net/viewer/geotiff-to-svg/
aliases: [geotiff, svg, conversion, raster, vector]
---

## Overview
## Genel Bakış

This viewer allows you to convert GeoTIFF files into SVG format.
Bu görüntüleyici, GeoTIFF dosyalarını SVG biçimine dönüştürmenizi sağlar.  You can adjust various parameters to control the output quality and appearance.
Çıktı kalitesini ve görünümünü kontrol etmek için çeşitli parametreleri ayarlayabilirsiniz.

## Usage
## Kullanım

1.  **Upload GeoTIFF:** Drag and drop your GeoTIFF file or click "Choose File" to upload it.
    **GeoTIFF Yüklemesi:** GeoTIFF dosyanızı sürükleyip bırakın veya yüklemek için "Dosya Seçin"’e tıklayın.
2.  **Adjust Parameters (Optional):** Modify the parameters below to fine-tune the conversion process.
    **Parametreleri Ayarlama (İsteğe Bağlı):** Dönüştürme işlemini iyileştirmek için aşağıdaki parametreleri değiştirin.
3.  **Convert:** Click "Convert" to start the conversion.
    **Dönüştür:** Dönüşümü başlatmak için "Dönüştür"’e tıklayın.
4.  **Download SVG:** Once the conversion is complete, download the resulting SVG file.
    **SVG İndirme:** Dönüştürme tamamlandıktan sonra sonuçlanan SVG dosyasını indirin.

## Parameters
## Parametreler

*   **Resolution (DPI):** The resolution of the output SVG image in dots per inch.  Higher values result in larger files and more detail.
    **Çözünürlük (DPI):** Nokta başına inç cinsinden çıktı SVG görüntüsünün çözünürlüğü. Daha yüksek değerler daha büyük dosyalara ve daha fazla ayrıntıya neden olur.
*   **Color Clipping:**  Defines the color range to be included in the conversion. Colors outside this range will be clipped (removed).
    **Renk Kırpma:** Dönüştürmeye dahil edilecek renk aralığını tanımlar. Bu aralık dışındaki renkler kırpılır (kaldırılır).
*   **Simplify Tolerance:**  A value that controls how much the vector lines are simplified during conversion. Lower values preserve more detail but result in larger files. Higher values simplify the lines more aggressively, resulting in smaller files.
    **Basitleştirme Toleransı:** Dönüştürme sırasında vektör çizgilerinin ne kadar basitleştirileceğini kontrol eden bir değerdir. Daha düşük değerler daha fazla ayrıntıyı korur ancak daha büyük dosyalara neden olur. Daha yüksek değerler çizgileri daha agresif bir şekilde basitleştirir ve daha küçük dosyalara neden olur.
*   **Output Format:** Select the desired output format (e.g., SVG, PNG).
    **Çıktı Biçimi:** İstediğiniz çıktı biçimini seçin (örneğin, SVG, PNG).

## Notes
## Notlar

*   Large GeoTIFF files may take a significant amount of time to convert.
    Büyük GeoTIFF dosyalarının dönüştürülmesi önemli ölçüde zaman alabilir.
*   The quality of the resulting SVG file depends on the resolution and simplification settings.
    Sonuçlanan SVG dosyasının kalitesi çözünürlük ve basitleştirme ayarlarına bağlıdır.
*   This tool is intended for raster-to-vector conversion only. It does not support other image formats.
    Bu araç yalnızca rastan vektöre dönüştürme için tasarlanmıştır. Diğer görüntü formatlarını desteklemez.

---
