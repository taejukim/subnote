#정보관리기술사 #데이터베이스 #DataAsAProduct #DaaP
## 정의
Data as a Product(DaaP)
- 데이터를 독립적인 제품으로 관리하는 데이터 거버넌스 및 아키텍처 패러다임
- 도메인 책임자(Data Product Owner) 중심으로 데이터 품질·접근성·신뢰성을 제품처럼 운영
## 키워드
* Data Mesh, Data Fabric, Data Product Owner, 데이터 카탈로그, API 기반 서비스
## 암기법
* 조사기품: 조직·사용자·기술운영·품질보안
## 특징
- 제품화성: 데이터를 제품처럼 SLA·OKR 관리
- 도메인 책임성: 도메인별 Data Product Owner
- 사용자 중심성: Consumer 친화적 접근·검색
- 자동화성: 파이프라인·API 기반 서비스 제공
## 목적
- 부서 간 데이터 사일로 제거와 활용성 극대화
- 고객 중심 데이터 제공·품질·지속 가능성 확보
## 구성요소
- 배경 기술: Data Mesh, Data Fabric, Cloud Native, 데이터 카탈로그, ETL/ELT 자동화, API 기반 서비스
- 조직: Data Product Owner, 거버넌스 체계, 도메인 운영 기반 구조
- 사용자: Data Consumer, 데이터 카탈로그, 검색 기능, 사용자 피드백·만족도
- 기술 운영: 자동화 파이프라인, API 기반 서비스, 모니터링·로깅
- 품질·보안: 품질 관리 체계, 메타데이터·데이터 리니지, 보안·접근 제어
- 요구사항 - 조직: 도메인 책임, 거버넌스 준수, 역할 기반 운영
- 요구사항 - 사용자: 사용자 중심 설계, 접근성·탐색성, 피드백 수용
- 요구사항 - 기술 운영: 표준화·상호 운용성, 서비스화, 확장성
- 요구사항 - 품질·보안: 지속 개선, SLA·모니터링, 규제 준수
- Data Product 비교: 거버넌스 패러다임 vs 산출물·서비스 단위
## 구성도
```
[Domain A] Data Product (Owner·SLA·Catalog)
[Domain B] Data Product (Owner·SLA·Catalog)   →  Consumer
[Domain C] Data Product (Owner·SLA·Catalog)
                     ↑ 거버넌스·메타데이터·리니지·보안
```
## 연관 토픽
- [[데이터 메시]] - 도메인 분산 데이터 아키텍처
- [[데이터 페브릭]] - 통합 데이터 패브릭
- [[데이터 카탈로그]] - 메타데이터 통합 관리
- [[데이터 거버넌스]] - 데이터 거버넌스
