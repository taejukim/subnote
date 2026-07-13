#정보관리기술사 #디지털서비스 #CRIO #컨테이너런타임
## 정의
CRI-O
- Kubernetes의 CRI(Container Runtime Interface) 사양에 맞춰 설계된 경량 OCI 컨테이너 런타임
- Docker 의존을 제거하고 K8s 전용으로 최적화된 런타임 구현체
## 키워드
* Kubernetes, CRI, OCI, runc, Pod, Containerd 비교
## 암기법
* 경표쿠: 경량·표준·쿠버네티스전용
## 특징
- 경량성: 불필요한 기능 제거로 가벼움
- 표준 준수성: OCI·CRI 표준 호환
- K8s 최적화: K8s 전용 설계
- 보안성: 최소 권한·자체 컴포넌트 분리
## 목적
- K8s 환경의 단순·안정 컨테이너 런타임 제공
- Docker 의존 제거와 컨테이너 운영 최적화
## 구성요소
- CRI: K8s ↔ 런타임 인터페이스
- runc/crun: OCI 런타임
- conmon: 컨테이너 모니터링
- 이미지 관리: Skopeo, Buildah
- 비교: Docker(데몬), containerd(범용 런타임), CRI-O(K8s 전용)
## 구성도
```
[Kubelet] ── CRI ── [CRI-O] ── runc/crun ── 컨테이너
                       ↓
                conmon (모니터링)
```
## 연관 토픽
- [[쿠버네티스(Kubernetes)]] - K8s 일반
- [[컨테이너(Container)]] - 컨테이너 일반
- [[도커(Docker)]] - Docker
- [[클라우드 네이티브]] - 클라우드 네이티브
