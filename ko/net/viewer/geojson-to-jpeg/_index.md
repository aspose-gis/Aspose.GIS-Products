---
title: GeoJSON을 JPEG로 변환하기
linkTitle: GeoJSON을 JPEG로
weight: 10
description: GeoJSON 데이터를 JPEG 이미지로 변환하는 방법을 설명합니다.
url: /ko/net/viewer/geojson-to-jpeg/
aliases: [geojson to jpeg, geojson2jpeg]
---

## 소개

이 도구는 GeoJSON 데이터를 JPEG 이미지로 변환합니다.  이를 통해 지리 공간 데이터를 시각적으로 표현하고 공유할 수 있습니다.

## 사용법

1.  GeoJSON 파일 준비: 변환하려는 GeoJSON 데이터가 포함된 파일을 준비합니다.
2.  변환 실행: 도구를 사용하여 GeoJSON 파일을 JPEG 이미지로 변환합니다.
3.  결과 확인: 생성된 JPEG 이미지를 확인하고 필요에 따라 조정합니다.

## 상세 설명

GeoJSON은 지리 공간 데이터를 JSON 형식으로 인코딩하는 표준 포맷입니다. 이 도구는 GeoJSON 데이터를 읽고, 해당 데이터를 기반으로 맵을 생성하고, 최종적으로 맵을 JPEG 이미지로 렌더링합니다.

### 입력 파일 형식

*   **형식:** GeoJSON
*   **확장자:** .geojson
*   **내용:** 유효한 GeoJSON 데이터 (점, 선, 다각형 등)

### 출력 파일 형식

*   **형식:** JPEG 이미지
*   **확장자:** .jpeg 또는 .jpg

## 옵션

다음은 변환 프로세스를 제어하는 데 사용할 수 있는 몇 가지 옵션입니다.

*   `--width`: 출력 이미지의 너비 (기본값: 800)
*   `--height`: 출력 이미지의 높이 (기본값: 600)
*   `--scale`: 지도 스케일 (기본값: 1.0)
*   `--projection`: 투영법 (예: Mercator, EPSG:4326) (기본값: Mercator)
*   `--output`: 출력 파일 이름 (기본값: output.jpeg)

## 예제

다음은 도구를 사용하는 몇 가지 예제입니다.

1.  GeoJSON 파일을 기본 설정으로 JPEG로 변환:

    ```bash
    geojson-to-jpeg input.geojson
    ```

2.  출력 이미지의 너비와 높이를 지정하여 JPEG로 변환:

    ```bash
    geojson-to-jpeg --width 1024 --height 768 input.geojson
    ```

3.  특정 투영법을 사용하여 GeoJSON 파일을 JPEG로 변환:

    ```bash
    geojson-to-jpeg --projection EPSG:4326 input.geojson
    ```

## 문제 해결

*   **입력 파일이 유효하지 않음:** GeoJSON 파일의 형식이 올바른지 확인합니다.  유효성 검사기를 사용하여 파일을 확인할 수 있습니다.
*   **출력 이미지 품질 불량:** `--scale` 옵션을 조정하여 지도 스케일을 변경해 봅니다. 또한 `--width` 및 `--height` 옵션으로 출력 이미지의 해상도를 높여보세요.
*   **오류 메시지:** 오류 메시지를 주의 깊게 읽고 문제 해결을 위한 단서를 찾습니다.

## 추가 정보

*   GeoJSON 공식 웹사이트: [https://geojson.org/](https://geojson.org/)
*   투영법에 대한 자세한 내용은 관련 문서를 참조하십시오.
---
