#정보관리기술사 #보안 #TTPs #MITREATTCK
## 정의
TTPs(Tactics, Techniques and Procedures)
- 공격자 전술·기법·절차를 계층구조로 체계화한 행위기반 위협정보
- 공격자 행동을 이해·예측하는 능동적 보안 접근법의 핵심 개념
## 키워드
* 전술·기법·절차, MITRE ATT&CK, 위협 인텔리전스, IOC, STIX/TAXII
## 암기법
* 계매행표: 계층구조·매트릭스화·행동패턴기반·표준화공유
## 특징
- 계층구조: 전술(목표)-기법(방법)-절차(실제 실행방식) 3계층 체계화
- 매트릭스화: MITRE ATT&CK이 14개 전술·200개 이상 기법을 매트릭스로 정리
- 행동패턴 기반: IOC 대비 변경이 어려운 행동패턴으로 탐지 지속성 높음
- 표준화 공유: STIX/TAXII로 IOC·TTP를 구조화해 자동 배포·공유
## 목적
- 공격자 행동 이해를 통한 능동적 위협 헌팅 실현
- 조직 탐지 커버리지 시각화 및 보안투자 우선순위 결정
## 구성요소
- 전술(Tactic): 공격자 전략적 목표단계(TA0001~TA0043)
- 기법(Technique): 전술달성 구체방법(T1xxx, Sub-technique)
- 절차(Procedure): 특정 위협행위자 실제 실행방식(G0xxx, S0xxx)
- 탐지·완화(Detection·Mitigation): Sigma·YARA 룰, SIEM/EDR 연계
- 공유형식(STIX/TAXII): IOC·TTP 구조화, MISP·OpenCTI로 자동배포
## 구성도
```
[전술: 목표단계] → [기법: 구체방법] → [절차: 실제 실행사례]
        │                                     │
   MITRE ATT&CK 매트릭스 매핑          위협행위자(G0xxx)·도구(S0xxx)
        │
[탐지·완화 매핑] → SIEM/EDR 연계 → STIX/TAXII로 공유(MISP, OpenCTI)
```
## 연관 토픽
- [[OWASP LLM Top 10:2025]] - AI 특화 위협 분류체계
- [[ISMS-P 인증제도]] - 침해사고 대응 체계 연계
- [[PQC(양자내성암호)]] - 차세대 보안 위협 대응 기술
