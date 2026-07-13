#정보관리기술사 #보안 #SASE #보안/클라우드보안
Secure Access Service Edge
## 정의
- 광역 네트워킹(WAN)과 네트워크 보안 서비스(예 CASB, FWaaS, 제로트러스트)를 통합하여 제송하는 클라우드 기반 서비스 모델

## 키워드
- SD-WAN, 보안, Network as a Service, Network Security as a Service

## SASE 개념도
![[Pasted image 20260410002445.png|500]]

## SASE 구성 요소

|구성요소|핵심기술|설명|
|---|---|---|
|**네트워크 서비스**|**SD-WAN**|- SD-WAN Controller, SD-WAN CPE로 구성되어 통신망 사업자와 서비스 제공자 WAN으로 확장 적용하는 네트워크|
|**네트워크 서비스**|**SD-브랜치**|- 프로그래밍할 수 있고 중앙에서 오케스트레이션하는 방식으로 지사 환경에 더 많은 IT 인프라를 제공하는 기술 (LAN, Wi-Fi, SD-WAN, 라우팅, 보안 기능을 통합)|
|**보안 서비스**|**CASB**|- 클라우드 서비스 이용자와 클라우드 서비스 사이에 위치하여 독립적으로 보안 기능을 수행하는 소프트웨어|
|**보안 서비스**|**SECaaS**|- CSP SECaaS, SSP SECaaS로 제공하는 클라우드 보안 서비스|
|**보안 서비스**|**ZTNA**|- 기존 네트워크의 바깥 경계선(perimeter)에 도입했던 보안 개념을 데이터 하나하나의 바깥 경계선(microperimeter)에 적용하는 보안 모델|