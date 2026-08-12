#정보관리기술사 #보안 #SecureSDLC #위협모델링
## 정의
Secure SDLC(Secure Software Development Life Cycle)
- 요구사항-설계-구현-테스트-운영 전 단계에 보안 활동을 내재화하여 취약점을 사전 예방하는 개발 방법론
- Shift-Left 전략으로 개발완료 후 패치 비용을 최소화하는 소프트웨어 공급망 보안 핵심 수단
## 키워드
* MS SDL, BSIMM, OWASP SAMM, NIST SSDF, DevSecOps, SBOM, STRIDE, SAST, DAST, 시큐어코딩
## 암기법
* 요설구테운: 요구사항·설계·구현·테스트·운영 단계별 보안 통제 내재화
## 특징
- 전주기 내재화: 개발 全 단계에 보안 활동을 내장해 취약점 사전 차단
- 표준 다양성: MS SDL·OWASP SAMM·BSIMM·NIST SSDF 등 조직 성숙도별 선택 적용
- 자동화 연계: DevSecOps 파이프라인에 SAST·DAST·SCA·SBOM을 자동 통합
- 위협 모델링 중심: 설계 단계 STRIDE 기반 위협 식별로 보안 요구사항 도출
## 목적
- 개발 완료 후 패치 비용 최소화 및 취약점 사전 제거
- 법·규제 준수 및 소프트웨어 공급망 신뢰성 확보
## 구성요소
- 요구사항 단계: 보안요구사항 도출, PIA 수행, 법규 준수기준 정의
- 설계 단계: 보안 아키텍처 설계, STRIDE 위협모델링, 설계 검토
- 구현 단계: 시큐어코딩, SAST(SonarQube 등), SCA(Dependency-Check)
- 테스트 단계: DAST(OWASP ZAP), 모의침투, 퍼징
- 운영 단계: SIEM/SOAR 연동, SBOM 기반 취약점 추적, 사고대응
- STRIDE: Spoofing, Tampering, Repudiation, Information Disclosure, DoS Elevation of Privilege
## 구성도
```
요구사항 → 설계(STRIDE 위협모델링) → 구현(SAST/SCA)
   ↓             ↓                    ↓
보안요구사항   DFD·신뢰경계 식별      시큐어코딩 가이드
   ↓             ↓                    ↓
테스트(DAST/침투) ← 위협평가·대응(DREAD) ← 보안게이트
   ↓
운영(SIEM/SOAR, SBOM) → 지속 모니터링/패치
```
## 연관 토픽
- [[SW 공급망 보안]] - 공급망 전주기 위협 대응
- [[사이버 보안 플랫폼]] - SIEM/SOAR 기반 탐지·대응
- [[제로트러스트]] - 최소권한 기반 보안 아키텍처
- [[APT]] - 시큐어코딩 미비로 인한 표적공격 경로
