#정보관리기술사 #AI #TestTimeCompute #TTC #AI/LLM/생성AI #NEW
## 정의
Test-Time Compute(TTC, 테스트타임 컴퓨팅)
- AI 모델이 추론(Inference) 단계에서 사용하는 연산 자원·시간의 총량
- 문제 난이도에 따라 추론 시 추가 연산으로 품질 향상
## 키워드
* TTA, TTR, TENT, CoT, Self-Consistency, Best-of-N, STaR, MCTS, ToT
## 암기법
* 적재: Adaptation(TTA)·Revision(TTR)
## 특징
- System 1(즉답 LLM) vs System 2(TTC 기반 단계 추론)
- TTA: 테스트 환경 파라미터·입력 변환 적응
- TTR: 자기 검증·수정으로 정확도 향상
## 목적
- 가성비 향상: 난이도별 연산 배분
- 할루시네이션 감소: 중간 추론·검증
## 구성요소
- TTA: TENT(Entropy·BN), Prompt Adaptation
- TTR: CoT, Self-Consistency, Best-of-N, Weighted Best-of-N, STaR, MCTS·ToT
## 구성도
```
Input → Inference → [TTC: CoT/탐색/자기검증] → Verify → Output
```
## 연관 토픽
- [[테스트 타임 스케일링]] - TTS
- [[COT(Chain of Thought)]] - CoT
- [[대규모 언어 모델(LLM) 성능 향상 기술]] - LLM 고도화
