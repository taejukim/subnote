#정보관리기술사 #AI #PINN #PhysicalAI #AI/ML/기법 #NEW
## 정의
물리 정보 신경망(PINN, Physics-Informed Neural Network)
- PDE(편미분방정식) 등 물리 법칙을 Loss Function에 내재화한 Physics AI 신경망
- 소량 데이터로도 물리적 일관성·고예측 정확도 제공
## 키워드
* PDE, Physics Loss, Data Loss, BC, Automatic Differentiation, Collocation
## 암기법
* 물손하: 물리+데이터 하이브리드
## 특징
- L_total = L_data + L_phys
- 데이터 부족·물리 불일치·시뮬레이션 한계 해결
- DNN 대비 PDE·경계조건 반영
## 목적
- Physical AI·Digital Twin 고신뢰 예측
- 적은 실험 데이터로 물리 모델 학습
## 구성요소
- Physics Model: PDE, BC, IC
- Learning: DNN, Hybrid, Collocation Point
- Loss: Data Loss, Physics Loss, Residual Loss
- Optimization: Automatic Differentiation, Backpropagation
## 구성도
```
Input → DNN(u) → L_data + L_phys(PDE/BC) → Backprop → PINN solution u(x,t)
```
## 연관 토픽
- [[디지털트윈]] - 물리-가상 동기화
- [[합성데이터]] - 데이터 보강
- [[양자머신러닝]] - 물리 기반 AI
