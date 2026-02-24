---
title: Shapefile から SVG への変換
linkTitle: シェープファイルからSVGへ
weight: 10
description: シェープファイルを SVG 形式に変換する方法。
url: /ja/net/viewer/shapefile-to-svg/
aliases: [shapefile to svg, shapefile2svg]
---

## はじめに

このドキュメントでは、シェープファイル (.shp) をスケーラブルなベクターグラフィックス (SVG) 形式に変換する方法について説明します。 シェープファイルは、地理空間データを保存するための一般的な形式であり、SVG は Web 上での表示に適したベクトル画像形式です。

## 前提条件

*   .NET Framework 4.7.2 以降がインストールされていること
*   Visual Studio がインストールされていること (開発用)
*   ShapefileToSvgConverter ライブラリへのアクセス権があること

## シェープファイルを SVG に変換する手順

1.  **プロジェクトの作成:** Visual Studio で新しい .NET コンソールアプリケーションプロジェクトを作成します。
2.  **ShapefileToSvgConverter の参照追加:** プロジェクトに ShapefileToSvgConverter ライブラリを参照を追加します。 NuGet パッケージマネージャーを使用するか、DLL ファイルをプロジェクトに追加できます。
3.  **コードの記述:** シェープファイルを SVG に変換する C# コードを記述します。以下はサンプルコードです。

```csharp
// ShapefileToSvgConverter の名前空間参照を追加
using ShapefileToSvgConverter;

public class Program
{
    public static void Main(string[] args)
    {
        // シェープファイルのパスと SVG ファイルのパスを指定
        string shapefilePath = "path/to/your/shapefile.shp";
        string svgFilePath = "path/to/your/output.svg";

        // ShapefileToSvgConverter を使用してシェープファイルを SVG に変換
        try
        {
            ShapefileToSvgConverter.Converter converter = new Converter();
            converter.Convert(shapefilePath, svgFilePath);
            Console.WriteLine("変換が完了しました。");
        }
        catch (Exception ex)
        {
            Console.WriteLine($"エラーが発生しました: {ex.Message}");
        }
    }
}
```

4.  **コードの実行:** プロジェクトをビルドして実行します。 シェープファイルが SVG 形式に変換され、指定した出力パスに保存されます。

## オプション

ShapefileToSvgConverter ライブラリは、SVG の生成方法をカスタマイズするためのさまざまなオプションを提供します。 これらのオプションには以下が含まれます。

*   **線の太さ:** SVG の線の太さを設定します。
*   **塗りつぶしの色:** SVG のポリゴンの塗りつぶし色を設定します。
*   **アウトラインの色:** SVG のポリゴンのアウトラインの色を設定します。
*   **座標系の変換:** シェープファイルの座標系を SVG 座標系に変換します。

これらのオプションの詳細については、ShapefileToSvgConverter ライブラリのドキュメントを参照してください。

## トラブルシューティング

シェープファイルを SVG に変換する際に問題が発生した場合は、以下の点を確認してください。

*   シェープファイルが有効な形式であること
*   ShapefileToSvgConverter ライブラリが正しく参照されていること
*   出力パスに書き込み権限があること
*   必要な依存関係がすべてインストールされていること

## まとめ

このドキュメントでは、シェープファイルを SVG 形式に変換する方法について説明しました。 ShapefileToSvgConverter ライブラリを使用すると、シェープファイルを簡単に SVG に変換し、Web 上での表示に適したベクトル画像を作成できます。
---
