#정보관리기술사 #AI #앙상블학습 #AI/ML_알고리즘/기법
## 정의
- 여러개의 분류기를 생성하고, 그 예측을 결합함으로써 보다 적환한 예측을 도출하는 기법
## 키워드
- 과적합, 결합, 보팅
## 보팅(Voiting) 정의/개념
여러 개의 분류기가 **투표**를 통해 최종 예측 결과를 결정하는 방식입니다.
- **특징:** 서로 다른 알고리즘을 가진 분류기들을 결합 (예: Linear Regression + SVM)
- **보팅 방식:**
    - **하드 보팅(Hard Voting):** 다수 분류기의 예측 결과 중 다득표 결과 선택
    - **소프트 보팅(Soft Voting):** 분류기들의 결정 확률을 평균 내어 가장 높은 확률 선택
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260320222729.png|200]]

## 부스팅(Boosting) 정의/개념
**데이터 샘플링(Bootstrap)**을 통해 모델을 학습시키고 결과를 집계하는 방식입니다.
- **특징:** **동일한 유형의 알고리즘**을 사용하며, 샘플링된 데이터 셋(Sample Data set 1, 2...)으로 각각 학습
- **데이터 형태에 따른 결정:**
    - **Categorical (범주형):** 투표(Voting) 방식으로 결과 결정
    - **Continuous (연속형):** 평균(Average) 방식으로 결과 결정
 ![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260320222914.png|300]]
## 배깅(Bagging) 정의/개념
여러 개의 분류기를 **순차적으로 학습**시켜 **강한 분류기**를 만드는 방법입니다.
- **특징:** 앞선 모델의 **오류를 줄이는 데 초점**을 두며, 다음 분류기에 **가중치(Weight)**를 부여
- **주요 유형:**
    - **AdaBoost:** 에이다 부스트 (Adaptive Boosting)
    - **Gradient Boosting (GB):** 잔차를 경사하강법으로 보정
    - **XGBoost:** Extreme Gradient Boosting
    - **LightGBM:** Light Gradient Boosting Machine
    - **CatBoost:** Category Boosting
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260320222940.png|300]]
## 스태킹(Stacking) 정의/개념
**Cross Validation**을 기반으로 개별 모델이 예측한 데이터를 **meta dataset**으로 생성하여, 최종 모델인 **Meta Learner**에서 다시 학습하는 방식입니다.
- **프로세스:**
    1. Training Set을 여러 개별 모델(Model)이 학습
    2. 각 모델의 예측 결과를 모아 새로운 데이터 셋(New Training Set) 생성
    3. 최종 메타 모델(Meta Model)이 해당 데이터를 학습
    4. 최종 예측(Final Predictions) 도출
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260320222957.png|500]]