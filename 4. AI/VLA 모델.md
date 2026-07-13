#정보관리기술사 #AI #VLA #VisionLanguageAction
## 정의
시각언어행동 모델(VLA, Vision-Language-Action)
- 시각 정보·자연어 명령·물리적 행동을 통합한 멀티모달 AI 모델
- 로봇·자율주행이 보고·이해하고 행동할 수 있게 하는 피지컬 AI 핵심 기술
## 키워드
* Multi-Modal, Embodied AI, Foundation Model, Closed-Loop, PEFT, Tokenizer
## 암기법
* 입출모피: 입력·출력·모델·피드백
## 특징
- 초기 융합성: 시각·언어·행동 다중 모달 통합
- 이중 시스템성: 빠른 반응 + 느린 추론 아키텍처
- 자가 수정성: 환경 피드백 기반 자체 수정
- 효율성: 매개변수 및 추론 효율화
## 목적
- 범용 로봇 에이전트 실현
- 시각·언어·행동의 통합적 자율 수행
## 구성요소
- 입력 데이터: 다중 모달 데이터, 사용자 명령, 센서 데이터
- VLA 핵심 모델: VLM Backbone, Fusion Module, Task Planner, 동작 생성 헤드
- 출력·피드백: 액션 토크나이저, 컨트롤러, 폐루프 피드백
- 작동 원리: 멀티모달 공통 언어화 → 상호 참조 상황 이해 → 자기회귀 다음 동작 예측 → 추상 토큰→물리 신호 변환 → 폐루프 환경 적응
- 활용: 휴머노이드, 의료/헬스케어, 자율주행, 정밀 농업, 산업용 로봇
- 도전과제: 실시간 추론, 안전성, 데이터 편향, 컴퓨팅 요구
- 해결: 모델 경량화, 병렬 디코딩, RLHF, 합성데이터, 연합학습, PEFT
## 구성도
```
[Vision] + [Language] + [Sensor] → VLM Backbone → Fusion Module
   → Task Planner → Action Tokenizer → Controller → 물리 행동
   ↑___________________ Closed-Loop Feedback ___________________|
```
## 연관 토픽
- [[신체화 AI]] - Embodied AI 개념
- [[피지컬 AI(Physical AI)]] - 물리 세계 AI
- [[휴머노이드 로봇]] - 적용 사례
- [[멀티모달(Multi Modal) AI]] - 다중 모달 학습
