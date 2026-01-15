---
title: Conversor OSM para JPEG
linkTitle: Conversor OSM para JPEG
weight: 10
description: Converta dados OpenStreetMap em imagens JPEG.
url: /pt/viewer/osm-to-jpeg/
aliases: [osm2jpg, osm-to-jpeg]
---

## Visão geral

Este guia explica como usar o conversor OSM para JPEG para gerar imagens a partir de dados OpenStreetMap (OSM).

## Requisitos

*   [Netlabel Viewer](https://netlabel.github.io/viewer/) instalado
*   Dados OpenStreetMap (arquivo .osm ou URL)

## Uso

O conversor é executado como um comando na linha de comando:

```bash
./net-viewer osm-to-jpeg --input <arquivo OSM ou URL> --output <arquivo JPEG> [opções]
```

### Opções

*   `--input`: O arquivo OSM de entrada ou a URL para baixar. Obrigatório.
*   `--output`: O arquivo JPEG de saída. Obrigatório.
*   `--width`: A largura da imagem em pixels. Padrão: 1024.
*   `--height`: A altura da imagem em pixels. Padrão: 1024.
*   `--scale`: Fator de escala para os dados OSM. Padrão: 1.0.
*   `--attribution`: Texto do atributo a ser incluído na imagem. Padrão: "Dados © OpenStreetMap".
*   `--verbose`: Exibe informações detalhadas durante o processamento.

## Exemplos

### Converter um arquivo OSM para JPEG

```bash
./net-viewer osm-to-jpeg --input planet.osm --output world.jpg --width 2048 --height 2048
```

Este comando converte o arquivo `planet.osm` em uma imagem JPEG chamada `world.jpg` com largura e altura de 2048 pixels.

### Converter um URL OSM para JPEG

```bash
./net-viewer osm-to-jpeg --input https://download.geofabrik.de/europe/germany.osm --output germany.jpg
```

Este comando baixa os dados OSM da URL fornecida e converte em uma imagem JPEG chamada `germany.jpg`.

### Converter um arquivo OSM para JPEG com atributo personalizado

```bash
./net-viewer osm-to-jpeg --input my_data.osm --output custom.jpg --attribution "Mapa © Minha Organização"
```

Este comando converte o arquivo `my_data.osm` em uma imagem JPEG chamada `custom.jpg` e inclui um atributo personalizado na imagem.

## Solução de problemas

*   **Erro: Arquivo OSM inválido:** Verifique se o arquivo OSM está no formato correto e não está corrompido.
*   **Erro: Impossível baixar dados OSM:** Verifique se a URL do OSM está correta e acessível.
*   **Imagem muito grande ou pequena:** Ajuste as opções `--width` e `--height` para controlar o tamanho da imagem.
*   **Dados OSM não visíveis na imagem:** Ajuste a opção `--scale` para aumentar ou diminuir o zoom nos dados OSM.

## Notas adicionais

*   O conversor usa o [Mapnik](https://mapnik.org/) como renderizador de mapa. Certifique-se de que o Mapnik esteja instalado e configurado corretamente.
*   A qualidade da imagem depende da resolução dos dados OSM e das opções de renderização usadas.
*   Para obter melhores resultados, use dados OSM atualizados e experimente diferentes opções para encontrar as configurações ideais para suas necessidades.
---
