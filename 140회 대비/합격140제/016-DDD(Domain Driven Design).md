#정보관리기술사 #SW공학 #DDD #MSA
## 정의
DDD(Domain Driven Design)
- 복잡한 비즈니스 도메인 지식을 소프트웨어 설계와 긴밀히 연결하는 설계 방법론
- 전략적 설계로 서비스 경계를 정의하고 전술적 설계로 도메인 모델을 구현하는 2단계 기법
## 키워드
* Ubiquitous Language, Bounded Context, Context Map, Entity, Aggregate, Repository
## 암기법
* 유도서바컨: 유비쿼터스언어·도메인식별·서브도메인·바운디드컨텍스트·컨텍스트맵 (전략적 설계 절차)
## 특징
- 도메인 중심 사고: 기술레이어가 아닌 비즈니스 영역 기준으로 설계
- 공통언어 사용: Ubiquitous Language로 기획자·개발자 용어 통일
- 2단계 구조: 전략적 설계(Macro)와 전술적 설계(Micro)로 구분
- 경계 명확화: Bounded Context로 서비스 간 독립적 개발을 지원
## 목적
- 서비스 경계와 책임을 명확히 하여 팀별 독립적 개발 지원
- 비즈니스 규칙을 코드에 정확히 반영하는 도메인 로직 중심 설계
## 구성요소
- 전략적 설계: 도메인, 서브도메인, Bounded Context, Context Map
- 전술적 설계: Entity, Value Object, Aggregate/Aggregate Root, Repository, Domain/Application Service
- 산출물: Context Map(전략적), 클래스/도메인모델 코드(전술적)
## 구성도
```
[전략적 설계] 도메인 → 서브도메인 → Bounded Context → Context Map
                              │
                              ▼
[전술적 설계] Entity/VO → Aggregate(Root) → Repository → Domain/App Service
```
## 연관 토픽
- [[MSA]] - Bounded Context 단위로 서비스 분리하는 아키텍처
- [[Bounded Context]] - DDD 전략적 설계의 핵심 경계 개념
- [[Aggregate 패턴]] - 전술적 설계의 일관성 경계 단위
- [[헥사고날 아키텍처]] - 도메인 로직 중심 설계와 결합되는 아키텍처
