#정보관리기술사 #컴퓨터구조 #CISCvsRISC #컴퓨터구조/프로세서 #NEW
## 정의
CISC vs RISC
- 명령어 구성 방식에 따른 CPU 유형 분류
## 키워드
* Instruction Set, 마이크로프로그램/하드와이어드, 가변/고정 길이, 컴파일러, 레지스터
## 암기법
* 복단고다: CISC(복잡·다중사이클)·RISC(단순·1사이클)
## 특징
- CISC: 복합 명령·가변길이·마이크로프로그램·소수 레지스터·Intel
- RISC: 단순 명령·고정(32bit)·하드와이어드·다중 레지스터·Load/Store·ARM
## 목적
- 명령어 집합 설계 철학에 따른 성능·복잡도 최적화
## 구성요소
| 구분 | CISC | RISC |
| 사이클 | 다중 사이클 복잡 명령 | 1사이클 단순 명령 |
| 메모리 | 다수 메모리 참조 | Load/Store만 |
| 파이프라인 | 적용 어려움 | 고도 파이프라인·슈퍼스칼라 |
| 제어 | 마이크로프로그램 | 하드와이어드 |
| 형식/길이 | 다양·가변 | 고정·32비트 |
| 컴파일러/회로 | 복잡 | 단순 |
## 구성도
```
CISC: DataPath ↔ Microprogram CU ↔ Cache ↔ Memory (가변 OP+Operand)
RISC: DataPath ↔ Hardwired CU / I-Cache·D-Cache ↔ Memory (고정 32bit)
```
## 연관 토픽
- [[Pipeline]] - RISC 파이프라이닝
- [[CPU 처리과정]] - 명령 실행
- [[Pipeline Hazard]] - 파이프라인 장애
