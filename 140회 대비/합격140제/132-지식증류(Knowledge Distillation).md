#정보관리기술사 #AI #지식증류 #모델경량화
## 정의
지식증류(Knowledge Distillation)
- 고성능 대형 교사모델(Teacher)의 출력분포·내부표현·추론패턴을 경량 학생모델(Student)에 전달하는 모델 압축 기법
- Pruning·Quantization·PEFT와 함께 LLM의 학습·추론 비용을 절감하는 경량화 전략
## 키워드
* Teacher-Student, Soft Target, Pruning, Quantization, Transfer Learning, LoRA, QLoRA, PEFT
## 암기법
* 응특관추: 응답기반·특징기반·관계기반·추론기반(지식전이 4대 메커니즘)
## 특징
- 지식전이성: Soft Target으로 교사의 일반화 지식을 학생에 전달
- 경량화성: 가지치기·양자화로 파라미터·연산량 축소
- 자원효율성: 전이학습·PEFT로 적은 데이터·연산으로 미세조정
- 성능균형성: 모델 크기를 줄이면서 유사 성능 확보
## 목적
- LLM의 학습·추론 비용 및 에너지 소모 문제 해결
- 경량 모델로 대형 모델 수준의 성능·일반화 능력 확보
## 구성요소
- 지식증류: 응답기반(Logit), 특징기반(Feature), 관계기반(Relation), 추론기반(Reasoning) 증류
- 가지치기(Pruning): Weight/Channel/Layer 단위로 불필요 파라미터 제거
- 양자화(Quantization): FP32→INT8/INT4로 정밀도 변환, PTQ/QAT
- 전이학습·PEFT: Full Fine-tuning, LoRA, QLoRA, Adapter, Prefix Tuning
## 구성도
```
[대형 교사모델] --Soft Target/지식전이--> [경량 학생모델]
                                              ↓
                        [Pruning·Quantization: 구조·정밀도 압축]
                                              ↓
                        [전이학습·PEFT: 도메인 미세조정] → [경량 고효율 모델]
```
## 연관 토픽
- [[sLLM]] - 경량화된 소형 언어모델
- [[LoRA]] - 저랭크 분해 기반 파라미터 효율적 미세조정
- [[AI 토큰 이코노미]] - 토큰 처리비용 최적화 생태계
- [[MoE(Mixture of Experts)]] - 부분 전문가 선택적 활성화 구조
