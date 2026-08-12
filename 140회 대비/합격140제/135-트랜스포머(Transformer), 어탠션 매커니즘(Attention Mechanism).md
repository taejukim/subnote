#정보관리기술사 #AI #트랜스포머 #어텐션메커니즘
## 정의
트랜스포머(Transformer)
- 셀프 어텐션(Self-Attention) 구조만으로 순차 데이터 내 관계를 추적해 맥락·의미를 학습하는 인코더-디코더 신경망
- RNN·LSTM의 병렬화 불가·기울기소실 한계를 극복하며 2017년 등장
## 키워드
* Self-Attention, Multi-head Attention, Positional Encoding, Encoder-Decoder, Masked Self-Attention
## 암기법
* 위인디출: 위치인코딩·인코더·디코더·출력층(트랜스포머 4대 구성)
## 특징
- 병렬처리성: RNN과 달리 입력 토큰을 동시에 병렬 처리
- 위치보존성: Positional Encoding으로 순서 정보 보완
- 다중어텐션성: Multi-head로 여러 관점의 유사도를 동시 계산
- 확장범용성: BERT·GPT·T5·ViT 등 다양한 파생모델의 기반
## 목적
- RNN 계열 모델의 순차처리 병목·기울기소실 문제 해결
- 장거리 의존관계를 효율적으로 학습하는 범용 아키텍처 제공
## 구성요소
- Positional Encoding: 사인·코사인 함수로 단어 위치정보 부여
- 인코더: Multi-head Self-Attention + Feed Forward NN, 6개 층 반복
- 디코더: Masked Self-Attention + Encoder-Decoder Attention + FFN
- 출력층: Linear Layer + Softmax로 다음 단어 확률 예측
## 구성도
```
[입력+Positional Encoding] → [인코더: Self-Attention→FFN] x N
                                          ↓ (Key, Value)
[출력 임베딩] → [디코더: Masked Self-Attention→Enc-Dec Attention→FFN] x N
                                          ↓
                              [Linear·Softmax → 출력 단어]
```
## 연관 토픽
- [[BERT]] - 인코더 기반 사전학습 언어모델
- [[GPT]] - 디코더 기반 생성형 언어모델
- [[ViT(Vision Transformer)]] - 이미지 처리용 트랜스포머
- [[VLA(Vision-Language-Action) 모델]] - 트랜스포머 기반 피지컬 AI 모델
