#정보관리기술사 #SW공학 #CleanArchitecture #관심사분리 #NEW
## 정의
Clean Architecture
- SW 아키텍처를 4계층으로 관심사를 분리해 계층 의존성에서 벗어나 모듈성·확장성·유연성을 확보하는 아키텍처
- 의존성 규칙: 외부 → 내부(안쪽 계층만 의존)
## 키워드
* Separation of Concerns, Entities, Use Case, Interface Adapters, Frameworks & Drivers
## 암기법
* EUIF: Entity → Use Case → Interface Adapter → Frameworks/Drivers
## 특징
- Entity: 핵심 업무 규칙 캡슐화
- Use Case: 애플리케이션 업무 규칙·흐름 조정
- Interface Adapter: Presenter/Controller/Gateway 변환
- External Interface: UI·DB·Framework 등 변경 빈번 계층 분리
## 목적
- 비즈니스 규칙을 프레임워크·DB·UI 변경으로부터 보호
- 테스트·교체·확장이 쉬운 구조 확보
## 구성요소
- Entity: Enterprise Business Rules
- Use Case: Application Business Rules, Interactor
- Interface Adapters: Controllers, Presenters, Gateways
- Frameworks & Drivers: Web, UI, DB, Devices, External Interfaces
## 구성도
```
  ┌── Frameworks & Drivers (UI/DB/Devices) ──┐
  │  ┌── Interface Adapters (C/P/G) ──┐      │
  │  │  ┌── Use Cases ──┐             │      │
  │  │  │   Entities    │             │      │
  │  │  └───────────────┘             │      │
  │  └────────────────────────────────┘      │
  └──────────────────────────────────────────┘
  Controller → UC Input | UC → Presenter(Output)
```
## 연관 토픽
- [[SW Architecture]] - 아키텍처 일반
- [[객체지향 설계의 원리]] - DIP·의존역전
- [[DDD]] - 도메인·엔티티
