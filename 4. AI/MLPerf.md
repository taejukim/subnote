#정보관리기술사 #AI #MLPerf #AI/AI_평가/테스트 #NEW
## 정의
MLPerf
- AI 하드웨어·소프트웨어의 학습(Training) 및 추론(Inference) 성능을 다양한 조건에서 평가하는 벤치마크
## 키워드
* Training, Inference, CLOSED 방식, OPEN 방식
## 암기법
* 학추 / 훈처 추정처: 학습·추론 / 훈련시간·처리량·추론속도·정확도·처리량
## 특징
- 학습 평가: Time to Train으로 최단 학습 시간 경쟁
- 추론 평가: Latency·Accuracy·Throughput 트레이드오프
- CLOSED/OPEN: 모델·데이터 고정 경쟁 vs 자유 설정 경쟁
- 과업 다양성: 분류·탐지·음성·NLP·추천·강화학습
## 목적
- AI 시스템 학습·추론 성능의 공정·비교 가능한 측정
- 하드웨어·소프트웨어 스택 최적화 지표 제공
## 구성요소
- 학습지표: 훈련시간, 처리량
- 추론지표: 추론속도, 정확도, 처리량
- 벤치마크: 이미지분류, 객체탐지, 음성인식, NLP, 추천, 강화학습
- CLOSED: 과업·모델·데이터 고정 후 도달시간 경쟁
- OPEN: CLOSED 외 항목 자유 설정
## 구성도
```
MLPerf
 ├─ Training: Time to Train (min)
 └─ Inference: Latency ↔ Accuracy (Throughput)
    CLOSED(고정) / OPEN(자유)
```
## 연관 토픽
- [[AI 시스템 테스트]] - AI 테스트 일반
- [[ISO-IEC TS 42119-2]] - AI 테스트 표준
- [[MLOps]] - 학습·배포 운영
- [[고영향 인공지능 평가]] - 고영향 AI 평가
