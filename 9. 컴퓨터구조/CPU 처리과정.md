#정보관리기술사 #컴퓨터구조 #CPU처리과정 #컴퓨터구조/프로세서 #NEW
## 정의
CPU 처리과정
- CPU가 한 개의 명령어를 실행하는 데 필요한 과정으로, 실행 시작부터 중단될 때까지 반복되는 과정
## 키워드
* 인출 사이클, 실행 사이클, PC, MAR, MBR, IR, AC, 주소/데이터/제어 버스
## 암기법
* 인실: 인출(Fetch)·실행(Execution)
## 특징
- Fetch-Execute 반복: 명령 인출 후 실행
- 레지스터 중심: PC·MAR·MBR·IR·AC 활용
- 버스 연결: 주소·데이터·제어 버스로 메모리 접근
## 목적
- 단일 명령어를 인출·해석·실행하여 프로그램 수행
## 구성요소
- 인출: t0 MAR←PC / t1 MBR←M(MAR), PC←PC+1 / t2 IR←MBR
- 실행(ADD 예): t0 MAR←IR(addr) / t1 MBR←M(MAR) / t2 AC←AC+MBR
- CPU 내부: PC, ALU, AC, MAR, MBR, IR, 제어장치
- 외부: 기억장치, 주소·데이터·제어 버스
## 구성도
```
[PC]→[MAR]→Memory →[MBR]→[IR]  (인출)
[IR(addr)]→[MAR]→Memory→[MBR]→ALU(+AC)→[AC]  (실행)
```
## 연관 토픽
- [[Pipeline]] - 파이프라인 처리
- [[CISC vs RISC]] - 명령어 집합
- [[DMA]] - CPU 우회 전송
