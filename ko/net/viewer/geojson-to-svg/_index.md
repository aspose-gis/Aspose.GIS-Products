---
title: GeoJSON을 SVG로 변환하기
linkTitle: GeoJSON을 SVG로 변환하기
weight: 10
description: GeoJSON 데이터를 SVG 형식으로 변환하는 방법을 설명합니다.
url: /ko/net/viewer/geojson-to-svg/
aliases: [geojson to svg, geojson svg conversion]
---

## 소개

이 도구는 GeoJSON 데이터를 SVG 형식으로 변환합니다.  SVG(Scalable Vector Graphics)는 벡터 이미지 형식이므로 이미지를 확대해도 품질 저하 없이 선명하게 표시됩니다. 이 기능을 사용하면 지도 데이터와 같은 지리 공간 정보를 웹 페이지나 다른 응용 프로그램에 쉽게 통합할 수 있습니다.

## 사용법

1.  GeoJSON 파일을 준비합니다.
2.  변환 도구를 사용하여 GeoJSON 데이터를 SVG 형식으로 변환합니다.
3.  SVG 파일을 웹 페이지 또는 다른 응용 프로그램에 삽입합니다.

## 예제

다음은 GeoJSON 데이터를 SVG로 변환하는 간단한 예제입니다.

```json
[
  {
    "type": "Feature",
    "geometry": {
      "type": "Point",
      "coordinates": [127.0, 37.5]
    },
    "properties": {
      "name": "서울"
    }
  }
]
```

위의 GeoJSON 데이터를 SVG로 변환하면 다음과 같은 SVG 코드가 생성됩니다.

```svg
<svg width="200" height="200">
  <circle cx="100" cy="100" r="50" fill="red" />
  <text x="100" y="110" text-anchor="middle" font-size="16">서울</text>
</svg>
```

## 추가 정보

*   GeoJSON 형식에 대한 자세한 내용은 [GeoJSON 공식 웹사이트](https://geojson.org/)를 참조하십시오.
*   SVG 형식에 대한 자세한 내용은 [W3C SVG 명세](https://www.w3.org/TR/svg11/)를 참조하십시오.

## 문제 해결

변환 과정에서 문제가 발생하면 다음 사항을 확인하십시오.

*   GeoJSON 파일이 유효한 형식을 따르는지 확인합니다.
*   변환 도구가 올바르게 설치 및 구성되었는지 확인합니다.
*   SVG 파일을 지원하는 브라우저 또는 응용 프로그램을 사용하고 있는지 확인합니다.

