---
title: Chuyển đổi SHP sang PNG
url: /vi/net/viewer/shp-to-png/
weight: 10
layout: single
draft: false
toc: true
---

## Giới thiệu

Công cụ này cho phép bạn chuyển đổi các tệp Shapefile (.shp) thành hình ảnh .png. Nó rất hữu ích để tạo bản đồ hoặc hình ảnh trực quan từ dữ liệu không gian của bạn.

## Yêu cầu

*   .NET Framework 4.7.2 trở lên
*   Thư viện GeoSharp (được cài đặt thông qua NuGet)

## Cài đặt

1.  Tạo một dự án .NET mới.
2.  Cài đặt thư viện GeoSharp bằng trình quản lý gói NuGet.

    ```csharp
    Install-Package GeoSharp
    ```
3.  Sao chép mã nguồn được cung cấp vào dự án của bạn.

## Sử dụng

1.  Thay đổi đường dẫn đến tệp Shapefile (.shp) và thư mục đầu ra mong muốn.
2.  Chạy ứng dụng. Nó sẽ chuyển đổi tất cả các tệp .shp trong thư mục đầu vào thành hình ảnh .png và lưu chúng vào thư mục đầu ra.

## Mã nguồn

```csharp
using System;
using System.IO;
using GeoSharp;
using NetTopologySuite.Features;

namespace ShpToPngConverter
{
    class Program
    {
        static void Main(string[] args)
        {
            // Thay đổi các đường dẫn này thành đường dẫn thực tế của bạn
            string inputShapefileDirectory = "C:\\path\\to\\shapefiles";
            string outputPngDirectory = "C:\\path\\to\\output\\pngs";

            // Đảm bảo thư mục đầu ra tồn tại
            if (!Directory.Exists(outputPngDirectory))
            {
                Directory.CreateDirectory(outputPngDirectory);
            }

            // Lặp qua tất cả các tệp shapefile trong thư mục đầu vào
            foreach (string shapefilePath in Directory.GetFiles(inputShapefileDirectory, "*.shp"))
            {
                try
                {
                    // Tải shapefile
                    var shapefile = Shapefile.Open(shapefilePath);

                    // Lặp qua tất cả các đặc điểm trong shapefile
                    foreach (IFeature feature in shapefile.Features)
                    {
                        // Tạo tên tệp đầu ra
                        string outputPngPath = Path.Combine(outputPngDirectory, $"{feature.GetRecordId()}.png");

                        // Vẽ đặc điểm vào hình ảnh
                        var image = feature.Render(256, 256);

                        // Lưu hình ảnh thành tệp .png
                        image.Save(outputPngPath);
                    }
                }
                catch (Exception ex)
                {
                    Console.WriteLine($"Lỗi khi xử lý {shapefilePath}: {ex.Message}");
                }
            }

            Console.WriteLine("Hoàn tất!");
        }
    }
}
```

## Các tùy chọn bổ sung

*   Bạn có thể điều chỉnh kích thước hình ảnh bằng cách thay đổi các tham số trong phương thức `Render`.
*   Bạn có thể thêm các lớp hoặc chú thích khác vào hình ảnh.
*   Bạn có thể sử dụng thư viện GeoSharp để thực hiện các thao tác không gian khác trên dữ liệu của bạn.

## Khắc phục sự cố

Nếu bạn gặp bất kỳ vấn đề nào, hãy đảm bảo rằng bạn đã cài đặt tất cả các yêu cầu và rằng đường dẫn đến tệp Shapefile và thư mục đầu ra là chính xác. Bạn cũng có thể thử khởi động lại máy tính của mình.
---
