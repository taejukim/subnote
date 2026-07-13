#정보관리기술사 #디지털네트워크 #MoQ #MediaOverQUIC
## 정의
MoQ(Media over QUIC)
- 실시간 대용량 콘텐츠 전송을 빠르고 안정적으로 처리하기 위해 QUIC 프로토콜 위에서 동작하는 미디어 전송 프로토콜
- HTTP 기반 전송의 지연을 극복한 차세대 저지연 미디어 스트리밍 프로토콜
## 키워드
* QUIC, WebTransport, Publisher-Relay-Subscriber, Track, Group, Object
## 암기법
* 전세보: 전송계층·세션계층·보안신뢰성
## 특징
- 저지연성: 수 ms 수준 초저지연
- 모듈성: Publisher·Relay·Subscriber 분리 구조
- 신뢰성: E2E 암호화·인증·권한 제어
- 확장성: WebTransport 기반 광범위 적용
## 목적
- HTTP 기반 미디어 전송의 지연·비효율 해결
- 실시간 스트리밍·게임 방송 등 저지연 서비스 제공
## 구성요소
- 등장 배경: HTTP 전송 지연, 전송 효율 저하, 복잡한 CDN 구조
- 프로토콜 스택: IP → UDP/TCP → TLS·QUIC·RTP → HTTP/3 → MoQ·RTP·WebRTC
- 전송 계층: QUIC, WebTransport
- 세션 계층: Publisher·Relay·Subscriber 모델, Track·Group·Object 구조, Session Negotiation
- 보안·신뢰성: E2E 암호화, 인증·권한 제어, Redundancy & Adaptive Delivery
- 비교 - MoQ: QUIC, 수 ms, WebTransport, 높은 모듈성, 실시간 스트리밍·게임
- 비교 - WebRTC: UDP+SRTP, 수백 ms, 부분 지원, 한계, 화상회의·채팅
- 비교 - HLS/DASH: HTTP+TCP, 수 초, 완전 지원, 제한, VOD·방송
## 구성도
```
[Publisher] → MoQ Track(Group/Object)
                  ↓
              [Relay 서버] (P2P/CDN)
                  ↓
            [Subscriber 다수]
              ↑ QUIC + WebTransport (저지연·E2E 암호화)
```
## 연관 토픽
- [[HTTP V3.0]] - HTTP/3 프로토콜
- [[TCP]] - 전송 제어 프로토콜
- [[UDP]] - 사용자 데이터그램 프로토콜
- [[Network Slicing]] - 네트워크 슬라이싱
