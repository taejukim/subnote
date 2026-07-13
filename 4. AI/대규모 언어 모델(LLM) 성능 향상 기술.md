#정보관리기술사 #AI #대규모언어모델성능향상기술 #AI/LLM/생성AI
## 정의
- 대규모 언어 모델(LLM)의 추론 능력 부족, 정보의 정확성 문제, 지식의 일관성 유지 어려움 등의 한계를 극복하기 위한 기술

## 키워드
- 추론 능력 강화, RAG, 모델 병합 및 결합, 효율성 및 비용 절감, 멀티 모달 통합

## 암기법
- 주요기법
	- 추R모효멀 (추론 능력 강화, RIG, 모델 병합 및 결함, 효율성 및 비용절감, 멀티모달 통합)
## 주요기법
| **기술 그룹**                                                     | **정의**                                                      | **주요 기법**                                                                                      |
| ------------------------------------------------------------- | ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------- |
| **추론 능력 강화**<br>(Reasoning Enhancement)                       | 모델이 논리적인 사고 과정을 통해 보다 정확하고 신뢰성 있는 응답을 생성하도록 돕는 기술           | - Chain of Thought (CoT)<br>- Tree of Thought (ToT)<br>- Least-to-Most Prompting               |
| **외부 지식 활용 및 정밀 검색**<br>(Retrieval-Augmented Generation, RAG) | 모델이 외부 데이터베이스를 참조하여 최신 정보를 반영하거나 문맥을 보강하여 더 정확한 응답을 생성하는 기술 | - RAG<br>- Knowledge-Intensive NLP                                                             |
| **모델 병합 및 결합**<br>(Merging & Integration)                     | 여러 개의 사전 훈련된 모델을 결합하여 성능을 향상시키거나 특정 태스크에 맞게 조정하는 기술         | - Model Merging via Interpolation<br>- DARE (Drop And REscale)<br>- Evolutionary Model Merging |
| **효율성 및 비용 절감**<br>(Optimization & Efficiency)                | 모델의 계산 비용을 줄이면서도 성능을 유지하거나 향상시키는 기술                         | - Mixture of Experts (MoE)<br>- Sparse Attention<br>- Quantization (양자화)<br>- LoRA             |
| **멀티모달 통합**<br>(Multimodal Integration)                       | 텍스트뿐만 아니라 이미지, 음성, 영상 등을 함께 처리할 수 있도록 확장하는 기술               | - CLIP<br>- Flamingo<br>- BLIP-2                                                               |
## Reasoning 기술 상세
| **Reasoning 종류**                    | **설명**                                          | **대표적인 모델/기법**                      |
| ----------------------------------- | ----------------------------------------------- | ----------------------------------- |
| **사고사슬**<br>(Chain of Thought: CoT) | 답변을 도출하기 전에 중간 추론 과정을 단계별로 서술하여 복잡한 문제를 해결하는 방법 | GPT-3, GPT-4, PaLM                  |
| **디컴포지션**<br>(Decomposition)        | 큰 문제를 여러 개의 하위 문제로 분해하여 단계별로 해결하는 방식            | Least-to-Most Prompting, Self-Ask   |
| **메타-리즌**<br>(Meta-Reasoning)       | 모델이 자신의 추론 과정을 검토하고 수정하여 더 나은 답변을 생성하는 능력       | Self-Reflection, ReAct              |
| **귀납적 추론**<br>(Inductive Reasoning) | 주어진 데이터에서 패턴이나 규칙을 찾아내어 일반화된 결론을 도출하는 방식        | In-Context Learning, Transformer 기반 |
| **상호 추론**<br>(Mutual Reasoning)     | 두 개의 모델이 서로의 추론 과정을 검증하여 더 정확한 답변을 도출하는 방식      | rStar(Microsoft) 모델                 |
