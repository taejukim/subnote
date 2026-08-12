#정보관리기술사 #SW공학 #카오스테스트 #ChaosEngineering
## 정의
카오스 테스트(Chaos Test)
- 시스템에 의도적으로 장애를 주입해 신뢰성과 회복력을 검증·강화하는 테스트 기법
- 분산시스템의 예측 불가능한 장애 상황을 통제된 환경에서 미리 검증하는 방법
## 키워드
* 장애주입, System call, Traffic shaping, Kill-switch, Auto-rollback
## 암기법
* 시트바메: 시스템콜·트래픽쉐이핑·바이트코드주입·메모리호그 (장애주입 기술요소)
## 특징
- 의도적 장애주입: System call, Memory hog 등으로 결함을 유발
- 실시간 관측: 시계열분석으로 지표 임계치 초과를 예측
- 자동제어: Kill-switch, Auto-rollback으로 위험을 즉시 통제
- 범위집중: 마이크로 테스트로 특정영역·사용자 대상 집중 수행
## 목적
- 런타임 동적 장애상황을 사전 발견해 시스템 회복력을 강화
- 장애를 통제 가능한 영역으로 전환해 비즈니스 연속성을 확보
## 구성요소
- 장애주입 기술: System call, Traffic shaping, Bytecode Injection, Memory hog
- 관측/복구 기술: 시계열분석, Kill-switch, Auto-rollback
- 수행전략: 마이크로 테스트 범위 수립, 인적 대응 프로세스 결합
## 구성도
```
[정상지표 정의] → [가설수립] → [장애주입: SystemCall/TrafficShaping/MemoryHog]
                                          ↓
                        [실시간 관측: 시계열분석 / Kill-switch]
                                          ↓
                        [Auto-rollback / 조직 대응 훈련(SOP)]
```
## 연관 토픽
- [[SRE]] - 사이트 신뢰성 엔지니어링과 카오스 테스트 연계
- [[Shift-Right Test]] - 운영환경 중심 테스트 기법
- [[장애복구(DR)]] - 카오스 테스트 결과로 강화되는 복구체계
- [[MSA]] - 분산 서비스 구조에서 카오스 테스트가 주로 적용되는 아키텍처
