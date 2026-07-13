#정보관리기술사 #디지털네트워크 #BGP #라우팅 #NEW
## 정의
BGP(Border Gateway Protocol)
- 서로 다른 AS(Autonomous System) 간 라우팅 정보를 교환하는 Exterior Gateway 프로토콜
- Open·Update 등으로 이웃을 맺고 Weight·Local Preference 등 메트릭으로 경로 우선순위 결정
## 키워드
* iBGP, eBGP, Path Vector, AS, Local Preference, MED
## 암기법
* 내외AS: 같은AS=iBGP, 다른AS=eBGP
## 특징
- Path Vector: AS-Path를 누적해 루프 방지·경로 선택
- iBGP/eBGP: 동일 AS 내부 / 이종 AS 간 연결
- TCP 179: Open으로 Neighbor 수립
- 정책 라우팅: Local Pref·MED·Weight로 출입 경로 제어
## 목적
- 인터넷 규모 AS 간 경로 정보 교환
- 정책 기반의 안정적 외부 라우팅
## 구성요소
- Next-Hop: BGP 정보 전달 라우터 IP, 목적지 경유 필수 주소
- Local Preference: 출구 경로 우선순위(기본 100)
- AS-Path: 경유 AS 목록, 짧을수록 선호
- MED: 다중 진입 경로 시 우선순위(Multi-Exit-Discriminator)
- Open: TCP 179 Neighbor 설정
- Update: 도달 가능성 정보 비정기 교환
- Notification: 오류·이웃 단절 통보
- Keepalive: Neighbor 생존 확인
- Route-Refresh: Neighbor 정보 재확인
## 구성도
```
[AS 200]──eBGP──[AS 100]
  iBGP mesh      iBGP mesh
 (내부 동일AS)   (내부 동일AS)
```
## 연관 토픽
- [[라우팅 알고리즘]] - 거리벡터·링크상태·경로벡터
- [[Distance Vector Algorithm]] - IGP 거리벡터
- [[Link State Algorithm]] - IGP 링크상태
- [[OSI 7 Layers]] - 네트워크 계층 라우팅
