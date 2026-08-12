#정보관리기술사 #디지털서비스 #AIFactory #가속컴퓨팅
## 정의
AI Factory
- LLM·생성형 AI의 학습·추론을 위해 컴퓨팅·메모리·네트워크·스토리지·전력·냉각·운영SW를 하나의 목적에 맞게 통합 설계한 목적형 데이터센터
- 범용 데이터센터의 전력·발열·통신 병목 한계를 극복하기 위한 AI 특화 인프라 아키텍처
## 키워드
* 가속컴퓨팅(GPU/ASIC), Memory Wall, 멀티테넌시, Confidential Computing, HBM, 액침냉각
## 암기법
* 연전통메보: 연산밀도급증·전력냉각제약·통신병목·메모리월·보안(멀티테넌시)이 필요성 5요소
## 특징
- 고밀도연산: GPU/ASIC 중심의 랙 단위 초고밀도 전력·발열 설계
- 초저지연통신: RDMA 기반 InfiniBand/RoCE로 집합통신 병목 해소
- 메모리확장성: HBM·CXL로 메모리 월(Memory Wall) 완화
- 보안격리성: Confidential Computing으로 멀티테넌시 실행 중 데이터 보호
## 목적
- 대규모 AI 학습·추론에 특화된 고성능·고효율 인프라 구축
- 전력·냉각 제약 하에서도 성능과 운영 효율을 극대화
## 구성요소
- Data Plane: GPU/TPU, HBM/HBF, CXL, NVLink/NVSwitch, InfiniBand/RoCE, NVMe
- Control Plane: Kubernetes 기반 오케스트레이션, HPC 스케줄러, 통합관측, Confidential Computing, KMS/HSM
- 전력 최적화: Quantization(정밀도축소), Sparsity 활용, DVFS, Power Capping, MIG
- 냉각 최적화: 다이렉트투칩(DLC), 후면도어 열교환기(RDHx), 액침냉각, 열인식 스케줄링
## 구성도
```
[GPU/TPU + HBM/CXL] ── NVLink ── [노드 내부]
        │ InfiniBand/RoCE(RDMA)
[클러스터: Kubernetes+HPC스케줄러] ── 통합관측/자동복구
        │
[전력: DVFS/MIG/Capping] + [냉각: DLC/액침/RDHx] → 성능·효율 극대화
```
## 연관 토픽
- [[엣지 컴퓨팅]] - 분산 AI 추론 인프라
- [[디지털 트윈]] - 데이터센터 열관리 시뮬레이션
- [[Confidential Computing]] - 실행 중 데이터 보호
- [[GPU 가상화]] - 자원 분할·공유 기술
