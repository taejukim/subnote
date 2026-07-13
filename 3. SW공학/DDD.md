#정보관리기술사 #SW공학 #DDD #도메인설계
## 정의
DDD(Domain-Driven Design)
- 비즈니스 도메인 지식을 SW 설계와 연결하는 도메인 중심 설계 방법론
- 책임·역할 반영을 위해 유비쿼터스 언어·바운디드 컨텍스트로 모델 분할
## 키워드
* 유비쿼터스 언어, Bounded Context, Aggregate, Entity, Value Object, MSA
## 암기법
* 유바애엔밸: 유비쿼터스·바운디드·애그리거트·엔티티·밸류
## 특징
- 도메인 정렬성: 비즈니스 규칙이 코드로 직접 표현
- 분할성: 도메인 → 서브도메인 → 바운디드 컨텍스트
- 언어 일관성: 유비쿼터스 언어로 의사소통
- 진화성: 도메인 변화에 맞춰 모델 지속 개선
## 목적
- 비즈니스 중심 시스템 분할로 MSA 경계 명확화
- 데이터 중심이 아닌 행위 중심 설계로 복잡성 제어
## 구성요소
- 전략적 설계: 도메인, 서브도메인, Bounded Context, Context Map
- 전술적 설계: Entity, Value Object, Aggregate & Root, Repository
- Domain Service, Application Service, Factory
- 핵심원칙: 도메인 중심 사고, 유비쿼터스 언어, 도메인 전문성
## 구성도
```
도메인 → 서브도메인 → Bounded Context → Microservice
[전략적 설계: 어떻게 나눌 것인가] vs [전술적 설계: 어떻게 구현할 것인가]
```
## 연관 토픽
- [[MSA]] - DDD 기반 서비스 분리
- [[이벤트 스토밍과 헥사고날 아키텍처]] - DDD 모델링 기법
- [[SDD]] - 명세 중심 개발 비교
- [[아키텍처 모델-패턴]] - 설계 패턴
