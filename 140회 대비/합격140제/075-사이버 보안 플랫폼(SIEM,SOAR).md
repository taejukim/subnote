#정보관리기술사 #보안 #SIEM #SOAR
## 정의
사이버 보안 플랫폼(SIEM/SOAR)
- IT 인프라 전반의 보안 이벤트를 통합 수집·분석해 위협을 탐지·대응하는 통합 보안 관리 체계
- SIEM은 로그 수집·상관분석, SOAR는 대응 자동화·오케스트레이션을 담당
## 키워드
* 이벤트 로그, 상관분석, Automation, Orchestration, ==Playbook==, Workflow, Threat Intelligence, MTTR
## 암기법
* 엔네디모: 엔드포인트·네트워크·DB·모바일 로그를 SIEM이 통합 수집
## 특징
- 통합 수집성: 엔드포인트·네트워크·DB·모바일 등 이종 로그를 중앙 집중 수집
- 상관분석: 빅데이터 기반 이벤트 상관분석으로 위협 패턴 탐지
- 자동화·오케스트레이션: SOAR가 다양한 보안장비·IT시스템을 통합 운영·자동대응
- Playbook 기반 대응: 사전 정의된 워크플로우로 신속한 사고 대응 수행
## 목적
- 고도화되는 보안위협에 대한 실시간 탐지·분석 체계 확보
- 대응 자동화를 통한 MTTD·MTTR 단축 및 오탐 감소
## 구성요소
- SIEM 수집로그: 엔드포인트(백신·레지스트리), 네트워크(방화벽·IDS/IPS·웹프록시), DB(쿼리·인증), 모바일(APP·네트워크구성)
- SOA(SOAR 기술요소): Orchestration(통합운영), Automation(자동대응), Integration API(SIEM·EDR·Firewall 연계)
- SIRP: Response/Reporting, Workflow Engine, Dynamic Playbook
- TIP: Threat Intelligence, Case Management, Artifact Workflow
## 구성도
```
[엔드포인트/네트워크/DB/모바일 로그] → SIEM(수집·상관분석)
                                         ↓ 이벤트/알림
                                       SOAR
                          ┌──────────────┼──────────────┐
                       SOA(자동화)   SIRP(대응관리)   TIP(위협정보)
                          └──────────────┴──────────────┘
                                    신속 대응(MTTR↓)
```
## 연관 토픽
- [[멀웨어]] - EDR/XDR 연계 탐지 대상
- [[APT]] - SIEM/SOAR 기반 다단계 위협 대응
- [[Secure SDLC 및 STRIDE 기반 위협 모델링]] - 운영단계 SIEM 연동
- [[위협 헌팅]] - 능동적 위협 탐지 활동
