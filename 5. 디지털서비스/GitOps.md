#정보관리기술사 #디지털서비스 #GitOps #DevOps
## 정의
GitOps
- Git 저장소를 단일 진실 공급원(SSoT)으로 사용하여 인프라·애플리케이션 배포와 운영을 선언적으로 자동화하는 운영 방식
- Pull-based 배포·자동 동기화·자동 복구를 특징으로 하는 차세대 DevOps 패러다임
## 키워드
* Git SSoT, Declarative, Pull-based, Argo CD, Flux, Reconciliation
## 암기법
* 선풀자감: 선언적·풀기반·자동복구·감사가능
## 특징
- 선언성: 원하는 상태를 코드로 선언
- Pull 기반: Operator가 변경을 감지·적용
- 자동 복구성: 드리프트 감지·자동 회복
- 감사 가능성: 모든 변경이 Git 이력으로 추적
## 목적
- 운영 자동화와 신뢰성 확보
- 변경 추적성·감사·롤백 용이성 강화
## 구성요소
- 핵심 원칙: 선언적, 버전 관리, Pull 기반, 자동 동기화
- 도구: Argo CD, Flux, Jenkins X
- 워크플로우: Git PR → Merge → Operator Pull → 클러스터 동기화
- 보안: SOPS, Sealed Secrets, OPA Gatekeeper
- 운영: 드리프트 감지, 자동 Reconciliation
## 구성도
```
[개발자] → Git Push → [Git Repo (SSoT)]
                           ↑ PR/Merge
[GitOps Operator (Argo CD/Flux)] ── Pull/감지 ── 적용
                                                 ↓
                                          [K8s 클러스터]
                                          드리프트 감지·자동 복구
```
## 연관 토픽
- [[DevOps]] - DevOps 협업
- [[NoOps]] - 운영 추상화
- [[쿠버네티스(Kubernetes)]] - K8s
- [[플랫폼 엔지니어링]] - 플랫폼 엔지니어링
