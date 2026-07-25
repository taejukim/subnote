#정보관리기술사 #보안 #React2Shell #CVE-2025-55182 #보안/공격/위협 #NEW
## 정의
React2Shell
- React 19·Next.js 15/16 하위 버전 서버 함수 처리 중 역직렬화 기반 RCE 취약점(CVE-2025-55182, CVSS 10.0)
## 키워드
* 역직렬화, Flight Protocol, Prototype Pollution, Reverse Shell, RCE
## 암기법
* 악역프원: 악성요청·역직렬화·프로토타입·RCE
## 특징
- Flight Stream 조작, Action ID Discovery
- 불안전 역직렬화 → Prototype Pollution → OS Command Injection
- C&C 리버스 쉘 연결
## 목적
- React/Next.js 서버 원격 코드 실행
- 웹 애플리케이션 장악
## 구성요소
- 공격: Flight 조작, 역직렬화, 프로토타입 오염, OS 명령·리버스 쉘
- 대응: Secure Coding, SPM, 3-Tier 망분리, 컨테이너 격리, 긴급 패치, WAF
## 구성도
```
악성 Flight 요청 → 역직렬화 → Prototype Pollution → RCE → C&C
```
## 연관 토픽
- [[OWASP LLM Top 10]] - LLM·웹 보안
- [[시큐어 코딩]] - 입력 검증
- [[SW개발보안(시큐어 코딩)]] - 개발 보안
