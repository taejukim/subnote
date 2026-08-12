#정보관리기술사 #디지털서비스 #데이터레지던스 #DataResidency
## 정의
데이터 레지던스(Data Residency)
- 기업·개인 데이터를 저장·처리하는 데이터센터·서버 등이 위치한 물리적·지리적 위치
- 데이터 위치에 따른 법률 적용을 통제하기 위한 클라우드 데이터 주권 확보 기법
## 키워드
* Geo-fencing, Policy as Code, KMS, HSM, IAM, PAM, BYOK, MFA
## 암기법
* 규주보: 데이터규제·데이터주권·데이터보안이 등장 배경
## 특징
- 위치통제성: 데이터센터·리전 등 물리적 저장 위치를 통제
- 정책기반성: Policy as Code로 허용 리전·국외이전 정책 자동화
- 암호보호성: KMS·HSM·BYOK로 암호키 관리 및 보호
- 접근통제성: IAM·PAM·MFA로 해외 관리자 접근 제한
## 목적
- 개인정보·금융·의료 등 데이터의 국외 이전 제한 준수
- 자국 데이터에 대한 법적 관할권과 통제권 확보
## 구성요소
- 통제범위: 서비스 데이터(업무·개인정보), 기반 데이터(백업·로그·암호키·AI학습데이터)
- 식별·분류: Data Discovery, Data Classification
- 정책 통제: Geo-fencing, Policy as Code
- 보호 기술: KMS, HSM, BYOK
- 접근 통제: IAM, PAM, MFA
## 구성도
```
[데이터 식별/분류] → [Geo-fencing / Policy as Code 정책 적용]
                              ↓
        [허용 리전 저장] ── KMS/HSM/BYOK(암호보호)
                              ↓
        [IAM/PAM/MFA 접근통제] → 규제 준수 확인
```
## 연관 토픽
- [[데이터 주권]] - 법적 관할권·통제권 개념
- [[클라우드 보안]] - 클라우드 환경 보안 통제
- [[GDPR]] - EU 개인정보보호규정
- [[Zero Trust]] - 신뢰 없는 접근통제 모델
