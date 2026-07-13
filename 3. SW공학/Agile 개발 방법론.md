#정보관리기술사 #SW공학 #Agile #개발방법론 #SW공학/SW_개발_방법론/모델 #NEW
## 정의
Agile 개발 방법론
- 짧은 반복(Iteration)과 점진적(Incremental) 인도(Delivery)로 변화하는 요구에 빠르게 대응하는 소프트웨어 개발 접근법
- 2001년 Agile Manifesto의 4대 가치·12원칙에 기반한 경량 프로세스 체계
## 키워드
* Manifesto, Iteration, Incremental, Scrum, XP, Kanban, Waterfall 대비
## 암기법
* "가치사람협변" - 개인과 상호작용, 동작하는 SW, 고객 협력, 변화에 대응
## 특징
- 반복·점진: 짧은 주기로 계획·개발·검증·회고를 반복하며 점진적으로 가치 인도
- 고객 협업: 계약·문서보다 지속적 피드백과 우선순위 조정을 중시
- 적응적 계획: 초기 상세 계획보다 변화 수용과 백로그 기반 우선순위 관리
- 자기조직화: 교차기능 팀이 자율적으로 일정·작업 방식을 조정
## 목적
- 불확실성·요구 변경이 큰 환경에서 조기·빈번한 가치 전달
- 피드백 루프 단축으로 품질·적합성(Fit) 향상 및 리스크 조기 발견
## 구성요소
- Agile Manifesto: 프로세스·도구보다 개인/상호작용, 문서보다 동작 SW, 계약보다 고객 협력, 계획 준수보다 변화 대응
- Scrum: Sprint, Product Backlog, Daily Scrum, Review/Retrospective 기반 프레임워크
- XP(eXtreme Programming): TDD, Pair Programming, CI, Refactoring 등 공학 실천법
- Kanban: WIP 제한, 시각화 보드, Pull 방식으로 흐름(Flow) 최적화
- Waterfall 대비: 순차·단계 완료형 vs Agile의 반복·적응형; 요구 확정성이 높을수록 Waterfall, 변화가 클수록 Agile 적합
## 구성도
```
[Agile Manifesto 4 Values]
  개인·상호작용 > 프로세스·도구
  동작하는 SW   > 포괄적 문서
  고객 협력     > 계약 협상
  변화 대응     > 계획 준수
        │
        ▼
┌─────────────── Iterative / Incremental ───────────────┐
│  Plan → Build → Test → Review → Adapt  (짧은 주기)   │
└───────────────────────────────────────────────────────┘
        │
   ┌────┼────┬────────┐
   ▼    ▼    ▼        ▼
 Scrum  XP  Kanban  (하이브리드)
        │
        ▼
 Waterfall: 요구→설계→구현→시험→인도 (순차, 변경 비용↑)
 Agile:     백로그 기반 반복 인도 (변경 비용↓, 피드백↑)
```
## 연관 토픽
- [[Scrum]] - Sprint·역할·이벤트 중심 Agile 프레임워크
- [[XP]] - 공학 실천법 중심 Extreme Programming
- [[Kanban]] - WIP 제한·시각화 기반 흐름 관리
- [[폭포수 모델]] - 순차형 전통 개발 모델과의 대비
