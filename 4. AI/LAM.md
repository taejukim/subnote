#정보관리기술사 #AI #LAM #LargeActionModel #AI/LLM/생성AI #NEW
## 정의
LAM(Large Action Model)
- LLM의 언어 이해 능력에 실제 행동 수행 능력을 결합해 물리 세계와 상호작용하는 인공지능 모델
## 키워드
* AI Agent, 의도분류, 계층적작업분해, Neuro-symbolic Programming, RLHF
## 암기법
* 입분실: 입력처리·분석(프롬프트)·실행(행동생성)
## 특징
- 행동 생성성: 지시→Action Plan→에이전트 실행
- 폐루프성: Environment Feedback으로 계획 재조정
- 계층 진화성: LLM→LMM→LAM으로 행동·자동화 확장
- 멀티모달성: 음성·이미지 등 통합 인코딩
## 목적
- 복잡한 태스크의 실제 행동 계획·자동화
- 물리·디지털 환경에서의 자율 작업 수행
## 구성요소
- 단계: 입력처리(데이터 수집) → 분석(도메인 특화 프롬프트) → 실행(행동 생성)
- Input: 멀티모달 인코딩, 의도 분류, 동적 컨텍스트 윈도우
- Planning: CoT, 계층적 작업분해, Neuro-symbolic Programming
- Action: API 오케스트레이션, 동적 계획, 원자적 액션 실행
- Feedback: 다차원 평가, Contextual Memory, RLHF
## 구성도
```
INSTRUCTION → QUERY(Examples/Instruction/Info) → LLM → ACTION PLAN
                    ↕ Feedback/Env Info
              Agent → Action → Environment
진화: LLM(텍스트) → LMM(멀티모달) → LAM(행동·자동화)
```
## 연관 토픽
- [[AI Agent]] - 자율 에이전트
- [[에이전틱 AI]] - 목표 자율 수행
- [[VLA 모델]] - Vision-Language-Action
- [[피지컬 AI(Physical AI)]] - 물리 세계 AI
