#정보관리기술사 #AI #XAI #설명가능AI
## 정의
XAI(eXplainable AI)
- AI가 왜 그렇게 판단했는지에 대한 설명을 제공하는 인공지능 및 그 평가 기술
- 투명성·신뢰성·편향 개선을 위해 모델 예측 근거를 정량적으로 평가하는 체계
## 키워드
* Descriptive Accuracy, Sparsity Accuracy, Cumulative Descriptive Accuracy, XAI Weight
## 암기법
* 설희누가: 설명정확성·희소성정확도·누적설명정확도·가중치평가(XAI 4대 평가기술)
## 특징
- 설명 정확성(DA): 관련성 높은 피처 제거 시 예측 변화로 설명력 측정
- 희소성 정확도(SA): 가중치가 정확히 0인 비율(MAZ)로 희소성 평가
- 누적 설명 정확도(CDA): 상위 N개 피처 누적 제거로 정확도 하락폭 측정, 면적 작을수록 우수
- XAI 가중치 평가: 피처 기여도와 정확도 하락값의 상관관계 검증
## 목적
- AI 예측 과정의 투명성 확보 및 숨겨진 패턴·지식 발견
- AI 응용에서 잠재적 편향과 원치 않는 결과 완화
## 구성요소
- Descriptive Accuracy: 관련 피처 순차 제거 후 예측 변화 관찰
- Sparsity Accuracy: [-1,1] 정규화 후 MAZ 계산
- Cumulative Descriptive Accuracy: 상위 N개 피처 누적 제거, 정확도 하락 곡선 면적 평가
- XAI Weight 기반 평가: 기여도 점수와 정확도 하락값의 비율 표준편차로 신뢰도 검증
## 구성도
```
[입력 데이터] → [딥러닝 모델] → [모델 출력] + [모델 설명(XAI)]
                                        ↓
      [평가: DA·Sparsity Accuracy·CDA·XAI Weight]
                                        ↓
        [투명성/신뢰성 향상] + [편향 완화]
```
## 연관 토픽
- [[모델 해석성]] - XAI의 상위 목표 개념
- [[SHAP]] - 대표적 XAI 피처 기여도 산출 기법
- [[AI 거버넌스]] - XAI 결과를 활용한 신뢰성 확보 체계
- [[편향 완화]] - XAI 평가로 도출되는 개선 활동
