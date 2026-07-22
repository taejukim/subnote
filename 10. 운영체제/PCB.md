#운영체제 #PCB #필수 #운영체제/CPU스케줄링 #NEW
## 정의
PCB(Process Control Block)
- 프로세스 실행 시마다 정보를 기록·관리하는 특별한 자료구조, Process Management = PCB Management
## 키워드
* PID, Process State, PC, Register, Scheduling, Accounting, I/O, Memory
## 암기법
* 식상카레스계입메: PID·상태·PC·Register·Scheduling·Accounting·I/O·Memory
## 구성요소/특징/유형
| 항목 | 설명 |
| ---- | ---- |
| PID | 프로세스 고유 식별자 |
| Process State | New/Ready/Running/Waiting/Finished |
| Program Counter | 다음 실행 명령 주소 |
| Register Save Area | AC, ISR, 범용레지스터 등 |
| Scheduling Info | 우선순위, 큐 포인터 |
| I/O Status | 할당 I/O, 열린 파일 |
| Memory Mgmt | Page/Segment Table, 경계 |
## 연관 토픽
- [[프로세스 상태 전이도]] - 상태
- [[문맥교환]] - PCB 저장·복원
- [[프로세스와 스레드 비교]] - PCB vs TCB
