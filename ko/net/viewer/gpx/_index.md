---
title: GPX 파일 형식
url: /ko/gpx/
weight: 10
description: GPX 파일 형식에 대한 정보입니다.
---

## GPX란 무엇인가요?

GPX(GPS Exchange Format)는 GPS 데이터 교환을 위한 XML 기반의 개방형 표준입니다. 지리적 위치, 경로, 웨이포인트 및 트랙과 같은 데이터를 저장하는 데 사용됩니다.

## GPX 파일의 용도

GPX 파일은 다음과 같은 다양한 용도로 사용됩니다.

*   GPS 장치 간의 데이터 교환
*   매핑 소프트웨어로의 데이터 가져오기 및 내보내기
*   온라인 매핑 서비스에 대한 트랙 업로드
*   여행 로그 기록

## GPX 파일 구조

GPX 파일은 XML 문서이며 다음과 같은 주요 요소를 포함합니다.

*   `gpx`: 루트 요소입니다.
*   `metadata`: GPX 파일에 대한 메타데이터를 포함합니다.
*   `tracks`: 하나 이상의 트랙을 포함합니다. 각 트랙은 일련의 웨이포인트로 구성됩니다.
*   `waypoints`: 하나 이상의 웨이포인트를 포함합니다. 웨이포인트는 특정 위치를 나타냅니다.
*   `routes`: 하나 이상의 경로를 포함합니다. 경로는 일련의 웨이포인트로 구성되며, 일반적으로 이동 순서를 나타냅니다.

## GPX 파일 예제

다음은 간단한 GPX 파일의 예입니다.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<gpx version="1.1">
  <metadata>
    <name>My GPS Track</name>
    <description>This is my GPS track from yesterday.</description>
    <creator>My GPS Device</creator>
    <generator>My Mapping Software</generator>
  </metadata>
  <track name="My Track">
    <numPoints>5</numPoints>
    <waypoint latitude="37.7749" longitude="-122.4194"/>
    <waypoint latitude="37.7833" longitude="-122.4064"/>
    <waypoint latitude="37.7905" longitude="-122.3982"/>
    <waypoint latitude="37.7972" longitude="-122.3899"/>
    <waypoint latitude="37.8040" longitude="-122.3816"/>
  </track>
</gpx>
```

## GPX 파일 뷰어

GPX 파일을 보려면 다음과 같은 다양한 뷰어를 사용할 수 있습니다.

*   웹 브라우저
*   매핑 소프트웨어 (예: QGIS, ArcGIS)
*   GPS 장치
*   전용 GPX 뷰어 애플리케이션

## 추가 정보

*   [GPX 파일 형식](https://en.wikipedia.org/wiki/GPX): 위키백과에서 GPX 파일 형식에 대한 자세한 정보를 확인할 수 있습니다.
---
