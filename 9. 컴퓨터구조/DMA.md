#정보관리기술사 #컴퓨터구조 #DMA #컴퓨터구조/프로세서 #NEW
## 정의
DMA(Direct Memory Access)
- CPU를 통하지 않고 주변장치(I/O)와 주기억장치 사이 데이터 전송을 담당하는 장치
## 키워드
* 단일버스분리식, 단일버스통합형, 입출력버스, Burst, Cycle Stealing, Interleaved DMA
## 암기법
* 분통입 / 버싸디인: 연결방식·전송방식
## 특징
- CPU 부하 감소: I/O-메모리 직접 전송
- 연결·전송 모드로 버스 점유 방식 다양
## 목적
- 대량 I/O 전송 시 CPU 개입 최소화
## 구성요소
- 연결: 분리(시스템버스 2회 사용)·통합(I/O가 DMAC 하위, 1회)·I/O버스(시스템+I/O버스)
- 전송: Burst(블록 독점)·Cycle Stealing(워드 1사이클 훔침)·Demand(DREQ)·Interleaved(CPU 미사용 시)
## 구성도
```
분리: CPU·Memory·DMAC·I/O ─ System Bus
통합: System Bus─DMAC─I/O
I/O버스: System Bus─DMAC─I/O Bus─I/O×N
Burst: Block 연속 / Steal: Word 1cycle
```
## 연관 토픽
- [[CPU 처리과정]] - CPU vs DMA
- [[메모리 인터리빙]] - 버스·메모리
- [[I2C와 SPI]] - 주변장치 인터페이스
