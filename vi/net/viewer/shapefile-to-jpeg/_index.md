---
title: Chuyển đổi Shapefile sang JPEG
url: /vi/net/viewer/shapefile-to-jpeg/
weight: 10
layout: single
draft: false
toc: true
---

## Giới thiệu

Công cụ chuyển đổi Shapefile sang JPEG cho phép bạn tạo hình ảnh JPEG từ các tệp shapefile. Điều này hữu ích để trực quan hóa dữ liệu không gian và tạo bản đồ tùy chỉnh.

## Yêu cầu

*   .NET Framework 4.7.2 hoặc cao hơn
*   Thư viện GeoSharp

## Cài đặt

1.  Tải xuống thư viện GeoSharp từ [NuGet](https://www.nuget.org/packages/GeoSharp/).
2.  Cài đặt thư viện vào dự án .NET của bạn.

## Sử dụng

```csharp
// Tạo một đối tượng ShapefileReader mới
ShapefileReader reader = new ShapefileReader("path/to/your/shapefile.shp");

// Lặp qua từng hình dạng trong shapefile
while (reader.Read())
{
    // Lấy hình dạng hiện tại
    Shape shape = reader.GetShape();

    // Tạo một đối tượng Rasterizer mới
    Rasterizer rasterizer = new Rasterizer(shape, extent, resolution);

    // Chuyển đổi hình dạng thành JPEG
    byte[] jpegData = rasterizer.ToJpeg();

    // Lưu JPEG vào tệp
    File.WriteAllBytes("path/to/your/output.jpeg", jpegData);
}

// Đóng ShapefileReader
reader.Close();
```

### Tham số

*   `shapefile`: Đường dẫn đến tệp shapefile.
*   `extent`: Phạm vi của hình dạng cần chuyển đổi.
*   `resolution`: Độ phân giải của hình ảnh JPEG đầu ra.

## Ví dụ

Để chuyển đổi một shapefile sang JPEG, bạn có thể sử dụng mã sau:

```csharp
using GeoSharp;
using System;
using System.IO;

namespace ShapefileToJpeg
{
    class Program
    {
        static void Main(string[] args)
        {
            // Thay thế bằng đường dẫn đến shapefile của bạn
            string shapefilePath = "path/to/your/shapefile.shp";

            // Xác định phạm vi và độ phân giải
            Extent extent = new Extent(-180, 180, -90, 90); // Phạm vi toàn cầu
            double resolution = 96; // Độ phân giải 96 DPI

            try
            {
                // Tạo một đối tượng ShapefileReader mới
                using (ShapefileReader reader = new ShapefileReader(shapefilePath))
                {
                    // Lặp qua từng hình dạng trong shapefile
                    while (reader.Read())
                    {
                        // Lấy hình dạng hiện tại
                        Shape shape = reader.GetShape();

                        // Tạo một đối tượng Rasterizer mới
                        using (Rasterizer rasterizer = new Rasterizer(shape, extent, resolution))
                        {
                            // Chuyển đổi hình dạng thành JPEG
                            byte[] jpegData = rasterizer.ToJpeg();

                            // Xác định đường dẫn tệp đầu ra
                            string outputFilePath = "path/to/your/output_" + shape.RecordNumber + ".jpeg";

                            // Lưu JPEG vào tệp
                            File.WriteAllBytes(outputFilePath, jpegData);

                            Console.WriteLine($"Đã tạo: {outputFilePath}");
                        }
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Lỗi: {ex.Message}");
            }

            Console.WriteLine("Hoàn tất!");
        }
    }
}
```

## Lựa chọn nâng cao

*   **Thay đổi màu sắc:** Bạn có thể thay đổi màu sắc của hình dạng bằng cách sử dụng các tùy chọn khác nhau trong lớp `Rasterizer`.
*   **Thêm chú thích:** Bạn có thể thêm chú thích vào hình ảnh JPEG bằng cách sử dụng các thư viện đồ họa.
*   **Tự động hóa quy trình:** Bạn có thể tự động hóa quy trình chuyển đổi shapefile sang JPEG bằng cách sử dụng một tập lệnh hoặc ứng dụng.

## Khắc phục sự cố

Nếu bạn gặp bất kỳ vấn đề nào khi sử dụng công cụ này, vui lòng tham khảo phần [câu hỏi thường gặp](https://www.example.com/faq).
---
