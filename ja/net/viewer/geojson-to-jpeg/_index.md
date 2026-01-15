---
title: GeoJSON を JPEG に変換
url: /ja/viewer/geojson-to-jpeg/
weight: 10
layout: "default"
description: 地図データを画像形式に変換する方法を説明します。
---

## GeoJSON からの JPEG への変換

このツールを使用すると、GeoJSON ファイルを JPEG 画像に変換できます。これは、地図データの視覚化や共有に役立ちます。

### 前提条件

*   [NetViewer](https://github.com/netviewer-org/netviewer) がインストールされていること
*   GeoJSON ファイルがあること

### 使い方

1.  コマンドラインを開きます。
2.  `netviewer` コマンドを実行します。
    ```bash
    netviewer geojson-to-jpeg -i <geojson_file> -o <output_image.jpg>
    ```
    *   `-i`: 入力 GeoJSON ファイルのパスを指定します。
    *   `-o`: 出力 JPEG 画像のファイル名を指定します。

### 例

次のコマンドは、`data.geojson` を `output.jpg` に変換します。

```bash
netviewer geojson-to-jpeg -i data.geojson -o output.jpg
```

### オプション

*   `-s`: 縮尺を指定します (デフォルト: 1000)。
*   `-r`: 解像度を指定します (デフォルト: 512x512)。
*   `-c`: カラーパレットを指定します。
*   `-b`: 背景色を指定します。

### 注意事項

*   GeoJSON ファイルは有効な形式である必要があります。
*   出力画像のサイズは、入力データの複雑さによって異なります。
*   このツールは、NetViewer の機能を利用しています。

### トラブルシューティング

*   **エラー: GeoJSON ファイルが見つからない:** 入力ファイルのパスが正しいことを確認してください。
*   **エラー: JPEG 画像の作成に失敗しました:** 出力ファイル名が有効であることを確認し、書き込み権限があるディレクトリを指定してください。
*   **出力画像が期待どおりにならない:** オプションを使用して、縮尺、解像度、カラーパレット、背景色を調整してみてください。

### 関連情報

*   [NetViewer](https://github.com/netviewer-org/netviewer)
*   [GeoJSON](https://geojson.org/)
---
