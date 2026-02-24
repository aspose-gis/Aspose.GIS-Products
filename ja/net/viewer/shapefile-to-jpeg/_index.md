---
title: Shapefile を JPEG に変換する
linkTitle: シェープファイルをJPEGに変換する
weight: 10
description: .shp ファイルを JPEG 画像に変換する方法。
url: /ja/net/viewer/shapefile-to-jpeg/
aliases: [shapefile to jpeg, shapefile to jpg]
---

## Shapefile を JPEG に変換する

このドキュメントでは、.shp ファイルを JPEG 画像に変換する方法について説明します。

### 前提条件

*   .NET Viewer がインストールされていること。
*   Shapefile との互換性のある地理空間データが含まれていること。

### 手順

1.  .NET Viewer を起動します。
2.  「ファイル」メニューから「開く」を選択し、変換する Shapefile (.shp) を選択します。
3.  Shapefile が表示されたら、「変換」メニューから「JPEG にエクスポート」を選択します。
4.  出力 JPEG ファイルの名前と場所を指定します。
5.  必要に応じて、解像度や品質などのエクスポート設定を調整します。
6.  「保存」をクリックして変換を開始します。

### コマンドラインオプション

Shapefile を JPEG に変換するには、コマンドラインを使用することもできます。

```
dotnet viewer.exe -i input.shp -o output.jpg -f jpeg
```

`-i` オプションは入力 Shapefile を指定し、`-o` オプションは出力 JPEG ファイルを指定し、`-f` オプションは出力形式を指定します。

### トラブルシューティング

*   Shapefile が開けない場合は、ファイルが破損していないか確認してください。
*   JPEG ファイルをエクスポートできない場合は、必要なライブラリがインストールされていることを確認してください。
*   変換された JPEG 画像の品質が低い場合は、エクスポート設定を調整してみてください。

### 追加情報

*   .NET Viewer のドキュメント: [https://www.example.com/dotnet-viewer](https://www.example.com/dotnet-viewer)
*   Shapefile の仕様: [https://www.esri.com/arcgis/products/shapefile](https://www.esri.com/arcgis/products/shapefile)
---
