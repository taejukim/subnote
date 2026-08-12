#정보관리기술사 #SW공학 #데메테르의법칙 #LawOfDemeter
## 정의
데메테르의 법칙(Law of Demeter)
- 모듈은 자신이 직접 아는 객체와만 통신해야 한다는 최소 지식 기반 설계 원칙
- 객체 간 결합도를 최소화하여 정보은닉과 캡슐화를 강화하는 원칙
## 키워드
* 최소 지식 원칙, Message Chain, 정보은닉, Façade Pattern, Tell Don't Ask
## 암기법
* 최연위탈: 최소지식·연쇄호출지양·위임은닉·행위중심(Tell,Don't Ask)
## 특징
- 최소지식원칙: 직접 아는 객체와만 통신, 내부구조 비노출
- 연쇄호출 지양: 점(.)이 반복되는 Message Chain을 최소화
- 위임은닉: 하위 객체 접근을 상위 객체가 대신 처리
- 행위중심설계: 상태를 묻지 않고 행위를 요청(Tell, Don't Ask)
## 목적
- 객체 간 결합도를 낮춰 유지보수성과 캡슐화 강화
- 구조 변경 시 연쇄적 수정(Ripple Effect)을 최소화
## 구성요소
- 호출 가능 대상: 객체 자체, 파라미터 객체, 내부 생성 객체, 멤버 컴포넌트, 전역변수
- 정보전문가 패턴(GRASP): 정보를 가장 많이 가진 객체에게 책임을 부여
- 파사드 패턴(Façade Pattern): 복잡한 하위 시스템을 단일 인터페이스로 추상화
## 구성도
```
[Client] ──only talks to──> [Facade(SubsystemFacade)]
                                    │
                       ┌──────────────┼──────────────┐
                 [Subsystem A]  [Subsystem B]  [Subsystem C]
         (Client는 A/B/C를 직접 모르며 Message Chain 발생하지 않음)
```
## 연관 토픽
- [[GRASP 패턴]] - 책임 할당 설계원칙 모음, Information Expert 포함
- [[Facade Pattern]] - 데메테르 법칙 구현을 위한 대표 디자인 패턴
- [[캡슐화]] - 객체 내부구조 은닉의 근본 개념
- [[결합도와 응집도]] - 데메테르 법칙이 추구하는 설계 품질 지표
