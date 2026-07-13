#정보관리기술사 #데이터베이스 #SQL #데이터베이스/성능/튜닝 #NEW
## 정의
SQL(Structured Query Language)
- 관계형 데이터베이스 관리시스템(RDBMS)에서 자료 검색과 관리, 스키마 생성·수정, 객체 접근 조정을 위한 프로그래밍 언어
## 키워드
* 비절차적 언어, DDL, DML, DCL, TCL, SQL-99
## 암기법
* 정조권트: DDL(정의)·DML(조작)·DCL(제어)·TCL(트랜잭션)
## 특징
- 비절차성: what 중심 선언적 질의
- 표준성: SQL-99 등 표준
- 기능 분리: 정의·조작·권한·트랜잭션 제어
## 목적
- RDBMS 자료 검색·관리 및 스키마·권한·트랜잭션 제어
## 구성요소
- DDL: 스키마 객체 생성·변경·제거 (CREATE, ALTER, DROP, TRUNCATE, RENAME, COMMENT)
- DML: 자료 입력·수정·삭제·조회 (SELECT, INSERT, UPDATE, DELETE, MERGE 등)
- DCL: 권한 부여·회수 (GRANT, REVOKE)
- TCL: 트랜잭션 제어 (COMMIT, ROLLBACK, SAVEPOINT, SET TRANSACTION) — DCL에서 분리 표현하기도 함
## 구성도
```
SQL Commands
 ├─ DDL: CREATE ALTER DROP …
 ├─ DML: SELECT INSERT UPDATE DELETE …
 ├─ DCL: GRANT REVOKE
 └─ TCL: COMMIT ROLLBACK SAVEPOINT
```
## 연관 토픽
- [[관계대수]] - SQL 이론 기반
- [[조인]] - 다중 테이블 질의
- [[옵티마이저]] - 실행계획
- [[DB 튜닝]] - 성능 튜닝
