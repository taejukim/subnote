#정보관리기술사 #AI #MLOps #AI/LLM/생성AI #NEW
## 정의
MLOps
- 머신러닝 프로세스(데이터 수집·분석·배포)를 자동화하기 위해 DevOps와 결합한 머신러닝 IT 운영 프레임워크
## 키워드
* DevOps, 자동화, CI/CD, Feature Store, Data Drift
## 암기법
* 도파 대학평배: 도구선택·파이프라인·데이터수집·학습·평가·배포
## 특징
- ML+DEV+OPS 융합: Data/Model · Plan/Create/Verify/Package · Release/Configure/Monitor
- 성숙도 단계: Level0 수동 → Level1 ML 파이프라인 → Level2 CI/CD
- 재현성: 모듈화·Feature Store로 단계 재현
- 모니터링: Data Drift 감지·성능 추적
## 목적
- AI 프로젝트 실패 요인(인식 격차·조직문화·시스템 충돌·인력) 완화
- 데이터→학습→배포의 지속적 자동화·운영
## 구성요소
- Level0: 수동 개발·학습·배포, 형상관리 부재
- Level1: 파이프라인 자동화, Feature Store, 도구→구축→수집→학습→평가
- Level2: CI/CD 포함 배포·모니터링·드리프트 대응까지 자동화
## 구성도
```
도구선택 → 파이프라인구축 → 데이터수집 → 학습 → 평가 → 배포
              └────── MLOps Automation ──────┘
     ML(Data/Model) ∩ DEV ∩ OPS (Infinity Loop)
```
## 연관 토픽
- [[LLMOps]] - LLM 특화 운영
- [[모델 드리프트]] - 성능 저하 모니터링
- [[AutoML]] - 자동 모델 탐색
- [[AI Ready Data]] - 학습 준비 데이터
