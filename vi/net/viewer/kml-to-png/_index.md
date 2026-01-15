---
title: KML to PNG Conversion
linkTitle: Chuyển đổi KML sang PNG
weight: 10
url: /vi/net/viewer/kml-to-png/
aliases: [KML to PNG, KML2PNG]
description: Convert KML files to PNG images.
---

## Overview
## Tổng quan

This tool converts KML (Keyhole Markup Language) files into PNG image format. It allows you to visualize geographical data represented in KML as a static image.

Công cụ này chuyển đổi các tệp KML (Ngôn ngữ đánh dấu Keyhole) thành định dạng hình ảnh PNG. Nó cho phép bạn trực quan hóa dữ liệu địa lý được biểu diễn trong KML dưới dạng hình ảnh tĩnh.

## Features
## Tính năng

*   **KML to PNG Conversion:** Converts KML files into PNG images. Chuyển đổi các tệp KML thành hình ảnh PNG.
*   **Customizable Output:** Allows customization of the output image, including size and resolution. Cho phép tùy chỉnh hình ảnh đầu ra, bao gồm kích thước và độ phân giải.
*   **Easy to Use:** Simple and intuitive interface for easy conversion. Giao diện đơn giản và trực quan để chuyển đổi dễ dàng.
*   **Batch Conversion:** Supports batch conversion of multiple KML files. Hỗ trợ chuyển đổi hàng loạt nhiều tệp KML.

## Usage
## Cách sử dụng

1.  **Input KML File:** Select the KML file you want to convert. Chọn tệp KML bạn muốn chuyển đổi.
2.  **Configure Output Settings:** Adjust the output image settings, such as size and resolution. Điều chỉnh cài đặt hình ảnh đầu ra, chẳng hạn như kích thước và độ phân giải.
3.  **Convert:** Click the "Convert" button to generate the PNG image. Nhấp vào nút "Chuyển đổi" để tạo hình ảnh PNG.
4.  **Download:** Download the generated PNG image. Tải xuống hình ảnh PNG đã tạo.

## Parameters
## Tham số

*   `input`: Path to the input KML file. Đường dẫn đến tệp KML đầu vào.
*   `output`: Path to save the output PNG image. Đường dẫn để lưu hình ảnh PNG đầu ra.
*   `width`: Width of the output image in pixels. Chiều rộng của hình ảnh đầu ra theo pixel.
*   `height`: Height of the output image in pixels. Chiều cao của hình ảnh đầu ra theo pixel.
*   `scale`: Scale factor for the KML data. Hệ số tỷ lệ cho dữ liệu KML.

## Example
## Ví dụ

```bash
kml-to-png --input my_map.kml --output output.png --width 1024 --height 768 --scale 2.0
# Chuyển đổi tệp KML "my_map.kml" thành hình ảnh PNG có tên "output.png", với chiều rộng là 1024 pixel, chiều cao là 768 pixel và hệ số tỷ lệ là 2.0.
```

## Troubleshooting
## Khắc phục sự cố

*   **Invalid KML File:** Ensure the input file is a valid KML file. Đảm bảo tệp đầu vào là một tệp KML hợp lệ.
*   **Insufficient Permissions:** Make sure you have write permissions to the output directory. Đảm bảo bạn có quyền ghi vào thư mục đầu ra.
*   **Memory Issues:** For large KML files, increase the available memory or reduce the image size. Đối với các tệp KML lớn, hãy tăng bộ nhớ khả dụng hoặc giảm kích thước hình ảnh.

---
