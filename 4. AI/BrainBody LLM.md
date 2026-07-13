#정보관리기술사 #AI #BrainBodyLLM #AI/LLM/생성AI #NEW
## 정의
BrainBody LLM
- 두 개의 대형 언어모델(LLM)을 계층적으로 사용해 모델 간 상호작용으로 오류를 지속적으로 개선하도록 설계된 에이전트 시스템
## 키워드
* Hierarchy, Plan, Execution, Feedback Loop
## 암기법
* 브바클: Brain(고수준계획)·Body(저수준실행)·Closed-Loop
## 특징
- 계층 계획: Brain 고수준 → Body 저수준 토큰/명령
- 폐루프: Simulator/환경 오류를 Brain에 환류해 계획 수정
- 지속 개선: Initial Plan → State Feedback → Updated Plan → SUCCESS
- 신체화 연계: 로봇·시뮬레이터 제어에 적합
## 목적
- 복잡한 물리·시뮬레이션 작업의 계층적 계획·실행
- 오류 피드백으로 계획 자기 수정
## 구성요소
- Brain LLM: 고수준 태스크 계획·의미 추론, 오류 원인 분석·계획 수정
- Body LLM: 저수준 제어·실행 명령 생성
- Closed-Loop Feedback: 오류·상태 → Brain → 계획 갱신
- 사례: WASH THE PLATE, ARRANGE THE CUBES 등
## 구성도
```
User Command + World Knowledge
 → Brain-LLM (High-level Plan)
 → Body-LLM (Low-level Plan/Tokens)
 → Simulator/Controller
 ↑________ Feedback & Error _________|
```
## 연관 토픽
- [[AI Agent]] - 에이전트 구조
- [[에이전틱 AI]] - 자율 수행
- [[VLA 모델]] - Vision-Language-Action
- [[신체화 AI]] - Embodied AI
