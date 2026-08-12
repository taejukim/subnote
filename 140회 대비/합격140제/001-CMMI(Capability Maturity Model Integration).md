#정보관리기술사 #SW공학 #CMMI #프로세스개선
## 정의
CMMI(Capability Maturity Model Integration) v3.0
- 조직의 프로세스 개선을 통해 비용·품질·일정 등을 충족시키며 특정 성숙도 레벨 도달을 위해 수행해야 할 활동을 제시하는 모델
- 8개 도메인 지원과 DevSecOps 영역이 추가된 최신 버전(v3.0)
## 키워드
* Category, Capability Area, Practices, Domain, Maturity Level, DevSecOps
## 암기법
* 카캐프도: 카테고리·캐퍼빌리티영역·프랙티스·도메인 (모델 구성요소)
## 특징
- 계층 구조: Category-Capability Area-Practices 3단계로 구성
- 도메인 확장: DEV,SVC,SPM,SEC,SAF,PPL,Data,VRT 8개 도메인 지원
- 단계적 성숙도: Initial~Optimizing 5단계 성숙도 레벨 제시
- 공통·개별 분리: 17개 공통 Practices와 14개 도메인별 Practices 구분
## 목적
- 조직의 프로세스 성숙도를 체계적으로 진단·개선
- 비용·품질·일정 목표를 충족하는 표준화된 개발 프로세스 확립
## 구성요소
- Category: Doing, Managing, Enabling, Improving 4대 카테고리
- Capability Area: 관련 Practice Area들의 묶음(12개 영역)
- Practices: 공통 17개 + 도메인별 14개 Practice 영역
- Domain: DEV, SVC, SPM, SEC, SAF, PPL, Data, VRT(총 8개)
- Maturity Level: Initial, Managed, Defined, Quantitively Managed, Optimizing
## 구성도
```
[Model CMMI3.0]
   └─ Category (Doing/Managing/Enabling/Improving)
         └─ Capability Area (ENQ, EDP, DMS ...)
               └─ Practices Group (Level1 ... Leveln)
                     └─ Practice 1.1 ~ Practice n.x
                     └─ Informative Material (Context Specific)
```
## 연관 토픽
- [[SW-CMM]] - CMMI의 전신 소프트웨어 성숙도 모델
- [[ISO/IEC 15504(SPICE)]] - 국제 프로세스 심사 표준
- [[프로세스 성숙도 모델]] - 조직 역량 단계적 평가 개념
- [[DevSecOps]] - CMMI v3.0에 신규 반영된 보안 내재화 개발체계
