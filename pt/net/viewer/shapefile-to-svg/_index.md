---
title: Converter Shapefile para SVG
linkTitle: Converter Shapefile para SVG
weight: 10
url: /pt/net/viewer/shapefile-to-svg/
description: Converta arquivos shapefile em vetores SVG editáveis usando o Visualizador de Shapefile da .NET.
---

## Converter Shapefile para SVG com o Visualizador de Shapefile da .NET

O Visualizador de Shapefile da .NET permite converter arquivos shapefile em imagens SVG (Scalable Vector Graphics) editáveis. Esta funcionalidade é útil para criar gráficos vetoriais a partir de dados geoespaciais, que podem ser ampliados e modificados sem perda de qualidade.

### Requisitos

*   Visualizador de Shapefile da .NET instalado
*   Arquivo shapefile válido

### Passos

1.  **Carregue o arquivo shapefile:** Utilize a classe `Shapefile` para carregar o arquivo shapefile.
2.  **Configure as opções de conversão SVG:** Defina as propriedades desejadas para a saída SVG, como tamanho da página, cor de fundo e estilo das linhas.
3.  **Converta o shapefile para SVG:** Chame o método `GenerateSVG` para criar o arquivo SVG.

### Exemplo de código

```csharp
// Carrega o arquivo shapefile
Shapefile shapefile = new Shapefile("path/to/your/shapefile.shp");

// Configura as opções de conversão SVG
SvgOptions svgOptions = new SvgOptions();
svgOptions.PageWidth = 8.5 * 25.4; // Largura da página em polegadas (convertido para milímetros)
svgOptions.PageHeight = 11 * 25.4; // Altura da página em polegadas (convertido para milímetros)
svgOptions.BackgroundColor = Color.White; // Cor de fundo branco

// Converte o shapefile para SVG
string svgFilePath = "path/to/your/output.svg";
shapefile.GenerateSVG(svgFilePath, svgOptions);
```

### Opções de conversão

O método `GenerateSVG` aceita um objeto `SvgOptions` que permite personalizar a saída SVG. Algumas das opções disponíveis incluem:

*   `PageWidth`: Largura da página em milímetros.
*   `PageHeight`: Altura da página em milímetros.
*   `BackgroundColor`: Cor de fundo do SVG.
*   `LineColor`: Cor das linhas no SVG.
*   `LineWidth`: Espessura das linhas no SVG.
*   `FillColor`: Cor de preenchimento dos polígonos no SVG.

### Considerações

*   A conversão de arquivos shapefile complexos pode levar algum tempo.
*   O tamanho do arquivo SVG resultante dependerá da complexidade do shapefile e das opções de conversão escolhidas.
*   Certifique-se de que o arquivo shapefile não esteja corrompido antes de tentar convertê-lo.

### Solução de problemas

Se você encontrar algum problema durante a conversão, verifique os seguintes pontos:

*   O caminho do arquivo shapefile está correto?
*   Você tem permissão para acessar o arquivo shapefile?
*   As opções de conversão SVG são válidas?
*   O Visualizador de Shapefile da .NET está instalado corretamente?

Para obter mais informações e suporte, consulte a documentação do Visualizador de Shapefile da .NET.
---
