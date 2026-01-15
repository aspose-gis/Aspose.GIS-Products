---
title: Перетворення GeoTIFF у PNG
url: /uk/net/viewer/geotiff-to-png/
weight: 10
layout: single
draft: false
description: Інструмент для перетворення файлів GeoTIFF у формат PNG.
aliases: [geotiff2png, geotiff to png]
---

## Перетворення GeoTIFF у PNG за допомогою .NET Viewer

Цей інструмент дозволяє перетворювати файли GeoTIFF у формат PNG. Він надає простий інтерфейс для вибору вхідного файлу GeoTIFF та збереження результату як зображення PNG.

### Функціональність

*   Вибір файлу GeoTIFF: Виберіть файл GeoTIFF, який потрібно перетворити.
*   Параметри перетворення: Налаштуйте параметри перетворення, такі як роздільна здатність та колірна палітра.
*   Збереження PNG: Збережіть перетворене зображення у форматі PNG.

### Використання

1.  Завантажте .NET Viewer.
2.  Відкрийте інструмент перетворення GeoTIFF у PNG.
3.  Виберіть файл GeoTIFF, який потрібно перетворити.
4.  Налаштуйте параметри перетворення за потреби.
5.  Збережіть перетворене зображення у форматі PNG.

### Приклад коду

```csharp
// Цей код демонструє, як перетворити GeoTIFF у PNG за допомогою .NET Viewer.
// Замініть "input.tif" на шлях до вашого файлу GeoTIFF.
// Замініть "output.png" на бажаний шлях для збереження файлу PNG.

GeoTiffRaster raster = new GeoTiffRaster("input.tif");
PngBitmapEncoder encoder = new PngBitmapEncoder();
encoder.Frames.Add(raster);
File.WriteAllBytes("output.png", encoder.Encode());
```

### Зауваження

*   Переконайтеся, що у вас встановлено .NET Framework 4.7 або новішу версію.
*   Для перетворення великих файлів GeoTIFF може знадобитися більше часу та ресурсів.
*   Результат якості перетвореного зображення PNG залежить від параметрів перетворення.

### Подальша інформація

*   [GeoTIFF](https://www.geotiff.org/)
*   [.NET Viewer](https://example.com/net-viewer) - Замініть на реальний URL

