#정보관리기술사 #AI #혼동행렬 #AI/AI_평가/테스트
## 정의
- 데이터 분석에서 잘못된 예측의 영향을 파악하기 위해 예측된 값과 실제 값이 일치하는지 여부를 행렬로 분류하는 모델 평가 기법
## 키워드
* TP/FP/FN/TN
* Precision, Accuracy, Recall, Specificity, FR Rate, F1 Score, Kappa
## 개념도
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260320232615.png|600]]

## ROC Curve, AUC, PR Plot
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260320232647.png|700]]
- ROC커브는 이진 분류기의 성능을 표현하는 커드이고, 가능한 모든 Threshold에 대해 FRP과 TPR의 비율을 표현
- PR Plot는 정밀도(Precision)과 재현율(Recall)의 관계를 나타내는 곡선

## 해결방안
| **평가 항목**                     | **산출식**                                                                                                             | **설명**                                                                                             |
| ----------------------------- | ------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **Precision**                 | $$\frac{TP}{TP + FP}$$                                                                                              | - 정도<br>- Positive로 예측된 것 중 실제로도 Positive인 경우의 비율                                                  |
| **Accuracy**                  | $$\frac{TP + TN}{TP + FP + FN + TN}$$                                                                               | - 정해율<br>- 전체 예측에서 옳은 예측의 비율                                                                       |
| **Recall**                    | $$\frac{TP}{TP + FN}$$                                                                                              | - 진양성율, Sensitivity, True Positive Rate<br>- 실제로 Positive인 것 중 예측이 Positive로 된 경우의 비율              |
| **Specificity**               | $$\frac{TN}{FP + TN}$$                                                                                              | - 진음성율<br>- 실제로 Negative인 것 중 예측이 Negative로 된 경우의 비율                                               |
| **FP Rate**                   | $$\frac{FP}{FP + TN}$$                                                                                              | - False Alarm Rate<br>- Positive가 아닌데 Positive로 예측된 비율<br>- $1 - \text{specificity}$와 같은 값         |
| **F1 Score**                  | $$2 * \frac{1}{\frac{1}{Precision} + \frac{1}{Recall}}$$<br>$$= 2 * \frac{Precision * Recall}{Precision + Recall}$$ | - Precision과 Recall 사이의 균형을 맞추는 지표<br>- 1에 가까울수록 좋은 모델<br>- 0에 가까울수록 최악의 모델                        |
| **Cohen’s Kappa Coefficient** | $$K = \frac{Accuracy - P(e)}{1 - P(e)}$$                                                                            | - 정확도는 클래스 불균형이 심하면 높은 정확도가 나올 수 있지만 결과로선 의미가 없음<br>- 관측된 일치도와 우연의 일치도 사용<br>- 우연히 맞춘 경우까지 고려하여 보정 |