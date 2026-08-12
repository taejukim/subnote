#정보관리기술사 #보안 #SSL #핸드쉐이크
## 정의
SSL(Secure Socket Layer)
- 응용계층과 TCP 전송계층 사이에서 클라이언트-서버 간 안전한 보안 채널을 형성하는 보안 프로토콜
- 공개키 기반 인증과 대칭키 세션키 교환으로 기밀성·무결성·인증을 제공하는 전송보안 표준
## 키워드
* Handshake Protocol, Record Protocol, Change Cipher Spec, Alert Protocol, X.509 인증서, HTTPS/443
## 암기법
* 핸체알레: Handshake·Change Cipher Spec·Alert·Record (SSL 4대 서브 프로토콜)
## 특징
- 공개키 기반 인증: RSA 방식과 X.509 v3 인증서로 신뢰성 있는 인증 수행
- 3가지 인증모드: 익명·서버·클라이언트-서버 인증 모드 선택 지원
- 계층 구조: 상위(Handshake·ChangeCipherSpec·Alert)와 하위(Record) 프로토콜로 구성
- 알고리즘 협상: 다양한 암호화·MAC·압축 알고리즘을 세션별로 선택 협상
## 목적
- 웹 통신 구간의 도청·변조·위장을 방지하는 안전한 채널 확보
- 클라이언트-서버 간 상호 신원 인증 및 데이터 기밀성·무결성 보장
## 구성요소
- Handshake Protocol: 상호인증, 암호키 교환, 알고리즘/MAC/압축 방식 협상, 세션키 생성
- Change Cipher Spec Protocol: 협상된 암호방식 적용 시작을 알림
- Alert Protocol: 암호·압축·인증 오류 등 에러 발생 통보
- Record Protocol: 응용데이터를 레코드 단위로 단편화·압축·MAC첨부·암호화하여 전달
- 핸드쉐이크 절차: ClientHello → ServerHello → ServerKeyExchange → ServerHelloDone → ClientKeyExchange → ChangeCipherSpec → Finished
## 구성도
```
[상위 Protocol]  Handshake ─ ChangeCipherSpec ─ Alert
                        ↓ (협상된 파라미터 전달)
[하위 Protocol]  Record Protocol (단편화→압축→MAC→암호화)
                        ↓
Client ──ClientHello──> Server
Client <──ServerHello, KeyExchange, HelloDone── Server
Client ──ClientKeyExchange, ChangeCipherSpec, Finished──> Server
```
## 연관 토픽
- [[제로트러스트]] - mTLS 기반 상호인증 확장
- [[Secure SDLC 및 STRIDE 기반 위협 모델링]] - Tampering 대응 TLS 암호화
- [[금융권 내부망 SaaS 보안대책]] - TLS 1.2 이상 연계구간 암호화
- [[PKI]] - 공개키 인증서 발급·검증 체계
