---
title: OpenStreetMap을 JPEG로 변환하기
linkTitle: OpenStreetMap을 JPEG로 변환하기
weight: 10
description: OpenStreetMap 데이터를 JPEG 이미지로 변환하는 방법을 설명합니다.
url: /ko/net/viewer/osm-to-jpeg/
aliases: [osm2jpg, osm to jpeg]
---

## 개요

이 도구는 OpenStreetMap (OSM) 데이터를 JPEG 이미지로 변환합니다.  지리 정보 시스템(GIS) 작업에 유용하며, 지도 시각화 및 분석을 위한 이미지를 생성하는 데 사용할 수 있습니다.

## 요구 사항

*   .NET 6.0 이상
*   OpenStreetMap 데이터 파일 (.osm 또는 .pbf)
*   JPEG 이미지 저장 공간

## 설치

1.  이 프로젝트를 복제합니다: `git clone [저장소 주소]`
2.  디렉토리로 이동합니다: `cd osm-to-jpeg`
3.  솔루션 파일을 엽니다 (.sln).
4.  솔루션을 빌드하고 게시합니다.

## 사용법

명령줄에서 다음 명령을 실행합니다:

```bash
./osm-to-jpeg --input <입력 OSM 파일> --output <출력 JPEG 파일> --zoom <확대 레벨> --width <이미지 너비> --height <이미지 높이>
```

*   `--input`: OpenStreetMap 데이터 파일의 경로입니다.
*   `--output`: 생성된 JPEG 이미지 파일의 경로입니다.
*   `--zoom`: 지도 확대 레벨입니다 (기본값: 10).
*   `--width`: 출력 이미지의 너비입니다 (기본값: 512).
*   `--height`: 출력 이미지의 높이입니다 (기본값: 512).

## 예제

다음 명령은 `seoul.osm` 파일을 사용하여 서울 지역을 JPEG 이미지로 변환하고, 확대 레벨을 12로 설정하며, 이미지 크기를 1024x768로 만듭니다:

```bash
./osm-to-jpeg --input seoul.osm --output seoul.jpg --zoom 12 --width 1024 --height 768
```

## 추가 옵션

*   `--format`: 출력 이미지 형식입니다 (JPEG, PNG 등). 기본값은 JPEG입니다.
*   `--color`: 색상 팔레트입니다.
*   `--attribution`: 지도 출처 표시 여부입니다.

## 문제 해결

*   **입력 파일이 유효하지 않습니다.** OpenStreetMap 데이터 파일의 형식이 올바른지 확인합니다.
*   **출력 파일을 만들 수 없습니다.** 출력 디렉토리에 쓰기 권한이 있는지 확인합니다.
*   **이미지가 너무 크거나 작습니다.** `--width` 및 `--height` 옵션을 조정하여 이미지 크기를 변경합니다.

## 기여

이 프로젝트에 대한 기여는 환영합니다! 버그를 보고하거나, 새로운 기능을 제안하거나, 코드를 직접 제출할 수 있습니다.
---
