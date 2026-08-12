#정보관리기술사 #프로젝트관리 #AIDLC #AI에이전트
## 정의
AI-DLC(AI-Driven Development Life Cycle) 기반 프로젝트 관리
- 기존 SDLC의 요구분석~운영 단계를 AI 협업 중심으로 전환한 개발방법론
- AI가 산출물을 생성하고 인간이 검토·승인하는 HITL 기반 개발 생애주기
## 키워드
* Human-AI 협업, HITL, Unit/Bolt, Self-Correction Loop, Audit Trail, DevSecOps
## 암기법
* 협실생맥: 협업형개발·인간승인실행·생애주기내재화·맥락축적 (AI-DLC 4대 특징)
## 특징
- 협업형 개발: AI를 협력자로 활용하는 동적 팀 구성
- 인간 승인 실행: AI 산출물을 인간이 검토한 후 반영
- 생애주기 내재화: Inception-Construction-Operations 전 과정에 AI 내재화
- 맥락 축적: Unit/Bolt 반복을 통해 의사결정 이력을 누적
## 목적
- AI 중심 협업·자동화를 통한 개발 생산성 극대화
- AI 산출물의 정확성·보안성·책임성 확보를 위한 통제체계 구축
## 구성요소
- PM 역할: 범위/요구/일정/조직/도구/위험/품질/추적 관리
- 요구분석: 요구 컨텍스트 구조화, AI질의를 통한 인간 승인
- 구현: Self-Correction Loop, Continuous Code Inspection
- 테스트: Auto Test Generation, Edge-case Simulation
- 배포/운영: Automated Quality Gate, Anomaly Detection, Feedback Loop
## 구성도
```
[Inception] → [Construction] → [Operations]
     └── Unit ── (Bolt: 계획→질문→승인→실행→검증) 반복 ──┘
              ↑ Human 검토·승인(HITL)     AI 생성/실행 ↓
        Feedback Loop(장애·기술부채) → 다음 Inception 반영
```
## 연관 토픽
- [[SDLC]] - 전통적 소프트웨어 개발 생애주기
- [[HITL]] - 인간 개입 기반 AI 의사결정 체계
- [[AI 거버넌스]] - AI 활용 위험·책임 통제 체계
- [[DevSecOps]] - 보안 내재화 개발·운영 통합 방식
