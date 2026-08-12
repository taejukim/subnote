#정보관리기술사 #AI #VLA #PhysicalAI
## 정의
VLA(Vision-Language-Action) 모델
- 시각·자연어명령·물리적 행동을 통합해 로봇이 보고-이해하고-행동하도록 하는 피지컬 AI 핵심 모델
- Foundation Model의 지식을 물리적 하드웨어 실행 영역으로 확장한 체화된 지능(Embodied AI)
## 키워드
* VLM Backbone, Fusion Module, Task Planner, Action Tokenizer, Cross-modal Attention, Autoregressive Decoder, Embodied AI
## 암기법
* 시언행폐: 시각·언어·행동·폐루프피드백(VLA 핵심 처리 흐름)
## 특징
- 멀티모달통합: 시각·언어·상태정보를 공통 토큰으로 통일 처리
- 이중시스템: 저지연 물리제어(빠른 시스템)와 고차원 계획(느린 LLM) 결합
- 자기수정성: 실패 감지 시 보조경로로 상황 진단·복구
- 경량효율성: LoRA·양자화로 파라미터 축소, 병렬디코딩으로 속도 향상
## 목적
- 범용 로봇 에이전트 구현을 위한 시각-언어-행동 통합 프레임워크 제공
- 비정형 환경에서도 자연어 지시만으로 물리적 과업 수행 가능케 함
## 구성요소
- 입력데이터: 카메라·센서 등 멀티모달 데이터, 사용자 자연어 명령
- VLM Backbone: 대규모 시각-언어 사전학습 거대모델
- Fusion Module/Task Planner: 감각정보 결합 및 행동순서 추론
- Action Tokenizer/동작생성헤드: 상태·행동 토큰 생성, 제어값 출력
- Controller/폐루프 피드백: 물리신호 변환 및 실시간 상태 반영
## 구성도
```
[시각·언어·센서 입력] → [VLM Backbone·Fusion Module] → [Task Planner]
                                                              ↓
                                            [Action Tokenizer·동작생성헤드]
                                                              ↓
                              [Controller 물리신호 변환] → [로봇 행동 실행]
                                                              ↓
                              [폐루프 피드백] ─────────────────┘
```
## 연관 토픽
- [[피지컬 AI(Physical AI)]] - 물리세계 인식·행동 AI 시스템
- [[Embodied AI]] - 체화된 지능 개념
- [[지식증류(Knowledge Distillation)]] - VLA 경량화 핵심 기법
- [[트랜스포머(Transformer)]] - VLA 백본 아키텍처 기반 모델
