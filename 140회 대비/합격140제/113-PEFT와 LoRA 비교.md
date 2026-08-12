#정보관리기술사 #AI #PEFT #LoRA
## 정의
PEFT(Parameter-Efficient Fine-Tuning) & LoRA(Low-Rank Adaptation)
- PEFT는 전체 파라미터를 갱신하지 않고 일부만 조정해 적은 자원으로 파인튜닝하는 기법의 통칭
- LoRA는 파라미터 행렬을 저랭크 분해해 적은 추가 파라미터만 학습하는 대표적 PEFT 기법
## 키워드
* Adapter, Prefix Tuning, 저랭크 분해, Scaling, Parallel Adapter
## 암기법
* 범대적파: 범위·대표기법·적용방식·파라미터효율(PEFT-LoRA 비교기준)
## 특징
- 범위 차이: PEFT는 파인튜닝 기법 통칭, LoRA는 그 대표적 적용 방법
- 적용방식: PEFT는 일부모듈 학습, LoRA는 저랭크 행렬만 학습
- 파라미터 효율성: LoRA는 추가 파라미터를 극소화해 메모리 효율 극대화
- 확장성: PEFT는 다양한 모델에 선택적 적용, LoRA는 트랜스포머 계열에 최적화
## 목적
- 비용·자원·시간을 최소화하면서 LLM을 특정 도메인에 커스터마이징
- 대형 사전학습모델(PLM)을 최소 자원으로 효율적으로 적응시킴
## 구성요소
- Adapter: PLM 중간 Bottleneck 신경망 삽입 후 원래 흐름과 결합
- Prefix Tuning: 입력 앞단 학습가능 벡터 추가, Softmax로 영향 조절
- LoRA: PLM 가중치 대신 저랭크 행렬 추가 학습, Scaling으로 영향 조정
- Parallel/Scaled Adapter: PLM 경로와 병렬 연결, 스케일 조정으로 미세 제어
## 구성도
```
[PLM 파라미터(고정)]
     ├─ Adapter(Bottleneck 삽입)
     ├─ Prefix Tuning(입력 벡터 추가)
     ├─ LoRA(저랭크 행렬 A×B 추가, Scaling)
     └─ Parallel/Scaled Adapter(병렬 연결)
              ↓
        경량 파인튜닝 출력
```
## 연관 토픽
- [[파인튜닝]] - PEFT가 대체하는 전체 재학습 방식
- [[프롬프트 튜닝]] - 또 다른 경량 커스터마이징 기법
- [[전이학습]] - PEFT/LoRA의 기반 학습 원리
- [[모델 경량화]] - PEFT의 상위 목적 개념
