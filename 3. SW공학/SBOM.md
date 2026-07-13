#정보관리기술사 #SW공학 #SBOM #공급망보안 #NEW
## 정의
SBOM(Software Bill of Materials)
- SW 컴포넌트·구성 요소를 식별하는 메타데이터와 저작권·라이선스 등 콘텐츠 정보를 담은 공식 SW 자재 명세서
- 의존관계·버전·해시로 공급망 구성요소를 투명하게 관리
## 키워드
* Author, Timestamp, Version, SPDX, CycloneDX, SWID, Component Hash
## 암기법
* 작시공버해유관 / 스사사: 작성자·시각·공급자·버전·해시·UID·관계 / SPDX·CycloneDX·SWID
## 특징
- 명세성: 구성요소·버전·공급자·해시 공식 목록화
- 관계표현: Included-in 등 의존 트리
- 표준형식: SPDX(라이선스)·CycloneDX(보안)·SWID(식별)
- 공급망: 취약 컴포넌트·라이선스 리스크 추적 기반
## 목적
- SW 구성요소·라이선스·무결성 정보 표준화
- 공급망 보안·컴플라이언스·취약점 대응 가속
## 구성요소
- Baseline: Author Name, Timestamp(ISO8601), Supplier, Component Name, Version String, Component Hash, Unique ID, Relationship
- 형식: SPDX(Linux Foundation), CycloneDX(OWASP), SWID
- 관계예: Compression⊂Browser⊂Application, Buffer⊂Application
## 구성도
```
[Carol Compression]⊂[Bob Browser]┐
                                 ├⊂[Acme Application]
              [Bingo Buffer]─────┘
속성: Author·Time·Supplier·Name·Ver·Hash·UID·Relation
형식: SPDX | CycloneDX | SWID
```
## 연관 토픽
- [[오픈소스 SW 보안위협]] - OSS 보안
- [[오픈소스 거버넌스]] - OSS 거버넌스
- [[오픈소스 License 분류]] - 라이선스
- [[오픈소스 소프트웨어]] - OSS 개념
