#정보관리기술사 #보안 #AgenticAI #Claude Mythos
## 정의
Claude Mythos / Agentic AI 보안 패러다임
- Anthropic의 자율 AI Agentic 시스템 공개로 촉발된, 목표를 스스로 해석·계획·실행하는 AI의 사이버보안 위협·방어 패러다임 변화
- Project Glasswing 등 방어자가 공격자보다 먼저 동일 AI 능력을 확보하는 Defender-First 전략 대두
## 키워드
* 목표(Goal), 자율성, 다단계 추론, Zero Trust, Least Agency, AIBOM, Project Glasswing, Defender-First
## 암기법
* 가통예협: 가시성·통제·예측대응·협력 (Agentic AI 보안 4대 프레임워크)
## 특징
- 높은 자율성: 상위 목표만 부여받아 하위 목표를 스스로 설정, 다단계(Multi-step) 추론·재계획 수행
- 광범위한 위협면: 목표탈취·도구오염·메모리오염 등 AI Agent 대비 통제·추적이 어려움
- 사이버킬체인 자동화: 정찰부터 침투경로 설계까지 단일 흐름으로 다수 표적 동시 공략 가능
- 적응형 방어 필요: AI로 AI에 대응하는 자율 SOC·상시 위협헌팅 기반 방어 체계 요구
## 목적
- Agentic AI가 야기하는 신종 사이버위협(취약점 자동탐색, 지속적응 공격)에 대한 선제 대응
- 방어자 우위 확보를 위한 글로벌 협력적 방어 능력 구축
## 구성요소
- Agentic AI 특성: 목표달성자, 장기메모리, 다중도구 오케스트레이션, 다중에이전트 협업
- 신규 위협: 취약점발굴 자동화, 사이버킬체인 자동화, 초개인화 피싱, 도구·권한 오남용, 적응형 공격
- 대응방안 - 개별측면: Risk-Based 우선순위, 행위기반탐지, Zero Trust+최소권한, 적응형 방어
- 대응방안 - 계층측면: 예방(Prevent)·탐지대응(Detect&Respond)·거버넌스(Govern) 3-Layer
- Project Glasswing: 로컬 취약점 자율탐지, 자율 침투테스트, 오픈소스 코드 강화
## 구성도
```
[Agentic AI 공격측]                    [Defender-First 방어측]
목표설정→계획→실행 ─────대칭──────→ Project Glasswing
(취약점탐색·킬체인자동화)              (자율탐지·침투테스트·OSS강화)
        ↓                                   ↓
   가시성(AIBOM) → 통제(Zero Trust) → 예측·대응(AutoSOC) → 협력(글로벌 거버넌스)
```
## 연관 토픽
- [[사이버 보안 플랫폼(SIEM,SOAR)]] - 행위기반 탐지 인프라
- [[제로트러스트]] - Agentic AI 통제 경계 재설계 원칙
- [[SBOM]] - AIBOM으로 확장되는 자산 추적
- [[APT]] - Agentic AI 기반 자동화된 지속 표적공격
