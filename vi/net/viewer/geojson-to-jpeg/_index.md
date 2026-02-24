---
title: Chuyển đổi GeoJSON sang JPEG
url: /vi/net/viewer/geojson-to-jpeg/
weight: 10
layout: single
draft: false
toc: true
---

## Giới thiệu

Công cụ này cho phép bạn chuyển đổi dữ liệu GeoJSON thành hình ảnh JPEG. Bạn có thể sử dụng nó để tạo bản đồ tùy chỉnh, trực quan hóa dữ liệu địa không gian hoặc đơn giản là tạo ra các hình ảnh đẹp từ dữ liệu GeoJSON của mình.

## Yêu cầu

*   [NetViewer](https://github.com/netviewer-io/netviewer)
*   GeoJSON hợp lệ

## Hướng dẫn sử dụng

1.  Cung cấp tệp GeoJSON của bạn làm đầu vào.
2.  Chọn các tùy chọn hiển thị mong muốn, chẳng hạn như:
    *   Bóng nền
    *   Màu đường viền
    *   Độ dày đường viền
    *   Màu sắc
    *   Độ phân giải

3.  Nhấp vào nút "Chuyển đổi" để tạo hình ảnh JPEG.

## Ví dụ

Dưới đây là một ví dụ về cách sử dụng công cụ này:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [ -122.86, 37.39 ],
            [ -122.86, 37.40 ],
            [ -122.85, 37.40 ],
            [ -122.85, 37.39 ],
            [ -122.86, 37.39 ]
          ]
        ]
      },
      "properties": {
        "name": "Công viên Golden Gate"
      }
    }
  ]
}
```

Sử dụng tệp GeoJSON này làm đầu vào và chọn các tùy chọn hiển thị mong muốn, bạn có thể tạo một hình ảnh JPEG của Công viên Golden Gate.

## Mẹo & Thủ thuật

*   Để cải thiện chất lượng hình ảnh, hãy tăng độ phân giải.
*   Thử nghiệm với các màu sắc và độ dày đường viền khác nhau để tìm ra giao diện phù hợp nhất cho dữ liệu của bạn.
*   Sử dụng công cụ này để tạo bản đồ tùy chỉnh cho trang web hoặc ứng dụng của bạn.

## Khắc phục sự cố

Nếu bạn gặp bất kỳ vấn đề nào khi sử dụng công cụ này, vui lòng kiểm tra các điều sau:

*   Đảm bảo rằng tệp GeoJSON của bạn hợp lệ.
*   Đảm bảo rằng bạn đã cài đặt NetViewer.
*   Thử khởi động lại trình duyệt của bạn.

Nếu bạn vẫn gặp sự cố, vui lòng liên hệ với chúng tôi để được hỗ trợ.
---
