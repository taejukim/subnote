#정보관리기술사 #디지털서비스 #LXC #리눅스컨테이너
## 정의
LXC(Linux Containers)
- 단일 Linux 호스트 위에서 시스템 컨테이너(OS 수준 가상화)를 실행하는 컨테이너 가상화 기술
- Cgroups·Namespaces 기반 경량 가상화로 OS 환경을 격리 제공
## 키워드
* OS Container, Cgroups, Namespaces, LXD, Docker 비교, 시스템 컨테이너
## 암기법
* 격경공: 격리·경량·공유커널
## 특징
- 시스템 컨테이너성: 전체 OS 환경 제공
- 경량성: 호스트 커널 공유로 부팅 빠름
- 격리성: Namespaces로 프로세스·네트워크 격리
- 자원 제한성: Cgroups로 CPU·메모리 제한
## 목적
- 가상머신 대비 경량 OS 격리 환경 제공
- 다중 OS 환경 운영의 자원 효율화
## 구성요소
- Cgroups: 자원 할당·제한
- Namespaces: 프로세스·NW·파일·UID 격리
- LXC 도구: lxc-create, lxc-start, lxc-stop
- LXD: LXC 상위 관리 데몬
- Docker 비교: LXC(시스템 컨테이너, OS 환경) vs Docker(애플리케이션 컨테이너, 단일 프로세스)
## 구성도
```
[Linux 호스트 커널]
   ├── Namespaces (격리)
   └── Cgroups (자원 제한)
         ├── [LXC 컨테이너 1: OS 환경]
         ├── [LXC 컨테이너 2: OS 환경]
         └── [LXC 컨테이너 N: OS 환경]
```
## 연관 토픽
- [[컨테이너(Container)]] - 컨테이너 일반
- [[도커(Docker)]] - Docker
- [[가상화]] - 가상화 일반
- [[Hypervisor]] - 하이퍼바이저
