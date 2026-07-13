#정보관리기술사 #AI #LoRA #PEFT
## 정의
LoRA(Low-Rank Adaptation)
- 초거대 AI 모델의 전체 파라미터를 동결하고 저차원 행렬만 학습하여 효율적으로 파인튜닝하는 기법
- 학습 비용·메모리를 1% 이하로 절감하는 PEFT(Parameter-Efficient Fine-Tuning) 대표 기법
## 키워드
* Low-Rank, QLoRA, PEFT, Adapter, Parameter Freezing, 파인튜닝
## 암기법
* 분고미통: 분해·고정·미세조정·통합
## 특징
- 효율성: 1% 이하 파라미터로 미세 조정
- 경량성: 메모리·연산 비용 대폭 감소
- 모듈성: 어댑터 단위로 교체·재사용
- 성능 보존성: Full Fine-Tuning과 유사 수준
## 목적
- 거대 모델 파인튜닝의 비용·시간 최소화
- 멀티 도메인·태스크 어댑터 운영 효율화
## 구성요소
- Parameter 분해: 가중치 행렬 W를 저랭크 A·B로 분해
- 학습 대상 설정: 기존 모델 가중치 고정, A·B만 학습
- 미세 조정 수행: 저차원 행렬 학습으로 적응
- 추론 시 통합: 원본 가중치 + 어댑터 결합
- 변형: QLoRA(양자화), DoRA, AdaLoRA
- PEFT 비교: Prompt Tuning, Prefix Tuning, Adapter Tuning
## 구성도
```
입력 → [기존 가중치 W (고정)] + [A · B (학습 가능, 저랭크 r)] → 출력
                                ↑ 학습 파라미터 1% 이하
```
## 연관 토픽
- [[파인튜닝(Fine-tuning)]] - 모델 적응 일반
- [[도메인 특화 언어 모델]] - 산업 특화 LLM
- [[지식 증류(Knowledge Distillation)]] - 모델 압축
- [[sLLM]] - 소형 LLM
