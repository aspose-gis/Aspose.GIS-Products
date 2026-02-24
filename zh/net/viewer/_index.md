---
title: NetViewer
date: 2023-11-27T14:58:36+09:00
draft: false
url: /zh/net/viewer/
weight: 10
aliases: [Net Viewer]
tags: [GIS, viewer, net]
---

## Overview ##

<p>NetViewer is a web-based GIS viewer that allows users to view and interact with geospatial data.</p>

## Features ##

*   View various types of geospatial data, including vector, raster, and WMS layers.
*   Perform basic map navigation and querying operations.
*   Customize the appearance of the map by changing colors, fonts, and labels.
*   Export maps to common image formats.
*   Support for multiple languages.

## Installation ##

<p>NetViewer is a web application and can be deployed on any standard web server.</p>

### Prerequisites ###

*   Web server (e.g., Apache, Nginx)
*   PHP 7.4 or higher
*   GD library

### Deployment ###

1.  Copy the NetViewer files to the web server's document root.
2.  Configure the web server to serve PHP files.
3.  Set the appropriate file permissions.
4.  Access NetViewer through a web browser.

## Configuration ##

<p>NetViewer can be configured using a configuration file.</p>

### Configuration File Format ###

The configuration file is in JSON format. Here's an example:

```json
{
  "map": {
    "center": [126.978, 37.566],
    "zoom": 13,
    "layers": [
      {
        "name": "OpenStreetMap",
        "url": "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
        "attribution": "© OpenStreetMap contributors"
      }
    ]
  },
  "language": "en"
}
```

### Configuration Options ###

*   `map.center`: The initial center of the map.
*   `map.zoom`: The initial zoom level of the map.
*   `map.layers`: An array of layers to display on the map.
    *   `name`: The name of the layer.
    *   `url`: The URL of the tile server.
    *   `attribution`: The attribution for the layer.
*   `language`: The default language for the user interface.

## Usage ##

<p>Once NetViewer is installed and configured, users can access it through a web browser.</p>

### Basic Navigation ###

*   Use the mouse wheel to zoom in and out.
*   Click and drag the map to pan.
*   Use the navigation buttons to move around the map.

### Querying Data ###

*   Click on features to view their attributes.
*   Use the search bar to find specific locations or features.

## Troubleshooting ##

<p>If you encounter any problems with NetViewer, please refer to the troubleshooting section below.</p>

### Common Issues ###

*   **Map not loading:** Check your web server configuration and make sure that PHP is enabled.
*   **Layer not displaying:** Verify that the layer URL is correct and that the tile server is accessible.
*   **Language not changing:** Make sure that the language setting in the configuration file is valid.

## Support ##

<p>If you need help with NetViewer, please contact us at <a href="mailto:support@example.com">support@example.com</a>.</p>

---
标题：NetViewer
日期：2023-11-27T14:58:36+09:00
草稿：false
url: /zh/net/viewer/
权重：10
别名：[Net Viewer]
标签：[GIS, viewer, net]
---

## 概述 ##

<p>NetViewer 是一个基于 Web 的 GIS 查看器，允许用户查看和交互地理空间数据。</p>

## 特性 ##

*   查看各种类型的地理空间数据，包括矢量、栅格和 WMS 图层。
*   执行基本的地图导航和查询操作。
*   通过更改颜色、字体和标签来自定义地图的外观。
*   将地图导出为常见的图像格式。
*   支持多种语言。

## 安装 ##

<p>NetViewer 是一个 Web 应用程序，可以部署在任何标准的 Web 服务器上。</p>

### 先决条件 ###

*   Web 服务器（例如 Apache、Nginx）
*   PHP 7.4 或更高版本
*   GD 库

### 部署 ###

1.  将 NetViewer 文件复制到 Web 服务器的文档根目录。
2.  配置 Web 服务器以提供 PHP 文件。
3.  设置适当的文件权限。
4.  通过 Web 浏览器访问 NetViewer。

## 配置 ##

<p>可以使用配置文件来配置 NetViewer。</p>

### 配置文件格式 ###

配置文件采用 JSON 格式。以下是一个示例：

```json
{
  "map": {
    "center": [126.978, 37.566],
    "zoom": 13,
    "layers": [
      {
        "name": "OpenStreetMap",
        "url": "https://tile.openstreetmap.org/{z}/{x}/{y}.png",
        "attribution": "© OpenStreetMap contributors"
      }
    ]
  },
  "language": "en"
}
```

### 配置选项 ###

*   `map.center`: 地图的初始中心点。
*   `map.zoom`: 地图的初始缩放级别。
*   `map.layers`: 要在地图上显示的图层数组。
    *   `name`: 图层的名称。
    *   `url`: 平铺服务器的 URL。
    *   `attribution`: 图层的署名信息。
*   `language`: 用户界面的默认语言。

## 用法 ##

<p>安装并配置 NetViewer 后，用户可以通过 Web 浏览器访问它。</p>

### 基本导航 ###

*   使用鼠标滚轮缩放。
*   单击并拖动地图以平移。
*   使用导航按钮在地图上移动。

### 查询数据 ###

*   单击要素以查看其属性。
*   使用搜索栏查找特定位置或要素。

## 故障排除 ##

<p>如果在 NetViewer 中遇到任何问题，请参阅以下故障排除部分。</p>

### 常见问题 ###

*   **地图未加载：**检查您的 Web 服务器配置并确保已启用 PHP。
*   **图层未显示：**验证图层 URL 是否正确以及平铺服务器是否可访问。
*   **语言未更改：**确保配置文件中的语言设置有效。

## 支持 ##

<p>如果您需要 NetViewer 的帮助，请通过 <a href="mailto:support@example.com">support@example.com</a> 联系我们。</p>

---
