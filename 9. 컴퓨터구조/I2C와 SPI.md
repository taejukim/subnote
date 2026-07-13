#정보관리기술사 #컴퓨터구조 #I2C와SPI #컴퓨터구조/프로세서 #NEW
## 정의
I2C와 SPI
- 보드 내 마이크로프로세서와 주변기기 간 시리얼 통신 방식
## 키워드
* SCL, SDA, CS, SCLK, MOSI, MISO, 100kbps, 70MHz
## 암기법
* I2C=클데반 / SPI=4전고: 클럭·데이터·반이중 / 4선·전이중·고속
## 특징
- I2C: 2선(SCL·SDA), 반이중, 공유버스, 저속 100kbps, 전력 상대적 높음
- SPI: 4선(CS·SCLK·MOSI·MISO), 전이중, 1:1, 고속(~70MHz), 전력 낮음
## 목적
- 보드 수준 동기식 시리얼로 MCU-주변장치 연결
## 구성요소
- I2C 동작: Start로 Bus 점유 → Slave주소·R/W 전송
- SPI 동작: CS로 Slave 선택 → SCLK 시작 → MOSI/MISO 전송
## 구성도
```
I2C: Master ──SDA/SCL── Slave×N (공유)
SPI: Master ─CS/SCLK/MOSI/MISO─ Slave (1:1)
```
## 연관 토픽
- [[DMA]] - 고속 I/O 전송
- [[워치독 타이머]] - 임베디드 주변
- [[CPU 처리과정]] - 프로세서
