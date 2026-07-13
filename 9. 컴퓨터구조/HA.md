#정보관리기술사 #컴퓨터구조 #HA #컴퓨터구조/고가용성 #NEW
## 정의
HA(High Availability)
- 두 대 이상 시스템을 클러스터로 묶어, 장애 시 최소 중단으로 다른 시스템에 Fail-Over하여 업무 연속성을 유지하는 메커니즘
## 키워드
* Heart-beat, Hot Standby, Mutual Takeover, Concurrent Access
## 암기법
* 핫상병: Hot Standby·Mutual Takeover·Concurrent Access
## 특징
- Heartbeat로 상호 상태 감시
- Active/Standby 또는 Active-Active 구성
- Failover로 연속성 확보
## 목적
- 시스템 장애에도 서비스 중단 최소화·업무 연속성 유지
## 구성요소
- Hot Standby: Active+대기 Backup, 장애 시 Take-over, 외장디스크는 Active만(장애 시 Backup)
- Mutual Takeover: 각자 Active 업무, 장애 시 상대 자원 Failover(이중 용량 필요)
- Concurrent Access: 전원 Active 병렬, L4 등, Failover 없이 가용성(동일 업무)
## 구성도
```
Hot: Active ─Heartbeat─ Standby → Shared DB
Mutual: A(ActA/StB) ⇄ B(ActB/StA) → DB_A, DB_B
Concurrent: Active×N ←L4→ Shared DB
```
## 연관 토픽
- [[워치독 타이머]] - 장애 감지·복구
- [[이레이저 코딩]] - 스토리지 내결함성
- [[쿼리 오프로딩]] - Slave HA
