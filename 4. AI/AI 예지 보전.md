#정보관리기술사 #AI #예지보전 #PdM #AI/ML/기법 #NEW
## 정의
AI 예지 보전(Predictive Maintenance, PdM)
- 설비 유·무선 센서로 실시간 데이터를 수집하고 AI로 잠재적 고장 시기·부품 교체 시점을 예측하는 AI 기술
## 키워드
* 멀티모달 센서, MQTT, 이상탐지, 고장진단, GAN, Autoencoder, RUL, 정비 추천
## 암기법
* 수분의: 수집·분석·의사결정
## 특징
- Big Data·Domain Knowledge + Expert System·ML 융합
- 실시간 모니터링·이상 감지·자동 고장 진단
- RUL 예측·정비 시나리오 권고
## 목적
- 계획적 정비로 다운타임 최소화
- 설비 수명·생산성 최적화
## 구성요소
- 데이터: 멀티모달 센서, MQTT Publisher, 데이터 게이트웨이
- 분석: 이상탐지(Outlier), 고장진단(베어링·기어 패턴)
- AI: GAN(불균형 해소), Autoencoder, Feature Engineering
- 의사결정: RUL 예측기, 정비 추천 시스템
## 구성도
```
센서 → 게이트웨이 → 이상탐지/고장진단 → RUL → 정비 추천
```
## 연관 토픽
- [[스마트 팩토리(Smart Factory)]] - 스마트 제조
- [[디지털트윈]] - 설비 시뮬레이션
- [[센서 퓨전]] - 다중 센서 통합
