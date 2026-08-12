#정보관리기술사 #컴퓨터구조 #UCIe #Chiplet
## 정의
UCIe(Universal Chiplet Interconnect Express)
- SiP 내부 이기종 Chiplet 간 고속·저지연·저전력 통신을 위한 개방형 Die-to-Die(D2D) 인터커넥트 표준
- 모놀리식 SoC의 수율·비용 한계를 극복하는 칩렛 기반 통합 연결 규격
## 키워드
* Chiplet, D2D Interconnect, Physical Layer, D2D Adapter Layer, Protocol Layer, PCIe/CXL/Streaming Mapping
## 암기법
* 물어프시: 물리계층·어댑터계층·프로토콜계층·시스템/패키징계층(4-Layer 구조)
## 특징
- 초고대역폭·저전력: Die 간 직접 연결로 병목 최소화
- 개방형 생태계: 멀티벤더 Chiplet 조합 가능
- 다중 프로토콜 지원: PCIe·CXL·Streaming 매핑 캡슐화
- 초저지연: 2ns 미만의 패키지 내부 통신 지연
## 목적
- 무어의 법칙 한계 극복 및 수율 향상·원가 절감
- 이기종 반도체(CPU/GPU/NPU/Memory) 통합으로 AI·HPC 성능 확보
## 구성요소
- Physical Layer: D2D PHY, Link Training/Calibration, Sideband Channel
- D2D Adapter Layer: Link Management, Protocol Negotiation, CRC/Retry
- Protocol Layer: PCIe/CXL/Streaming Mapping
- System/Packaging Layer: 2D/2.5D/3D Packaging, Multi-vendor Chiplet, DFx/Compliance Test
## 구성도
```
[CPU Chiplet] [GPU/NPU Chiplet] [I/O Chiplet] [Memory Chiplet]
        └────────────┬────────────┘
                UCIe D2D Interconnect
   (Physical → D2D Adapter → Protocol → Packaging Layer)
                     ↓
        Silicon Interposer / Package Substrate
```
## 연관 토픽
- [[CXL]] - 메모리 풀링·캐시 일관성 확장 프로토콜
- [[PCIe]] - 범용 I/O 연결 표준
- [[HBM]] - Chiplet과 결합되는 고대역폭 메모리
- [[SiP]] - 패키지 내 이기종 통합 기술
