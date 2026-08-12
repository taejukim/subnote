#정보관리기술사 #디지털서비스 #Sim2Real #PhysicalAI
## 정의
Sim2Real(Simulation-to-Reality)
- 시뮬레이션에서 생성된 경험과 학습된 지능을 현실 세계로 이전해 안정적으로 동작하게 하는 전이 메커니즘
- Physical AI의 "Last-Mile Transfer"로 Reality Gap을 극복하는 핵심 기술
## 키워드
* 도메인 랜덤화, Digital Twin, 동역학 보정, ADR, 강건 정책 학습
## 암기법
* 합도현물강: 합성경험생성·도메인랜덤화·현실적응·물리정합성·강건정책학습(5대 기술요소)
## 특징
- 합성 경험 생성: Physics Simulation·Digital Twin으로 대규모 학습데이터 확보
- 도메인 랜덤화: 시각·동역학 랜덤화 및 ADR로 일반화 성능 향상
- 물리 정합성 확보: 동역학 보정(System Identification)으로 현실과 근접
- 강건 정책 학습: 고수준 정책학습으로 환경 불확실성에 안정적 대응
## 목적
- 현실에서 수집하기 어려운 희귀·극한 상황 데이터의 학습 확보
- Reality Gap 극복을 통한 현실 환경에서의 안정적 성능 재현
## 구성요소
- 합성 경험 생성: Physics Simulation, Digital Twin, Synthetic Data
- 도메인 랜덤화: 시각/동역학 랜덤화, 자동 도메인 랜덤화(ADR)
- 현실 적응: 의미정보(Semantic) 정렬, 특징(Feature) 정렬
- 물리 정합성 확보: 동역학 보정, 적응형 시뮬레이션
- 강건 정책 학습: 고수준 정책학습, 강건 정책 생성
## 구성도
```
[Physics Simulation/Digital Twin] → [합성 경험 생성]
             ↓
   [도메인 랜덤화(시각/동역학/ADR)] → [현실 적응(의미/특징 정렬)]
             ↓
   [물리 정합성 확보(동역학 보정)] → [강건 정책 학습]
             ↓
       [현실 세계 로봇 행동 능력 (Embodied Capability)]
```
## 연관 토픽
- [[Physical AI]] - Sim2Real이 속하는 상위 개념
- [[디지털트윈]] - 현실 재현 시뮬레이션 기술
- [[강화학습]] - 정책 학습의 기반 알고리즘
- [[휴머노이드 로봇]] - Sim2Real 대표 적용 사례
