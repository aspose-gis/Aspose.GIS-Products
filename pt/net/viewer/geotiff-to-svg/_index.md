---
title: GeoTIFF to SVG Conversion
linkTitle: Conversão de GeoTIFF para SVG
weight: 10
url: /pt/net/viewer/geotiff-to-svg/
description: Learn how to convert GeoTIFF images to scalable vector graphics (SVG) format using .NET.
descrição: Aprenda como converter imagens GeoTIFF para o formato de gráficos vetoriais escaláveis (SVG) usando .NET.
---

## Introduction
introdução:

This guide explains the process of converting GeoTIFF files into SVG format using a .NET viewer. This allows for vector-based rendering of raster data, which can be beneficial for web applications and other scenarios where scalability and interactivity are required.
Esta guia explica o processo de conversão de arquivos GeoTIFF para o formato SVG usando um visualizador .NET. Isso permite a renderização baseada em vetor de dados rasterizados, o que pode ser benéfico para aplicativos da web e outros cenários onde escalabilidade e interatividade são necessárias.

## Prerequisites
pré-requisitos:

*   A .NET development environment (e.g., Visual Studio)
*   The necessary libraries for GeoTIFF and SVG manipulation (e.g., NetTopologySuite, ImageMagick)
*   A GeoTIFF file to convert
*   Um ambiente de desenvolvimento .NET (por exemplo, Visual Studio)
*   As bibliotecas necessárias para manipulação de GeoTIFF e SVG (por exemplo, NetTopologySuite, ImageMagick)
*   Um arquivo GeoTIFF para converter

## Conversion Steps
etapas de conversão:

1.  **Load the GeoTIFF image:** Use a library like NetTopologySuite to load the GeoTIFF file and extract its raster data and geographic coordinates.
    Carregue a imagem GeoTIFF: use uma biblioteca como NetTopologySuite para carregar o arquivo GeoTIFF e extrair seus dados rasterizados e coordenadas geográficas.

2.  **Rasterize the image:** Convert the raster data into vector paths by sampling pixel values and creating corresponding lines or polygons.
    Rastere a imagem: converta os dados rasterizados em caminhos vetoriais amostrando valores de pixels e criando linhas ou polígonos correspondentes.

3.  **Create SVG elements:** Generate SVG path elements based on the created vector paths, ensuring that each element accurately represents the original pixel data.
    Crie elementos SVG: gere elementos de caminho SVG com base nos caminhos vetoriais criados, garantindo que cada elemento represente com precisão os dados originais do pixel.

4.  **Save the SVG file:** Save the generated SVG elements into a valid SVG file format.
    Salve o arquivo SVG: salve os elementos SVG gerados em um formato de arquivo SVG válido.

## Code Example
exemplo de código:

```csharp
// Sample code demonstrating GeoTIFF to SVG conversion (simplified)
// Código de exemplo demonstrando conversão de GeoTIFF para SVG (simplificado)

using NetTopologySuite.Geometries;
using System;
using System.Drawing;
using System.Drawing.Imaging;

public class GeotiffToSvgConverter
{
    public static string ConvertGeoTiffToSvg(string geoTiffFilePath, double scale)
    {
        // Load GeoTIFF data
        // Carregar dados GeoTIFF
        Bitmap bitmap = new Bitmap(geoTiffFilePath);

        // Create SVG document
        // Criar documento SVG
        string svgDocument = $"<svg width=\"{bitmap.Width * scale}\" height=\"{bitmap.Height * scale}\">";

        // Iterate over pixels and create paths
        // Iterar sobre os pixels e criar caminhos
        for (int y = 0; y < bitmap.Height; y++)
        {
            for (int x = 0; x < bitmap.Width; x++)
            {
                Color pixelColor = bitmap.GetPixel(x, y);

                // Create a path for the pixel if it meets certain criteria
                // Criar um caminho para o pixel se ele atender certos critérios
                if (pixelColor.R > 100)
                {
                    svgDocument += $"<path d=\"M {x * scale} {y * scale}\" fill=\"red\" />";
                }
            }
        }

        // Close SVG document
        // Fechar documento SVG
        svgDocument += "</svg>";

        return svgDocument;
    }
}
```

## Considerations
considerações:

*   **Scalability:** The conversion process can be computationally intensive for large GeoTIFF files. Consider optimizing the rasterization and vectorization steps to improve performance.
    Escalabilidade: o processo de conversão pode ser computacionalmente intensivo para arquivos GeoTIFF grandes. Considere otimizar as etapas de rasterização e vetorização para melhorar o desempenho.

*   **Accuracy:** The accuracy of the resulting SVG file depends on the sampling rate and vectorization algorithm used. Experiment with different settings to achieve the desired level of detail.
    Precisão: a precisão do arquivo SVG resultante depende da taxa de amostragem e do algoritmo de vetorização usados. Experimente diferentes configurações para atingir o nível de detalhe desejado.

*   **File Size:** The size of the resulting SVG file can be significant, especially for complex GeoTIFF images. Consider using compression techniques to reduce file size.
    Tamanho do arquivo: o tamanho do arquivo SVG resultante pode ser significativo, especialmente para imagens GeoTIFF complexas. Considere usar técnicas de compressão para reduzir o tamanho do arquivo.

## Conclusion
conclusão:

Converting GeoTIFF files to SVG format provides a powerful way to render raster data in vector-based applications. By following the steps outlined in this guide and considering the associated considerations, you can effectively convert your GeoTIFF images into scalable and interactive SVG graphics.
Converter arquivos GeoTIFF para o formato SVG fornece uma maneira poderosa de renderizar dados rasterizados em aplicativos baseados em vetor. Seguindo as etapas descritas neste guia e considerando as considerações associadas, você pode efetivamente converter suas imagens GeoTIFF em gráficos SVG escaláveis ​​e interativos.

---
