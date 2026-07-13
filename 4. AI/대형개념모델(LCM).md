#정보관리기술사 #AI #LCM #대형개념모델 #AI/LLM/생성AI #NEW
## 정의
대형개념모델(LCM, Large Concept Models)
- 토큰 단위 제약을 벗어나 Concept(개념)을 의미 단위로 사용해 의미론적 추론을 수행하는 모델(Meta AI)
## 키워드
* SONAR embedding space, Meta AI, Concept, Zero-shot, Diffusion-LCM
## 암기법
* 소프트포: SONAR·PreNet·Transformer·PostNet
## 특징
- 계층적 가독성: 장문 컨텍스트를 문장·개념 단위로 처리
- 연산 효율성: Transformer 컨텍스트 길이 지수 연산 폭증 완화
- Zero-shot 일반화: 미학습 언어·모달리티에도 강한 일반화
- 모듈 확장성: 개념 인코더·디코더 분리로 멀티모달 간섭 회피
## 목적
- 토큰 기반 LLM의 의미 추론·장문 처리 한계 극복
- 다언어·음성·텍스트 통합 의미 공간에서 유사성·추론 강화
## 구성요소
- SONAR Encoder/Decoder: 문장↔개념 임베딩(텍스트 200언어, 음성 76언어)
- PreNet: 입력 정규화·내부 차원 매핑
- Transformer Decoder: 다음 문장 임베딩 예측
- PostNet: 예측 임베딩 역정규화·출력
- 유형: Base-LCM, Diffusion-based(One-Tower/Two-Tower), Quant-LCM
## 구성도
```
문장/음성 → SONAR Encoder → PreNet → Transformer Decoder → PostNet → SONAR Decoder
                              (Concept Embedding Space)
```
## 연관 토픽
- [[LLM]] - 토큰 기반 대형 언어모델
- [[트랜스포머(Transformer)]] - 어텐션 기반 백본
- [[멀티모달(Multi Modal) AI]] - 다중 모달 학습
- [[대규모 언어 모델(LLM) 성능 향상 기술]] - LLM 고도화
