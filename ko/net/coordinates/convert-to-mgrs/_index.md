---
title: MGRS 좌표 변환
linkTitle: MGRS 좌표 변환
weight: 10
url: /ko/net/coordinates/convert-to-mgrs/
description: MGRS(Military Grid Reference System) 좌표를 다른 좌표계로 변환하는 방법을 설명합니다.
---

## MGRS 좌표 변환하기

MGRS(Military Grid Reference System)는 전 세계를 격자 형태로 나누어 위치 정보를 나타내는 시스템입니다. 이 문서는 MGRS 좌표를 다른 좌표계, 예를 들어 위도/경도로 변환하는 방법에 대한 안내를 제공합니다.

### MGRS란?

MGRS는 군사 목적으로 개발되었지만 현재 다양한 분야에서 사용되고 있습니다. MGRS 좌표는 격자 구역의 위치를 나타내는 문자열로 구성됩니다. 이 문자열은 다음과 같은 정보를 포함합니다.

*   **격자 구역 식별자:** 전 세계를 나누는 격자의 고유한 식별자입니다.
*   **좌표:** 격자 구역 내의 특정 지점의 좌표입니다.

### 변환 과정

MGRS 좌표를 다른 좌표계로 변환하려면 다음과 같은 단계를 따릅니다.

1.  **MGRS 좌표 확인:** 변환할 MGRS 좌표 문자열을 확인합니다.
2.  **좌표 분리:** MGRS 좌표 문자열에서 격자 구역 식별자와 좌표를 분리합니다.
3.  **좌표계 변환:** 격자 구역 식별자를 사용하여 해당 지역의 좌표계를 결정하고, 좌표를 위도/경도 또는 다른 원하는 좌표계로 변환합니다.

### 사용 가능한 도구

MGRS 좌표 변환을 위한 다양한 온라인 도구와 소프트웨어가 있습니다. 몇 가지 예는 다음과 같습니다.

*   **Online MGRS Converter:** [https://www.geodataservices.com/mgrs-finder](https://www.geodataservices.com/mgrs-finder)
*   **GDAL:** GDAL은 다양한 좌표계 간의 변환을 지원하는 강력한 지리 공간 데이터 처리 라이브러리입니다.

### 추가 정보

MGRS에 대한 자세한 내용은 다음 자료를 참조하십시오.

*   **Wikipedia - MGRS:** [https://en.wikipedia.org/wiki/Military_grid_reference_system](https://en.wikipedia.org/wiki/Military_grid_reference_system)
---
