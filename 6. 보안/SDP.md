#정보관리기술사 #보안 #SDP #ZeroTrust #ZTNA #NEW
## 정의
SDP(Software Defined Perimeter)
- 애플리케이션 연결 허용 전 사용자 상태·ID 기반 선 인증, 후 연결로 신뢰 보안연결을 제공하는 클라우드 네트워크 접근제어 프레임워크
## 키워드
* Zero Trust, 선 인증·후 연결, SDP Controller, SDP Agent, SDP Gateway, PDP, PEP, ZTNA
## 암기법
* 에이컨게: Agent·Controller·Gateway / 선후: 선인증·후연결
## 특징
- 신원 중심: ID·상태 기반 접근
- Zero Trust: 정책·통제 후 허가
- 화이트리스트·동적 ID (VPN의 블랙리스트·정적 IP와 대비)
- SPA·IPSec 기반 보안 접속
## 목적
- 클라우드 환경에서 최소 권한·사전 인증 접근 통제
- 전통 VPN의 광역 노출·정적 경계 한계 보완
## 구성요소
- SDP Agent: PKI·SAML·OAuth, Controller 통신 후 허가·Gateway 보안접속
- SDP Controller: Zero Trust·RBAC, Agent·Gateway 간 연결 가능 여부 결정
- SDP Gateway: IPSec·SPA, 신원 검증된 사용자·앱 연결 제공
- 인증 ①접속요청(OAuth 등) ②Gateway에 SPA 정보전달 ③Zero Trust 기반 허가
- 연결 ④Agent↔Gateway IPSec 보안접속 ⑤허용 서비스 접속
- PDP: 주체에 대한 자원 접근 권한 결정·자격증명 생성
- PEP: 사용자–자원 연결의 활성화·감시·종료
- vs VPN: 사설망 vs 선인증후연결, 정적IP/블랙리스트 vs 동적ID/화이트리스트
## 구성도
```
[SDP Agent]─①요청─→[SDP Controller]─②SPA정보─→[SDP Gateway]
     ↑                    │③허가                      │
     └────────────────────┘                    ⑤서비스
     ←════ ④ IPSec 보안접속 ══════════════════→[Protected]
```
## 연관 토픽
- [[제로 트러스트(Zero Trust)]] - 신뢰 제로 접근 모델
- [[VPN]] - 전통 원격 접속·터널
- [[SASE]] - 클라우드 보안 액세스
- [[접근제어(AC)]] - 접근 통제
