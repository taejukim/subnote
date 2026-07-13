#정보관리기술사 #컴퓨터구조 #TPU #AI가속기
## 정의
TPU(Tensor Processing Unit)
- 구글이 딥러닝 핵심인 행렬 연산을 가속하기 위해 독자 개발한 AI 전용 주문형 반도체(ASIC)
- 학습·추론 효율을 극대화한 텐서 연산 특화 가속기
## 키워드
* Systolic Array, Tensor, MXU, HBM, TensorFlow, JAX, Edge TPU
## 암기법
* 전시효: 전문성·시스톨릭·효율성
## 특징
- 전문성: 딥러닝 행렬 연산에 특화
- 효율성: 불필요한 제어 제거로 전력·공간 절약
- Systolic Array: 격자형 연산 유닛 동시 처리
- 최적화 환경: TensorFlow·JAX 생태계와 강결합
## 목적
- 초대형 딥러닝 모델 학습·추론 가속
- AI 인프라 비용·전력 효율화
## 구성요소
- 핵심 구조: Systolic Array (수만개 연산 유닛 격자 형태 연결)
- 구조 비교: GPU(SIMT, 수천 코어 그룹) vs TPU(Systolic Array, 격자형)
- 작동 원리: 수만 개 연산 유닛 격자 연결로 행렬 곱 일괄 처리
- 주요 용도: 초대형 LLM 학습·추론
- 강점: 효율성, 최적화
- 약점: 딥러닝 외 작업 불가
- 프레임워크: TensorFlow, JAX 최적화
- 연결 구조: 토러스 기반
- 협업 시스템: 시간차 협업(TPU 학습, GPU 서비스), 전처리 구조(GPU 가공 → TPU 학습), 엣지 구조(Edge TPU → GPU 심화 분석)
- GPU 비교: 그래픽·범용 vs 딥러닝 전용, SIMT vs Systolic Array, CUDA 생태계 vs JAX/TF
## 구성도
```
[입력 텐서] → [Systolic Array (MXU)]
   ┌─┬─┬─┬─┐
   ├─┼─┼─┼─┤  ← 행렬 곱 격자 동시 처리
   ├─┼─┼─┼─┤
   └─┴─┴─┴─┘ → [출력 텐서] → 다음 레이어
   HBM (고대역폭 메모리) ↔ MXU
```
## 연관 토픽
- [[GPGPU - CUDA]] - GPU 컴퓨팅 비교
- [[HBM]] - 고대역폭 메모리
- [[뉴로모픽칩(Neuromorphic chip)]] - 뉴로모픽 칩
- [[AI데이터 센터]] - AI 데이터 센터 인프라
