#정보관리기술사 #SW공학 #GitOps #쿠버네티스
## 정의
깃옵스(GitOps)
- Git을 단일 진실 공급원(SSOT)으로 선언적 설정·Pull 배포·지속 조정을 수행하는 인프라 운영 방식
- 쿠버네티스 등 클라우드 네이티브 환경의 배포 신뢰성·보안을 높이는 표준 운영 모델
## 키워드
* 선언적 설정, Pull 기반 배포, 지속적 조정(Reconciliation), 드리프트 탐지, ArgoCD/Flux
## 암기법
* 선풀지드: 선언적 구성·Pull기반 배포·지속적 조정·드리프트 탐지
## 특징
- 선언적 구성: 인프라·앱의 원하는 상태를 Git에 선언
- Pull 기반 자동 배포: 에이전트가 변경 감지 후 스스로 끌어와 적용
- 지속적 조정: 실제 상태와 선언 상태를 비교해 자동 복원
- 드리프트 탐지·자가복구: 수동 변경·불일치 발견 시 자동 원복
## 목적
- 수동 배포·Push 방식의 보안 취약점과 상태 불일치 해소
- Git 이력 기반 완전한 감사·롤백 가능한 배포 체계 구축
## 구성요소
- Git 저장소: 선언적 설정(YAML·Helm·Kustomize)의 SSOT
- GitOps 컨트롤러: ArgoCD·Flux CD 등 Pull·동기화 에이전트
- 쿠버네티스 클러스터: 실제 상태(Actual State) 유지 대상
- Reconciler: Desired State와 Actual State 지속 비교·복원
- Policy Engine: OPA·Kyverno로 정책 검증 및 드리프트 방지
## 구성도
```
[Git Repo(Desired State)] → Pull → [GitOps 컨트롤러(ArgoCD/Flux)] → Sync/Apply → [K8s 클러스터(Actual State)]
                                        ↑── 지속적 비교·드리프트 탐지·자동 복원 ──┘
```
## 연관 토픽
- [[CI/CD]] - 지속적 통합·배포 파이프라인
- [[쿠버네티스]] - 컨테이너 오케스트레이션 플랫폼
- [[IaC(Infrastructure as Code)]] - 코드 기반 인프라 관리
- [[DevSecOps]] - 보안 내재화 개발운영
