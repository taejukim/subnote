#정보관리기술사 #SW공학 #SRE #DevOps #NEW
## 정의
SRE(Site Reliability Engineering)
- 대규모 시스템의 지속적·적정 안정성 확보를 위한 SW 엔지니어링 기술
- 고도의 자동화와 자가 치유 기능을 중심으로 운영 신뢰성을 설계
## 키워드
* 안정성, 자가치유, 자동화, 카나리 배포, Toil 관리, Error Budget
## 암기법
* 메용변응문: Metric·Capacity·Change·Emergency·Culture
## 특징
- 자동화 중심성: Toil을 줄이고 운영 오류 최소화
- 정량 관리성: SLI/SLO·Error Budget으로 의사결정
- 점진 배포성: 카나리·롤링으로 변경 위험 축소
- 공유 책임성: 개발·SRE 간 오너십·도구 공유
## 목적
- 대규모 서비스의 안정성·가용성 지속 확보
- 장애 대응·복구 자동화로 MTTR 단축
## 구성요소
- Metric & Monitoring: SLI/SLO 정의·시각화, 데이터 기반 의사결정
- Capacity Planning: 수요 예측, 용량 확보, SW 성능 튜닝
- Change Management: 점진적 배포·빠른 롤백(카나리, 롤링)
- Emergency Response: Playbook 기반 장애 대응, Toil 관리, MTTR
- Culture: 비난 없는 회고, Error Budget 공유
- CSF: Silo 통합, 실패 수용, 점진 개선, 자동화, 전방위 측정
## 구성도
```
[SLI/SLO 모니터링] → [Capacity Planning]
         ↓
[Change Mgmt: Canary/Rolling] → [Emergency: Playbook/MTTR]
         ↓
     [Culture: Error Budget / Postmortem]
```
## 연관 토픽
- [[무중단 배포 기법]] - 카나리·롤링 배포
- [[카오스 테스트]] - 회복력 검증
- [[릴리즈 엔지니어링]] - 배포 파이프라인
- [[성능 테스트]] - 용량·성능 튜닝
