#정보관리기술사 #디지털네트워크 #SRT #스트리밍 #디지털네트워크/기타 #NEW
## 정의
SRT(Secure Reliable Transport)
- 공용 인터넷에서도 저지연·고신뢰로 오디오/비디오를 전송하는 User-level 전송 프로토콜
## 키워드
* TSBPD, ARQ, AES-128/256, Packet Reordering, Rate Adaptation
## 암기법
* 손지대암: 손실·지터·대역·암호
## 특징
- ARQ 선택 재전송, TSBPD 지터 흡수, Rate Adaptation
- AES-128/256 CTR, Re-keying, Handshake 인증
- ~120ms 저지연 목표
## 목적
- 불안정 인터넷 환경 실시간 AV 전송
- IPTV·원격 제작·라이브 스트리밍
## 구성요소
- 패킷 손실: ARQ·NAK·ACK/NAK/ACKACK
- 지터: TSBPD·Latency Buffer·Reordering
- 대역: Rate Adaptation·CCC·Packet Pacing
- 보안: AES·Re-keying·Session Protection
## 구성도
```
App → SRT(Recovery+Encrypt) → UDP → Internet → SRT(Decrypt) → App
```
## 연관 토픽
- [[MoQ]] - QUIC 미디어
- [[CDN]] - 콘텐츠 전송
- [[QoS]] - 서비스 품질
