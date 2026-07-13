#정보관리기술사 #디지털서비스 #CNAPP #클라우드보안
## 정의
CNAPP(Cloud-Native Application Protection Platform)
- 개발·운영 전반에 걸쳐 클라우드 네이티브 애플리케이션을 보호하고 보안을 강화하는 통합 보안 플랫폼
- CSPM·CWPP·CIEM 등 분리된 클라우드 보안 도구를 통합한 차세대 보안 플랫폼
## 키워드
* CSPM, CWPP, CIEM, IaC Scan, Shift-Left, Runtime Protection
## 암기법
* 개식모대: 개발·식별·모니터링·대응
## 특징
- 통합성: 빌드·배포·런타임 단일 플랫폼
- 라이프사이클 보호: Shift-Left + Runtime
- 가시성: 자산·구성·권한·취약점 통합 가시화
- 자동화성: 정책 기반 자동 진단·대응
## 목적
- 분리된 클라우드 보안 도구의 사일로 해소
- 개발~운영 전 단계 클라우드 자산 보호
## 구성요소
- CSPM: 구성 오류 탐지·정책 준수
- CWPP: 워크로드 보호(컨테이너·VM)
- CIEM: 권한·자격 관리
- IaC Scan: 코드 단계 보안 검증
- Runtime Protection: 실행 단계 위협 탐지
- Vulnerability Mgmt: 취약점 통합 관리
## 구성도
```
[Code/IaC] → [Build] → [Deploy] → [Runtime]
   ↑           ↑         ↑          ↑
  IaC Scan   CSPM    CIEM·CWPP   Runtime Defense
   └─────────── 통합 가시성·정책·대응 ───────────┘
```
## 연관 토픽
- [[CWPP&CSPM]] - 클라우드 워크로드/구성 보호
- [[클라우드 네이티브 보안]] - 클라우드 네이티브 보안
- [[DevSecOps]] - 보안 통합 DevOps
- [[제로 트러스트(Zero Trust)]] - 제로 트러스트
