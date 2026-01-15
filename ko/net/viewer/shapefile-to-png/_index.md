---
title: Shapefile을 PNG로 변환하기
linkTitle: 셰이프파일을 PNG로 변환하기
weight: 10
description: 셰이프 파일을 이미지(PNG) 형식으로 변환하는 방법을 설명합니다.
url: /ko/net/viewer/shapefile-to-png/
---

## 소개

이 문서에서는 .NET 기반 뷰어를 사용하여 셰이프 파일(.shp)을 PNG 이미지로 변환하는 단계를 안내합니다. 이 프로세스는 지리 공간 데이터를 시각적 형식으로 공유하거나 분석하기 위해 필요할 수 있습니다.

## 전제 조건

*   .NET Framework 4.7.2 이상이 설치되어 있어야 합니다.
*   NetViewer 라이브러리가 프로젝트에 참조되어야 합니다. (다운로드 링크: [https://github.com/GIS-PRODUCTS/netviewer](https://github.com/GIS-PRODUCTS/netviewer))
*   셰이프 파일(.shp)이 준비되어 있어야 합니다.

## 단계

1.  **프로젝트 설정:** Visual Studio 또는 원하는 .NET 개발 환경에서 새 콘솔 애플리케이션 프로젝트를 만듭니다.
2.  **NetViewer 참조 추가:** NetViewer 라이브러리를 프로젝트에 참조합니다. NuGet 패키지 관리자를 사용하거나 DLL 파일을 직접 참조할 수 있습니다.
3.  **코드 작성:** 다음 코드를 사용하여 셰이프 파일을 PNG 이미지로 변환합니다.

```csharp
// 필요한 네임스페이스를 가져옵니다.
using NetViewer;
using System;
using System.Drawing;
using System.IO;

public class ShapefileToPngConverter
{
    public static void Main(string[] args)
    {
        // 셰이프 파일 경로 및 출력 PNG 파일 경로를 지정합니다.
        string shapefilePath = "path/to/your/shapefile.shp"; // 실제 셰이프파일 경로로 변경하세요.
        string outputPngPath = "path/to/output/image.png"; // 실제 출력 이미지 경로로 변경하세요.

        try
        {
            // ShapefileReader를 사용하여 셰이프 파일을 읽습니다.
            using (ShapefileReader reader = new ShapefileReader(shapefilePath))
            {
                // 첫 번째 피처를 가져옵니다.
                var feature = reader.GetFeature(0);

                // 피처의 형상(geometry)을 가져옵니다.
                Geometry geometry = feature.Geometry;

                // 이미지 크기를 설정합니다.
                int width = 512;
                int height = 512;

                // Bitmap 객체를 생성합니다.
                Bitmap bitmap = new Bitmap(width, height);

                // Graphics 객체를 사용하여 이미지를 그립니다.
                using (Graphics g = Graphics.FromImage(bitmap))
                {
                    // 이미지 배경을 흰색으로 설정합니다.
                    g.Clear("White");

                    // 형상을 이미지에 렌더링합니다.
                    geometry.Render(g, new Rectangle(0, 0, width, height));
                }

                // 이미지를 PNG 파일로 저장합니다.
                bitmap.Save(outputPngPath, System.Drawing.Imaging.ImageFormat.Png);

                Console.WriteLine($"셰이프 파일을 성공적으로 PNG 이미지로 변환했습니다: {outputPngPath}");
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine($"오류 발생: {ex.Message}");
        }

        Console.ReadKey();
    }
}
```

4.  **코드 설명:**
    *   `shapefilePath`: 변환할 셰이프 파일의 경로를 지정합니다.
    *   `outputPngPath`: 생성된 PNG 이미지 파일을 저장할 경로를 지정합니다.
    *   `ShapefileReader`: 셰이프 파일을 읽기 위한 클래스입니다.
    *   `Geometry`: 셰이프 파일의 형상 데이터를 나타내는 클래스입니다.
    *   `Render()`: 형상을 이미지에 그리는 메서드입니다.
5.  **실행:** 코드를 컴파일하고 실행합니다. 지정된 출력 경로에 PNG 이미지가 생성됩니다.

## 문제 해결

*   **NetViewer 라이브러리 누락:** NetViewer 라이브러리가 프로젝트에 올바르게 참조되었는지 확인합니다.
*   **셰이프 파일 경로 오류:** `shapefilePath` 변수가 셰이프 파일의 정확한 경로를 가리키는지 확인합니다.
*   **출력 경로 권한 문제:** 출력 PNG 파일을 저장할 디렉토리에 쓰기 권한이 있는지 확인합니다.
*   **형상 데이터 오류:** 셰이프 파일에 유효하지 않은 형상 데이터가 포함되어 있으면 변환 프로세스가 실패할 수 있습니다.

## 추가 정보

*   NetViewer 라이브러리: [https://github.com/GIS-PRODUCTS/netviewer](https://github.com/GIS-PRODUCTS/netviewer)
*   셰이프 파일 형식: [https://en.wikipedia.org/wiki/Shapefile](https://en.wikipedia.org/wiki/Shapefile)

---
