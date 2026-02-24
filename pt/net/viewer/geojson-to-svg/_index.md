---
title: GeoJSON to SVG Conversion
linkTitle: Conversão de GeoJSON para SVG
weight: 10
url: /pt/viewer/geojson-to-svg/
description: Convert GeoJSON data to SVG format for rendering in web browsers and other applications.
descrição: Converta dados GeoJSON para o formato SVG para renderização em navegadores da web e outros aplicativos.
---

## Overview
## Visão geral

This tool converts GeoJSON data into an SVG (Scalable Vector Graphics) representation.  SVG is a vector image format that can be rendered natively in web browsers, making it ideal for interactive mapping applications.
Esta ferramenta converte dados GeoJSON em uma representação SVG (Gráficos Vetoriais Escaláveis). SVG é um formato de imagem vetorial que pode ser renderizado nativamente em navegadores da web, tornando-o ideal para aplicativos de mapeamento interativos.

## Input Data
## Dados de entrada

The tool accepts GeoJSON data as input.  This can be a GeoJSON file or a GeoJSON string.
A ferramenta aceita dados GeoJSON como entrada. Isso pode ser um arquivo GeoJSON ou uma string GeoJSON.

## Output Format
## Formato de saída

The output is an SVG file that represents the geometry defined in the GeoJSON data.  The SVG can be downloaded and used in web pages or other applications.
A saída é um arquivo SVG que representa a geometria definida nos dados GeoJSON. O SVG pode ser baixado e usado em páginas da web ou outros aplicativos.

## Usage
## Uso

1.  **Provide GeoJSON Data:** Paste your GeoJSON data into the input area, or upload a GeoJSON file.
    **Fornecer Dados GeoJSON:** Cole seus dados GeoJSON na área de entrada ou carregue um arquivo GeoJSON.
2.  **Adjust Options (Optional):** Customize the SVG output by adjusting options such as stroke color, fill color, and line width.
    **Ajustar Opções (Opcional):** Personalize a saída SVG ajustando opções como cor do traçado, cor de preenchimento e largura da linha.
3.  **Convert:** Click the "Convert" button to generate the SVG file.
    **Converter:** Clique no botão "Converter" para gerar o arquivo SVG.
4.  **Download:** Download the generated SVG file.
    **Baixar:** Baixe o arquivo SVG gerado.

## Options
## Opções

*   **Stroke Color:** The color of the lines used to draw the features.
    **Cor do Traçado:** A cor das linhas usadas para desenhar os recursos.
*   **Fill Color:** The color used to fill the polygons and other shapes.
    **Cor de Preenchimento:** A cor usada para preencher polígonos e outras formas.
*   **Line Width:** The thickness of the lines used to draw the features.
    **Largura da Linha:** A espessura das linhas usadas para desenhar os recursos.

## Example
## Exemplo

Here's an example GeoJSON input:
Aqui está um exemplo de entrada GeoJSON:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [[[-122.4194, 37.7749], [-122.4194, 37.7749], [-122.4194, 37.7749]]]
      },
      "properties": {
        "name": "Golden Gate Park"
      }
    }
  ]
}
```

This GeoJSON represents a single polygon feature. The tool will convert this data into an SVG representation of the park's boundary.
Este GeoJSON representa um único recurso de polígono. A ferramenta converterá esses dados em uma representação SVG da fronteira do parque.

## Troubleshooting
## Solução de problemas

*   **Invalid GeoJSON:** Ensure that your GeoJSON data is valid.  Use a GeoJSON validator to check for errors.
    **GeoJSON Inválido:** Certifique-se de que seus dados GeoJSON são válidos. Use um validador GeoJSON para verificar se há erros.
*   **Large Files:** Converting very large GeoJSON files may take a long time or result in an error.  Consider simplifying your data or splitting it into smaller files.
    **Arquivos Grandes:** A conversão de arquivos GeoJSON muito grandes pode demorar muito ou resultar em um erro. Considere simplificar seus dados ou dividi-los em arquivos menores.
*   **SVG Rendering Issues:** If the generated SVG is not rendering correctly in your browser, try updating your browser to the latest version or using a different browser.
    **Problemas de Renderização SVG:** Se o SVG gerado não estiver sendo renderizado corretamente no seu navegador, tente atualizar seu navegador para a versão mais recente ou usar um navegador diferente.

---
