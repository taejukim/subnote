#정보관리기술사 #보안 #mTLS #MutualTLS #보안/인증/접근제어 #NEW
## 정의
mTLS(Mutual TLS)
- 클라이언트와 서버가 서로의 신원을 모두 인증하는 상호 TLS 암호화 프로토콜
- TLS는 서버만 인증, mTLS는 양방향 인증
## 키워드
* 공개키, 개인키, TLS Certificate, TLS Handshake, 상호 인증
## 암기법
* 연제확권암: 연결·제시·확인·권한·암호통신(7단계)
## 특징
- 7단계: Client 연결 → Server TLS → Client 검증 → Client TLS → Server 검증 → 권한 → 암호 통신
- Spoofing·Credential Stuffing·Phishing·악의적 API 요청 방어
## 목적
- Zero Trust·마이크로서비스 상호 인증
- API·서비스 메시 보안 강화
## 구성요소
- 공개키/개인키, TLS 인증서, TLS Handshake
- 기술: Certificate Authority, 양측 인증서 검증
## 구성도
```
Client ↔ [Server Cert↔Client Cert] ↔ Encrypted TLS
```
## 연관 토픽
- [[SSL_TLS]] - TLS/SSL
- [[SDP]] - Zero Trust
- [[OAuth]] - API 인증
