#운영체제 #RingLevel #CPU #필수 #운영체제/프로세스관리 #NEW
## 정의
CPU Ring Level
- 프로세서의 권한 수준(Privilege Level)을 계층적으로 표현해 OS·SW 실행 권한을 관리하는 보안 구조
## 키워드
* Ring 0(Kernel/Supervisor), Ring 1·2(중간), Ring 3(User/Application), System Call, Privilege Level
## 암기법
* Ring0커널 Ring3유저: 0=최고권한, 3=최저권한
## 구성요소/특징/유형
| Ring | 명칭 | 설명 |
| ---- | ---- | ---- |
| Ring 0 | Kernel Mode | OS 커널·드라이버, 최고 권한 |
| Ring 1·2 | Middle | 가상화 SW 등, 현대 OS에서 드묾 |
| Ring 3 | User Mode | 일반 앱 실행, HW 직접 접근 불가 |
## 연관 토픽
- [[커널]] - Ring 0에서 동작
- [[인터럽트]] - Ring 3→0 전환
- [[문맥교환]] - 모드 전환
