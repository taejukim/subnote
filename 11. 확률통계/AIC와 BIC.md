#정보관리기술사 #확률통계 #AIC와BIC #확률통계/분석 #NEW
## 정의
AIC(Akaike Information Criterion)
- 모델 적합도(log-likelihood)와 변수 개수(복잡도)를 동시에 고려하는 지표
BIC(Bayesian Information Criterion)
- 표본 크기 n을 고려하여 복잡한 모델에 더 큰 패널티를 부여하는 지표
## 키워드
* 회귀, 모델 적합도·복잡도 균형, Likelihood, 패널티
## 암기법
* AIC=2p / BIC=log(n)p
## 특징
- AIC: 예측 성능 중심, 패널티 약함→복잡 모델·과적합 위험
- BIC: 진실성·단순 모델 선호, n>8이면 AIC보다 변수에 민감
## 목적
- 적합도와 복잡도 균형으로 최적 모델 선택
## 구성요소
- AIC = −2 log(L) + 2p
- BIC = −2 log(L) + log(n)·p
- 최소화: Likelihood↑, p↓ 가 유리 / Bias–Variance 균형
## 구성도
```
실제분포 vs 모델분포 차이 + 복잡도 패널티
AIC: −2logL + 2p
BIC: −2logL + log(n)p  → 작을수록 선호
```
## 연관 토픽
- [[시계열 분석]] - ARIMA 차수 선택
- [[추정 이론]] - Likelihood
- [[ANOVA]] - 모델 비교
