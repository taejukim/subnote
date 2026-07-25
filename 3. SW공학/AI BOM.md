#정보관리기술사 #SW공학 #AIBOM #SBOM #NEW
## 정의
AI BOM(Artificial Intelligence Bill of Materials)
- AI 시스템을 구성하는 데이터·모델·SW 라이브러리·인프라 등 모든 구성요소를 체계적으로 목록화·추적하는 문서
## 키워드
* Model Card, Datasheet, SBOM, CycloneDX, SPDX, NVD/CVE
## 암기법
* 모데이터알: 모델·데이터·라이브러리·알고리즘
## 특징
- 4분류: 모델 명세, 데이터 명세, 라이브러리, 알고리즘
- CycloneDX v1.5 ML-BOM, Hugging Face Model Cards
- SBOM 대비: AI 모델·데이터·편향·적대적 공격
## 목적
- AI 구성요소 투명성·공급망 보안
- EU AI Act·NIST AI RMF 대응
## 구성요소
- Model: Model Card(목적·성능·한계)
- Data: Datasheet(출처·편향)
- Linkage: SBOM 통합(CycloneDX/SPDX)
- Security: NVD/CVE 취약점 모니터링
## 구성도
```
Model Card + Datasheet + Library + Algorithm → AI BOM ↔ SBOM
```
## 연관 토픽
- [[SBOM]] - SW BOM
- [[Secure SDLC]] - 개발 보안
- [[AI RMF]] - AI 리스크
