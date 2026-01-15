---
title: OSM을 SVG로 변환하기
linkTitle: OSM을 SVG로 변환하기
weight: 10
description: OpenStreetMap 데이터를 SVG 형식으로 변환하는 방법에 대한 설명입니다.
url: /ko/net/viewer/osm-to-svg/
aliases: [osm-to-svg]
---

## 개요

이 도구는 OpenStreetMap (OSM) 데이터를 SVG (Scalable Vector Graphics) 형식으로 변환합니다.  SVG는 웹 브라우저에서 쉽게 표시하고 조작할 수 있는 벡터 이미지 형식입니다. 이 도구를 사용하면 OSM 데이터를 지도, 다이어그램 또는 기타 시각적 표현으로 만들 수 있습니다.

## 기능

*   OSM 데이터 다운로드 및 처리
*   다양한 필터링 옵션 (예: 특정 태그 기반)
*   SVG 출력 파일 생성
*   사용자 정의 가능한 스타일 (예: 도로, 건물, 지형)
*   배경 이미지 오버레이 지원

## 사용법

1.  **OSM 데이터 다운로드:** 먼저 변환하려는 지역의 OSM 데이터를 다운로드해야 합니다. [Overpass API](https://overpass-api.org/) 또는 기타 OSM 데이터 제공자를 사용할 수 있습니다.
2.  **데이터 준비:** 다운로드한 OSM 데이터를 도구에서 처리할 수 있는 형식으로 준비합니다. 일반적으로 `.osm` 또는 `.pbf` 형식을 사용합니다.
3.  **변환 실행:** 도구를 실행하고 입력 파일 및 출력 파일 이름을 지정합니다. 필요한 경우 필터링 옵션 및 스타일을 구성합니다.
4.  **SVG 파일 확인:** 변환이 완료되면 생성된 SVG 파일을 열고 결과를 확인합니다.

## 예제

다음은 간단한 명령줄 예제입니다.

```bash
osm-to-svg -i input.osm -o output.svg -t highway,building
```

이 명령은 `input.osm` 파일에서 고속도로 및 건물을 추출하여 `output.svg` 파일로 변환합니다.

## 고급 옵션

*   `-f`: 필터링 규칙을 지정합니다 (예: `highway=residential`).
*   `-s`: 스타일 파일을 지정합니다.
*   `-b`: 배경 이미지 URL을 지정합니다.
*   `-l`: 지도 투영법을 설정합니다.
*   `-z`: 확대/축소 레벨을 설정합니다.

## 문제 해결

*   **오류 메시지:** 오류 메시지를 주의 깊게 읽고 문제를 해결하십시오.
*   **데이터 형식:** 입력 데이터 형식이 올바른지 확인하십시오.
*   **필터링 규칙:** 필터링 규칙이 예상대로 작동하는지 확인하십시오.
*   **스타일 파일:** 스타일 파일에 유효한 SVG 스타일 정의가 포함되어 있는지 확인하십시오.

## 추가 정보

*   [OpenStreetMap](https://www.openstreetmap.org/)
*   [Scalable Vector Graphics (SVG)](https://www.w3.org/Graphics/SVG/)
*   [Overpass API](https://overpass-api.org/)
---
