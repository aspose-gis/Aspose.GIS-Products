---
title: GeoJSONからSVGへの変換
linkTitle: GeoJSONからSVGへ
weight: 10
description: GeoJSONデータをSVG形式に変換するツールです。
url: /ja/viewer/geojson-to-svg/
aliases: [geojson2svg, geojson-to-svg]
---

## 概要

このツールは、GeoJSONデータをSVG（Scalable Vector Graphics）形式に変換します。地図データや地理情報をウェブページで表示する際に便利です。

## 機能

*   **GeoJSONデータの読み込み:**  ローカルファイルまたはURLからGeoJSONデータを読み込むことができます。
*   **SVG形式への変換:** 読み込んだGeoJSONデータをSVG形式に変換します。
*   **SVGのカスタマイズ:** SVGのスタイル（線の色、太さ、塗りつぶしなど）を調整できます。
*   **SVGのエクスポート:**  生成されたSVGファイルをダウンロードできます。

## 使用方法

1.  **GeoJSONデータの準備:** 変換したいGeoJSONデータを用意します。
2.  **ツールの起動:** このツールを開きます。
3.  **GeoJSONデータの読み込み:** 「ファイルを選択」ボタンをクリックしてローカルのGeoJSONファイルを選択するか、「URLを入力」欄にGeoJSONデータのURLを入力します。
4.  **変換とカスタマイズ:** ツールが自動的にGeoJSONデータをSVGに変換します。必要に応じて、スタイルを調整します。
5.  **SVGのエクスポート:** 「ダウンロード」ボタンをクリックして、生成されたSVGファイルを保存します。

## 注意事項

*   GeoJSONデータの複雑さによっては、SVGの生成に時間がかかる場合があります。
*   非常に大きなGeoJSONデータの場合、ブラウザのパフォーマンスが低下する可能性があります。
*   変換されるSVGは、元のGeoJSONデータの構造を反映したものです。必要に応じて、SVGを手動で編集して調整してください。

## 例

以下は、GeoJSONデータをSVGに変換する例です。

**入力 (GeoJSON):**

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [[
          [139.6916, 35.6894],
          [139.7024, 35.6894],
          [139.7024, 35.6953],
          [139.6916, 35.6953],
          [139.6916, 35.6894]
        ]]
      },
      "properties": {
        "name": "東京"
      }
    }
  ]
}
```

**出力 (SVG):**

（変換されたSVGコードが表示されます）

## 参考情報

*   [GeoJSON](https://geojson.org/)
*   [SVG](https://www.w3.org/Graphics/SVG/)

