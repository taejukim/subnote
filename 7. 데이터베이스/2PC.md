#정보관리기술사 #데이터베이스 #2PC #데이터베이스/트랜잭션/회복 #NEW
## 정의
2PC(2-Phase Commit)
- 분산 데이터베이스 환경에서 원자성을 보장하기 위해, 분산 트랜잭션에 관여하는 모든 노드가 Commit하거나 모든 노드가 Rollback하는 메커니즘
## 키워드
* Global Coordinator, 지역 노드, Prepare/Commit, Commit Point Site, 원자성
## 암기법
* 준커: Prepare(준비)·Commit(확정) 2단계
## 특징
- 원자성 보장: 전원 Commit 또는 전원 Rollback
- 중앙 조정: Global Coordinator가 결정
- 블로킹 가능: 조정자 장애 시 참여자 대기
## 목적
- 분산 트랜잭션의 원자성(All-or-Nothing) 보장
## 구성요소
- Global Coordinator: 참여자 목록 보유, Global Commit 개시
- 지역 노드(Local): 지역 트랜잭션 수행, 조정자 결정 따름
- Commit Point Site: 관련 원격 사이트 중 가장 Commit/Rollback 수행, 핵심 데이터 보유 노드
- Client: 타 노드 DB를 이용하는 노드
- Phase1 Prepare: Commit 요청 → Commit Point Site 결정 → Prepare 전송·응답
- Phase2 Commit: 전원 Ready면 Commit, 오류 시 Rollback
## 구성도
```
지역노드1 ─Commit요청→ [Global Coordinator]
                              │ Prepare
                    ┌─────────┼─────────┐
                 지역1      지역2 … 지역N
                    └─응답────┴─────────┘
                              │ Commit/Rollback
```
## 연관 토픽
- [[분산 DB]] - 분산 트랜잭션
- [[Transaction]] - ACID 원자성
- [[데이터베이스 회복기법]] - 회복
- [[MVCC]] - 동시성 제어
