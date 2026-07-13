#정보관리기술사 #디지털네트워크 #CDN #콘텐츠전송 #NEW
## 정의
CDN(Contents Delivery Network)
- 중간경로를 최소화해 콘텐츠를 효율 전달하기 위해 ISP 다수 노드(웹 캐시)에 데이터를 복제·저장·제공하는 시스템
- End-User가 Embedded URL의 CDN 서버에서 객체를 수신
## 키워드
* Caching, GSLB, Load Balancing, Streaming, Request Routing
## 암기법
* 캐글스: 캐싱·GSLB·스트리밍
## 특징
- Edge 복제: POP/Cache에 콘텐츠 분산 저장
- 경로 단축: First/Middle/Last-mile 구조로 지연 감소
- 부하 분산: GSLB·LB로 최적·가용 서버 선택
- 동기화: 분산 ISP 서버에 동일 콘텐츠 즉시 반영
## 목적
- 원본(CP) 부하·지연 감소, 전송 효율 향상
- 대용량 스트리밍·SW 배포의 안정 전달
## 구성요소
- CDN SP / CP / ISP / User / POP / IX
- Caching: 자주 접근 페이지 복사·저장·응답
- GSLB: 분산 캐시 중 최적 서버 선택 연결
- Load Balancing: 트래픽 분산·장애 서버 배제
- Streaming: 전체 다운로드 없이 즉시 재생
- 배포·동기화: 지역 분산 동일 콘텐츠 유지
- Grid Delivery: 일정 트래픽 이상 P2P로 보조 전송
- Request Routing: 근접·부하 기반 최근접 Cache 선택
## 구성도
```
[User]─Last-mile─[POP/Cache]─Middle-mile─[IX]─First-mile─[ISP/CP]
1) CP HTML(+Embedded CDN URL) 2) CDN Object 요청 3) 복제본 전달
```
## 연관 토픽
- [[DNS]] - 이름 해석·트래픽 유도
- [[HTTP V3.0]] - 웹 콘텐츠 전송
- [[MoQ]] - 저지연 미디어 전송
- [[SD-WAN]] - 광역 경로 최적화
