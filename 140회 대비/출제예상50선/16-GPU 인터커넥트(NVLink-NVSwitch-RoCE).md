#정보관리기술사 #컴퓨터구조 #GPU인터커넥트 #NVLink
## 정의
GPU 인터커넥트(NVLink/NVSwitch/RoCE)
- 다수 GPU 간 파라미터·그래디언트를 고속 교환하기 위한 GPU 통신 연결 기술
- 대규모 AI 모델 학습의 가능성과 비용효율성을 좌우하는 핵심 인프라 요소
## 키워드
* NVLink, NVSwitch, RoCE, GPU 클러스터, RDMA, All-Reduce
## 암기법
* 고저확계: 고대역폭·저지연직접연결·확장형토폴로지·계층적연결구조
## 특징
- 고대역폭: NVLink는 PCIe 대비 수배~수십배 GPU 간 통신 대역폭 제공
- 저지연 직접연결: GPU-GPU 메모리 직접참조(P2P)로 CPU 개입없이 통신
- 확장형 토폴로지: NVSwitch로 다중 GPU 완전연결(All-to-All) 구성
- 계층적 연결구조: 노드내부 NVLink/NVSwitch, 노드간 InfiniBand/RoCE
## 목적
- 대규모 GPU 클러스터의 학습 성능 병목 해소
- 비용효율적인 확장가능한 AI 인프라 구축
## 구성요소
- NVLink: NVIDIA 독자 포인트투포인트 고속링크, 900GB/s 양방향
- NVSwitch: 다수 NVLink를 중앙스위치로 연결, All-to-All 완전연결
- RoCE v2: 이더넷 위에 RDMA 구현, 표준 인프라 활용으로 비용절감
- InfiniBand: 전용 고속 저지연 패브릭, 최저지연·최고대역폭
- PCIe Gen5/CXL: CPU-GPU 호스트연결, 메모리 확장·풀링
## 구성도
```
[노드 내부] GPU0 ↔ NVLink ↔ GPU1 ↔ NVSwitch(All-to-All) ↔ GPU2~N
                                       │
                          [노드 간] InfiniBand / RoCE v2 (RDMA)
                                       │
                                  GPU 클러스터 확장(Scale-out)
```
## 연관 토픽
- [[피지컬 AI(Physical AI)와 로봇 파운데이션 모델]] - 대규모 모델 학습 인프라
- [[6G와 IMT-2030]] - 초고속 네트워크 기술 연계
- [[AI 데이터센터 특별법]] - 데이터센터 인프라 정책 기반
