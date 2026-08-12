#정보관리기술사 #SW공학 #GitOps #IaC
## 정의
깃옵스(GitOps)
- Git을 단일 진실 저장소(SSoT)로 활용해 애플리케이션·인프라 목표상태를 선언적으로 관리하는 운영모델
- 자동 동기화(Reconciliation)로 운영환경을 Git 상태와 지속 일치시키는 클라우드 네이티브 모델
## 키워드
* Single Source of Truth, Declarative Configuration, Reconciliation Loop, ArgoCD, FluxCD, IaC
## 암기법
* 형자운: 형상관리·자동동기화·운영안정성 (GitOps 3대 특징)
## 특징
- 단일 진실 저장소: Git으로 구성정보를 통합 관리
- Pull 기반 배포: 운영환경이 Git 상태를 지속적으로 당겨와 동기화
- 선언적 관리: 목표상태(Desired State)를 코드로 선언
- 감사추적성: 변경이력 추적과 신속한 롤백 지원
## 목적
- IaC를 애플리케이션 운영까지 확장해 배포 자동화를 실현
- 변경이력 추적과 신속한 장애복구로 운영 안정성 확보
## 구성요소
- 형상관리: Git(버전관리, 변경이력 추적)
- 배포자동화: ArgoCD, FluxCD(Reconciliation)
- 인프라관리: Terraform 등 IaC
- 컨테이너 플랫폼: Kubernetes(선언적 배포)
- CI/CD: Jenkins, GitHub Actions
## 구성도
```
[개발자 Commit/Push] → [PR 검증] → [Git Repository(SSoT)]
                                          ↓
                          [ArgoCD/FluxCD: Reconciliation]
                                          ↓
                       [Kubernetes 운영환경: 목표상태 유지]
```
## 연관 토픽
- [[IaC]] - 인프라를 코드로 관리하는 기반 기술
- [[DevOps]] - GitOps가 확장·구체화한 상위 운영 문화
- [[Kubernetes]] - GitOps의 대표적 배포 대상 플랫폼
- [[CI/CD]] - 빌드·테스트·배포 자동화 파이프라인
