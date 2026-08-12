#정보관리기술사 #AI #ConstitutionalAI #AIAlignment
## 정의
헌법적 AI(Constitutional AI)
- 사전에 정의된 윤리·안전 원칙(헌법)을 기준으로 AI가 자신의 응답을 스스로 평가·수정하도록 학습하는 AI 정렬 방법론
- Anthropic이 제안한 자기정렬(Self-Alignment) 기반 안전성 확보 기법
## 키워드
* Self-Alignment, Self-Critique, Self-Revision, Constitutional Fine-Tuning, RLHF, Constitutional AI 2.0
## 암기법
* 원자일: 원칙기반·자기평가·일관성(헌법적 AI 핵심 특징)
## 특징
- 원칙기반: 헌법(Constitution)에 근거해 정렬 수행
- 자기정렬: 인간 개입 없이 Self-Critique·Self-Revision 수행
- 사전예방성: 생성 단계부터 유해응답 통제
- 확장성: 평가 인력 증가 없이 자동화 기반 확장 가능
## 목적
- 생성형 AI의 안전성(Safety)과 정렬성(Alignment) 확보
- RLHF의 인간 평가 의존·비용·편차 한계 극복
## 구성요소
- 헌법(원칙): 사전 정의된 윤리·안전 규범 체계
- SFT 단계: 인간 작성 데이터 기반 지도학습
- Self-Critique: 헌법 기준으로 자기 응답 비판
- Self-Revision: 비판 결과 반영한 응답 자기수정
- Constitutional Fine-Tuning: 자기수정 데이터로 재학습
## 구성도
```
[SFT 초기 모델] → [응답 생성] → [헌법 기준 Self-Critique]
                                        ↓
                              [Self-Revision 응답 수정]
                                        ↓
                        [Constitutional Fine-Tuning 재학습]
```
## 연관 토픽
- [[RLHF]] - 인간 피드백 기반 강화학습 정렬 기법
- [[AI Safety]] - 인공지능 안전성 확보 체계
- [[XAI]] - 설명가능 인공지능
- [[AI 거버넌스]] - AI 위험관리·책임성 확보 체계
