#정보관리기술사 #AI #PEFT #AI/LLM/생성AI #NEW
## 정의
PEFT(Parameter-Efficient Fine-Tuning)
- 사전학습 모델의 전체 파라미터를 업데이트하지 않고 일부만 조정해, 적은 자원으로 효과적 파인튜닝을 실현하는 방법
## 키워드
* 일부만 파인튜닝, Adapter, Prefix Tuning, LoRA, Parallel Adapter
## 암기법
* 어프Lo병스: Adapter·Prefix·LoRA·Parallel Adapter·Scaled PA
## 특징
- 파라미터 효율성: 전체 대비 수~몇 %만 업데이트
- 적용 선택성: 모듈·태스크별 기법 선택 가능
- 비용 최소화: 자원·시간 절감하며 커스터마이징
- 구조 다양성: 병목 삽입·프리픽스·저랭크·병렬 스케일 등
## 목적
- Full Fine-Tuning 수준의 성능을 낮은 비용으로 달성
- 거대 모델의 도메인·태스크 적응 효율화
## 구성요소
- Adapter: PLM 중간 작은 신경망(Bottleneck) 삽입
- Prefix Tuning: 입력 앞단 학습 가능 벡터 + Softmax/게이팅
- LoRA: 저랭크 행렬 추가 학습·Scaling
- Parallel Adapter: PLM과 병렬 ReLU 어댑터 합산
- Scaled PA: Parallel Adapter에 Scaling 추가
## 구성도
```
Transformer: Attention → FFN → [Adapter] → LN → FFN → [Adapter]
Adapter: Down project → Nonlinearity → Up project
```
## 연관 토픽
- [[LoRA]] - 저랭크 어댑터
- [[프롬프트 튜닝]] - Soft Prompt PEFT
- [[파인튜닝(Fine-tuning)]] - Full Fine-Tuning
- [[지식 증류(Knowledge Distillation)]] - 모델 압축
