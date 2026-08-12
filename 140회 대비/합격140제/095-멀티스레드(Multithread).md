#정보관리기술사 #운영체제 #멀티스레드 #SMT
## 정의
멀티스레드(Multithread)
- 하나의 프로세스를 다수 스레드로 구성해 자원을 공유하며 작업을 분할 수행하는 경량 실행 구조
- OS 수준의 매핑모델(One-to-One 등)과 하드웨어 수준의 실행유형(SMT 등)으로 구현되는 동시성·병렬성 기법
## 키워드
* One to One, Many to One, Many to Many, User/Kernel Thread, Interleaved/Blocked multi-threading, Simultaneous multithreading, Chip multi-threading
## 암기법
* 일다다: One to One·Many to One·Many to Many (스레드 매핑 3대 모델)
## 특징
- 자원공유 효율성: 동일 프로세스 내 Code·Data·Heap 공유, Stack만 독립 보유
- 문맥전환 경량화: TCB 기반 전환으로 PCB 기반 프로세스 전환보다 오버헤드 적음
- 매핑모델 다양성: User/Kernel Thread 매핑 방식에 따라 병렬성·관리비용 트레이드오프 상이
- 하드웨어 실행유형 4가지: Interleaved·Blocked(전환기반), Simultaneous·Chip(동시실행기반) 멀티스레딩
## 목적
- 프로세스 생성 대비 적은 오버헤드로 동시성·병렬 처리 향상
- 멀티코어 환경에서 하드웨어 성능을 효과적으로 활용
## 구성요소
- 프로세스 vs 스레드: 독립 실행단위(PCB) vs 종속 실행단위(TCB), 자원공유 vs 독립주소공간
- 매핑모델: One to One(실제병렬·큰비용), Many to One(단순·Blocking 취약), Many to Many(병렬성+효율 확보)
- 스레드 전환기반: Interleaved(짧은지연 은닉), Blocked(긴지연 처리 적합)
- 동시실행기반: Simultaneous(SMT, 코어 내 자원 공유), Chip multi-threading(다중코어+다중스레드 결합)
## 구성도
```
[프로세스] ── Main Thread ── Worker Thread(들)
              (Code/Data/Heap 공유, Stack 독립)
OS매핑: User Thread ── Kernel Thread
        (1:1 / N:1 / N:M)
HW실행: Interleaved/Blocked(전환기반) ↔ Simultaneous/Chip(동시실행기반)
```
## 연관 토픽
- [[문맥교환(Context Switching)]] - 스레드 전환 오버헤드 비교 대상
- [[Belady's Anomaly]] - 메모리 관리 이상현상과 연계
- [[가상 메모리 관리 기법]] - 스레드별 스택 메모리 할당
- [[컴퓨터구조]] - SMT·멀티코어 하드웨어 구조
