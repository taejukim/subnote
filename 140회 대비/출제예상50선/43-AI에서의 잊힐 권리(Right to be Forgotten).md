#정보관리기술사 #AI #머신언러닝 #잊힐권리
## 정의
AI에서의 잊힐 권리(Right to be Forgotten)
- GDPR 등 법적 삭제권과 머신 언러닝(Machine Unlearning) 기술을 포괄하는 AI 개인정보 권리
- 모델 재학습 없이 특정 데이터의 학습 영향만 제거하려는 기술적 도전 과제
## 키워드
* 기계 언러닝, 데이터 삭제권, SISA, 근사 언러닝, 인증된 언러닝
## 암기법
* 법정근인: 법적삭제권·정확한언러닝(SISA)·근사언러닝·인증된언러닝
## 특징
- 법적 삭제권: GDPR Art.17 등에 근거해 정보주체가 삭제 요청 가능
- 정확한 언러닝(SISA): 데이터 제거 후 재학습, 완전한 망각 보장
- 근사 언러닝: 영향력 함수·기울기 업데이트로 재학습 없이 망각 근사
- 인증된 언러닝: Membership Inference Test로 삭제 완료 여부 검증
## 목적
- 개인정보보호 규제(GDPR 등) 준수를 위한 AI 학습 데이터 삭제권 보장
- 삭제 이행 여부를 통계적으로 검증 가능한 신뢰성 확보
## 구성요소
- 법적 삭제권: GDPR Art.17·개인정보보호법 기반 삭제 요청 권리
- SISA(Sliced, Isolated, Sliced, Aggregated): 샤딩 기반 효율적 정확 언러닝
- 근사 언러닝: Influence Function·Gradient Ascent로 영향 제거 근사
- 인증된 언러닝: Membership Inference Test로 제거 검증
- 데이터 리니지·체크포인트: 삭제 요청 추적, 버전별 롤백 관리
## 구성도
```
[삭제 요청(GDPR Art.17)] → [SISA 샤드 식별] → [해당 샤드만 재학습] → [Membership Inference 검증]
                    ↘ (대규모 모델) 근사 언러닝(Gradient Ascent) → 완전성 낮음
```
## 연관 토픽
- [[GDPR]] - EU 개인정보보호 규정
- [[차분 프라이버시]] - 사전 예방적 프라이버시 보존 학습
- [[모델 편집(Model Editing)]] - 특정 사실 수정 기법
- [[AI 윤리]] - AI 개발·운영의 윤리적 원칙
