#정보관리기술사 #컴퓨터구조 #HBM #HBF
## 정의
HBM(High Bandwidth Memory) & HBF(High Bandwidth Flash)
- DRAM/NAND를 3D 적층해 대역폭을 높이고 데이터 이동 병목을 해소한 차세대 메모리 계층 기술
- LLM 추론 시 요구되는 TB급 메모리를 고대역폭·비휘발성으로 지원하는 하이브리드 구조
## 키워드
* TSV, 인터포저, BiCS NAND, CBA, KV 캐시, D2D 인터페이스
## 암기법
* HTP실인: HBM·TSV·패키징·실리콘인터포저·인터페이스(HBM 핵심 구성)
## 특징
- HBM: DRAM 적층+TSV로 고대역폭·저지연 구현, SSD보다 빠른 접근
- HBF: NAND 3D 적층으로 대용량·비휘발성 확보, HBM보다 느리지만 SSD보다 빠름
- Hybrid 구조: 동일 인터포저 위 HBM·HBF 병렬 배치로 용량과 속도 균형
- LHB(Latency Hiding Buffer): HBF의 긴 지연시간을 보완하는 버퍼 내장
## 목적
- LLM 추론 시 TB급 KV 캐시 요구를 충족하는 메모리 용량 확보
- GPU 연산 대기(메모리 병목) 최소화로 AI 추론 비용(TCO) 절감
## 구성요소
- TSV: DRAM/NAND Die 관통 수직 전극
- Base(Logic) Die: PHY와 Core, 타 Die 연결 담당
- Silicon Interposer/Package Substrate: HBM·HBF·GPU 연결 기판
- Micro Bump: Die 간 접합용 미세 금속 돌기
- LHB: HBF Base Die 내 지연 보완 버퍼
## 구성도
```
[GPU] ── Silicon Interposer ──┬── [HBM: Core+Base Die+TSV]
                               └── [HBF: NAND Core+Base Die+LHB]
                (D2D Interface, Package Substrate)
```
## 연관 토픽
- [[CXL]] - 메모리 확장·풀링 기술
- [[UCIe]] - Chiplet 간 D2D 인터커넥트 표준
- [[KV 캐시]] - LLM 추론 메모리 요구 핵심
- [[메모리 계층구조]] - Memory Centric Computing
