#정보관리기술사 #AI #어텐션메커니즘 #AI/LLM/생성AI
## 정의
- 디코더에서 출력단어를 예측하는 매 시점(Time Step)마다, 인코더에서 전체 입력문장의 예측해야 할 단어와 연관있는 입력 단어 부분을 집중해 참고 하는 방법
## 키워드
- Q(Query), K(Key), V(Value), Attention Score, Attention Distribution, Attention Value
## 암기법
- 어텐션함수
	- 쿼키벨어 (쿼리, 키, 벨류, 어텐션 값)
- 어텐션 메커니즘 예측과정
	- 스분값연예 (어텐션 스코어, 어텐션 분포, 어텐션 값, 연결, 최종 예측)
## 어텐션 함수
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260320225705.png|500]]
1. 쿼리(Query)에 대해 모든 키(Key)의 유사도를 각각 구한다.
2. 유사도를 키와 매핑되어 있는 각각의 값(Value)에 반영
3. 유사도가 반영된 값을 모두 더해서 리턴
4. 어텐션 값(Attention Value)를 반환

## 어텐션 메커니즘 예측 과정
| **과정**                                 | **설명**                                                                                                                                                                                             |
| -------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **어텐션 스코어**<br>(Attention Score)       | - 디코더에서 새로운 단어를 예측하기 위해, 디코더의 hidden state와 인코더의 hidden states들이 얼마나 유사한지를 판단하는 점수<br>$$score(s_t, h_i) = s_t^T h_i$$                                                                              |
| **어텐션 분포**<br>(Attention Distribution) | - softmax를 활용해 Attention Distribution을 구함<br>- 입력 시퀀스에 대응하는 hidden states를 활용해 Attention scores를 구하고, 어텐션 분포 벡터를 얻게 됨<br>- 이 때 각각의 값을 Attention Weight(어텐션 가중치)라고 함<br>$$\alpha^t = softmax(e^t)$$ |
| **어텐션 값**<br>(Attention Value)         | - Attention Weight와 각 hidden state를 통해 최종적인 Attention value를 얻음<br>- 어텐션 값은 인코더의 맥락을 포함하고 있기 때문에 Context Vector(맥락 벡터) 라고도 불림<br>$$a_t = \sum_{i=1}^{N} \alpha_i^t h_i$$                           |
| **연결**<br>(concatenate)                | - 어텐션 값과 decoder의 hidden state 값을 연결<br>- decoder의 hidden state의 정보 외에도 encoder에서의 모든 hidden state를 고려한 정보 또한 포함하고 있기 때문에, sequence가 길어지더라도 정보를 크게 잃지 않음                                           |
| **최종값 예측**                             | $$\hat{y}_t = Softmax(W_y \tilde{s}_t + b_y)$$                                                                                                                                                     |
