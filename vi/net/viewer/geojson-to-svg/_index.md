---
title: Chuyển đổi GeoJSON sang SVG
url: /vi/net/viewer/geojson-to-svg/
weight: 10
layout: "default"
description: Công cụ chuyển đổi trực tuyến từ GeoJSON sang SVG.
---

## Giới thiệu

Công cụ này cho phép bạn chuyển đổi dữ liệu GeoJSON thành định dạng SVG (Scalable Vector Graphics).  SVG là một định dạng đồ họa vector dựa trên XML, rất phù hợp để hiển thị bản đồ và các đối tượng địa lý khác trên web vì nó có thể mở rộng mà không làm giảm chất lượng.

## Cách sử dụng

1.  **Nhập GeoJSON:** Bạn có thể nhập dữ liệu GeoJSON bằng cách:
    *   Dán trực tiếp vào hộp văn bản.
    *   Tải lên một tệp `.geojson`.
    *   Nhập từ URL.
2.  **Điều chỉnh cài đặt (tùy chọn):**  Bạn có thể điều chỉnh các cài đặt như màu sắc, độ dày đường viền và kiểu đổ bóng để tùy chỉnh giao diện của SVG được tạo ra.
3.  **Tạo SVG:** Nhấp vào nút "Tạo SVG" để bắt đầu quá trình chuyển đổi.
4.  **Tải xuống SVG:** Sau khi quá trình chuyển đổi hoàn tất, bạn có thể tải xuống tệp SVG đã tạo.

## Ví dụ GeoJSON

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "geometry": {
        "type": "Polygon",
        "coordinates": [[
          [ -122.4194, 37.7749 ],
          [ -122.4194, 37.7833 ],
          [ -122.4052, 37.7833 ],
          [ -122.4052, 37.7749 ],
          [ -122.4194, 37.7749 ]
        ]]
      },
      "properties": {
        "name": "San Francisco"
      }
    }
  ]
}
```

## Các tùy chọn nâng cao

*   **Đơn giản hóa:** Giảm số lượng điểm trong hình dạng để tạo ra các tệp SVG nhỏ hơn.
*   **Phong cách:** Sử dụng CSS để kiểm soát giao diện của các đối tượng SVG.
*   **Tích hợp bản đồ:**  Kết hợp SVG với thư viện bản đồ như Leaflet hoặc Mapbox GL JS để tạo ra các ứng dụng bản đồ tương tác.

## Hỗ trợ định dạng

Công cụ này hỗ trợ tất cả các loại GeoJSON, bao gồm:

*   Feature
*   FeatureCollection
*   GeometryCollection
*   LineString
*   MultiLineString
*   Point
*   MultiPoint
*   Polygon
*   MultiPolygon

## Ghi chú

*   Các tệp GeoJSON rất lớn có thể mất nhiều thời gian để chuyển đổi.
*   Đảm bảo rằng dữ liệu GeoJSON của bạn hợp lệ trước khi sử dụng công cụ này.  Bạn có thể sử dụng trình xác thực GeoJSON trực tuyến để kiểm tra tính hợp lệ của dữ liệu của mình.
*   Công cụ này được cung cấp như là một dịch vụ miễn phí và không đảm bảo khả năng sẵn sàng hoặc độ chính xác.

---
