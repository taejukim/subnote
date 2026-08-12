#정보관리기술사 #SW공학 #SDD #명세주도개발
## 정의
SDD(Spec-Driven Development)
- 실행·검증 가능한 명세를 SSOT로 코드·테스트를 자동 생성·동기화하는 명세 주도 개발 방법론
- AI 코드 생성 시대에 최적화된, 명세 품질이 곧 코드 품질을 결정하는 개발 패러다임
## 키워드
* 명세 기반 개발, 형식 명세, TDD·BDD 비교, AI 코드생성, 계약 기반 테스트
## 암기법
* 단자검친: 단일진실원천·자동동기화·검증가능성·AI친화성
## 특징
- 명세의 단일 진실 원천: 실행·검증 가능한 명세가 코드·테스트의 유일한 기준
- 자동 동기화: 명세 변경 시 코드와 테스트가 자동 재생성·갱신
- 검증 가능성: 명세 자체가 형식적으로 검증 가능해 모호성 최소화
- AI 친화성: 명세를 LLM 프롬프트로 제공해 코드·테스트 동시 생성
## 목적
- LLM 기반 AI 코드 생성 시 정확한 명세 제공으로 생성 품질 향상
- 명세-코드-테스트 간 불일치·드리프트 방지
## 구성요소
- 자연어 명세(Gherkin): Given-When-Then 형식, LLM 프롬프트 입력 활용
- 형식 명세(Formal Specification): Z·VDM·Alloy로 수학적 정확성 확보, SSOT 역할
- API 계약(OpenAPI/JSON Schema): REST API 구조를 SSOT로 정의, Mock 자동생성
- 계약 기반 테스트(Contract Test): Pact 등으로 소비자-공급자 계약 자동 검증
- 준수 검증(Conformance Verification): CI/CD 게이트에서 코드-명세 일치 확인
## 구성도
```
[명세 작성(자연어/형식명세)] → [AI 코드 생성(LLM)] → [자동 테스트 생성] → [명세 적합성 검증(CI 게이트)]
                                        ↑ 명세 변경 시 코드·테스트 자동 동기화
```
## 연관 토픽
- [[TDD(Test-Driven Development)]] - 테스트 우선 개발
- [[BDD(Behavior-Driven Development)]] - 행위 기반 개발
- [[AI-DLC(AI-Driven Development Life Cycle)]] - AI 주도 개발 생명주기
- [[계약 기반 테스트]] - API 계약 자동 검증
