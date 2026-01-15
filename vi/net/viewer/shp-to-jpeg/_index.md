---
title: Chuyển đổi SHP sang JPEG
url: /vi/net/viewer/shp-to-jpeg/
weight: 10
layout: single
draft: false
toc: true
---

## Giới thiệu

Công cụ này cho phép bạn chuyển đổi các tệp SHP (Shapefile) thành hình ảnh JPEG. Nó đặc biệt hữu ích để tạo bản xem trước nhanh hoặc hình ảnh nhỏ của dữ liệu không gian địa lý.

## Yêu cầu

*   [NetViewer](https://github.com/GIS-SOFTWARE/netviewer)
*   Các thư viện .NET phù hợp (thường được bao gồm trong NetViewer)

## Cài đặt

1.  Đảm bảo bạn đã cài đặt [NetViewer](https://github.com/GIS-SOFTWARE/netviewer).
2.  Không cần cài đặt bổ sung cho chức năng chuyển đổi SHP sang JPEG, vì nó là một phần của NetViewer.

## Cách sử dụng

Công cụ này có thể được sử dụng thông qua dòng lệnh hoặc tích hợp vào ứng dụng .NET của riêng bạn.

### Dòng lệnh

```
shp2jpeg.exe -i input.shp -o output.jpg -s 100
```

*   `-i`: Chỉ định tệp SHP đầu vào.
*   `-o`: Chỉ định tệp JPEG đầu ra.
*   `-s`: Chỉ định độ phân giải (tỷ lệ phần trăm).  Giá trị mặc định là 100.

Ví dụ: để chuyển đổi `my_shapefile.shp` thành `output.jpg` với độ phân giải 50%:

```
shp2jpeg.exe -i my_shapefile.shp -o output.jpg -s 50
```

### Trong ứng dụng .NET

Bạn có thể sử dụng các lớp và phương thức trong NetViewer để tích hợp chức năng chuyển đổi SHP sang JPEG vào ứng dụng của bạn.  Tham khảo tài liệu NetViewer cho hướng dẫn chi tiết về cách thực hiện việc này.

## Tùy chọn nâng cao

*   **Chọn thuộc tính:** Bạn có thể chỉ định các thuộc tính cụ thể từ tệp SHP để sử dụng trong quá trình chuyển đổi.
*   **Phong cách hóa:**  Bạn có thể áp dụng các kiểu dáng khác nhau cho các đối tượng hình học trong tệp SHP trước khi chuyển đổi chúng thành JPEG.
*   **Hệ tọa độ:** Đảm bảo rằng hệ tọa độ của tệp SHP được xác định chính xác để đảm bảo kết quả chính xác.

## Khắc phục sự cố

*   **Lỗi không tìm thấy tệp:**  Đảm bảo rằng đường dẫn đến tệp SHP đầu vào là chính xác.
*   **Lỗi định dạng tệp không hợp lệ:** Đảm bảo rằng tệp SHP là một tệp Shapefile hợp lệ.
*   **Kết quả không mong muốn:** Thử nghiệm với các tùy chọn khác nhau, chẳng hạn như độ phân giải và kiểu dáng, để đạt được kết quả mong muốn.

## Hỗ trợ

Nếu bạn gặp bất kỳ vấn đề nào hoặc có câu hỏi, vui lòng tham khảo [NetViewer GitHub](https://github.com/GIS-SOFTWARE/netviewer) để biết thêm thông tin và hỗ trợ.
---
