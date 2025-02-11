---
id: port-management
title: 노드를 위한 기술 인프라
sidebar_label: Technical Infrastructure For Nodes
description: Polygon 노드가 사용하는 기본 포트의 목록
keywords:
  - docs
  - polygon
  - matic
  - port
  - port management
  - infrastructure
  - default ports
image: https://wiki.polygon.technology/img/polygon-wiki.png
---

다음은 Polygon 노드에서 사용되는 기본 포트 목록입니다:

## Bor {#bor}

| ﻿이름 | 포트 | 태그 | 설명 |
|------------------------|-------|---------------------------|----------------------------------------------------------------------------------------------------------------|
| 네트워크 수신 대기 포트 | 30303 | 공개 | 네트워크 수신 대기 포트, Bor는 이 포트를 사용하여 피어에 연결하고 동기화 |
| RPC 서버 | 8545 | 공개 가능, 내부 | 트랜잭션을 전송하고 Bor에서 데이터를 받는 RPC 포트, Heimdall은 이 포트를 사용하여 체크포인트에 Bor 헤더를 가져옴 |
| WS 서버 | 8546 | 공개 가능, 내부 | 웹소켓 포트 |
| GraphQL 서버 | 8547 | 공개 가능, 내부 | GraphQL 포트 |
| 프로메테우스 서버 | 9091 | 공개 가능, 모니터링 | Grafanad의 데이터소스인 프로메테우스 서버 API, nginx 리버스 프록시를 통해 80/443에 매핑될 수 있음 |
| Grafana 서버 | 3001 | 공개 가능, 모니터링 | Grafana 웹 서버, nginx 리버스 프록시를 통해 80/443에 매핑될 수 있음 |
| Pprof 서버 | 7071 | 내부, 모니터링 | Bor에서 메트릭을 수집하는 Pprof 서버 |
| UDP 검색 | 30301 | 공개 가능, 내부 | 부트 노드 기본 포트 (피어 검색용) |

## Heimdall {#heimdall}

| ﻿이름 | 포트 | 태그 | 설명 |
|------------------------|-------|---------------------------|----------------------------------------------------------------------------------------------------------------|
| 네트워크 수신 대기 포트 | 30303 | 공개 | 네트워크 수신 대기 포트, Bor는 이 포트를 사용하여 피어에 연결하고 동기화 |
| RPC 서버 | 8545 | 공개 가능, 내부 | 트랜잭션을 전송하고 Bor에서 데이터를 받는 RPC 포트, Heimdall은 이 포트를 사용하여 체크포인트에 Bor 헤더를 가져옴 |
| WS 서버 | 8546 | 공개 가능, 내부 | 웹소켓 포트 |
| GraphQL 서버 | 8547 | 공개 가능, 내부 | GraphQL 포트 |
| 프로메테우스 서버 | 9091 | 공개 가능, 모니터링 | Grafanad의 데이터소스인 프로메테우스 서버 API, nginx 리버스 프록시를 통해 80/443에 매핑될 수 있음 |
| Grafana 서버 | 3001 | 공개 가능, 모니터링 | Grafana 웹 서버, nginx 리버스 프록시를 통해 80/443에 매핑될 수 있음 |
| Pprof 서버 | 7071 | 내부, 모니터링 | Bor에서 메트릭을 수집하는 Pprof 서버 |
| UDP 검색 | 30301 | 공개 가능, 내부 | 부트 노드 기본 포트 (피어 검색용) |