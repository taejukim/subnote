#정보관리기술사 #컴퓨터구조 #PipelineHazard #컴퓨터구조/프로세서 #NEW
## 정의
Pipeline Hazard
- 파이프라인 프로세스에서 명령어 의존성을 발생시킬 수 있는 문제
## 키워드
* 구조적 해저드, 데이터 해저드, 제어 해저드, RAW/WAR/WAW
## 암기법
* 구데제: 구조적·데이터·제어
## 특징
- 구조적: 동일 자원(메모리) 충돌
- 데이터: 이전 명령 결과 종속(RAW 등)
- 제어: Branch/Jump로 후속 명령 폐기
## 목적
- 파이프라인 성능 저하 요인 식별·해결
## 구성요소
- 구조적: IF·MEM 동시 접근 충돌 → 리소스/하드웨어 추가, Harvard, 메모리 인터리빙
- 데이터: R1 쓰기 전 읽기 → Renaming, Stall, Forwarding, 소프트웨어 제약
- 제어: 분기 결정 전 후속 유입 → Stall, 예측(Taken/Not), 지연분기, BTB, Loop Buffer
## 구성도
```
구조적: IF↔MEM 동일메모리
데이터: ADD R1… → SUB …R1 (RAW)
제어: Branch@EX → 후속 IF/ID 폐기
```
## 연관 토픽
- [[Pipeline]] - 파이프라인
- [[메모리 인터리빙]] - 구조적 해저드 완화
- [[CISC vs RISC]] - 파이프라인 적합성
