#정보관리기술사 #AI #LangGraph #AI/LLM/생성AI #NEW
## 정의
LangGraph
- 여러 에이전트가 협업해 작업을 수행하는 멀티 에이전트 시스템 구축을 위한 LangChain 기반 상태관리·워크플로우 라이브러리
## 키워드
* Agent, Multi Agent, Collaborative Agent, Workflow Library, Node, Edge, Designer
## 암기법
* 노엣데워API: Node·Edge·DataLayer·Workflow Designer·API 통합
## 특징
- 그래프 기반성: Node·Edge로 비순차·순환 워크플로우 표현
- 상태 순환성: Thought→Action→Observation 루프, Finish 조건 종료
- 시각화성: Workflow Designer로 NLP 파이프라인 시각 설계
- 병렬·재사용성: 모듈 병렬화·재사용으로 복잡 태스크 최적화
## 목적
- NLP·에이전트 작업의 설계·실행 단순화 및 데이터 흐름 시각화
- 모듈 간 상호작용 최적화와 AI Agent로의 전환 지원
## 구성요소
- Node: 전처리·모델실행·결과분석 등 NLP 모듈
- Edge: 노드 간 데이터 흐름·의존성
- Data Layer: 입출력 데이터 정의
- Workflow Designer: 그래프 설계·수정 UI
- API 통합: 외부 서비스·모델 연결
- vs LangChain: Chain(순차/병렬) vs Graph(노드·엣지·비순차)
## 구성도
```
Question → Thought → Action → Observation ↺
                              ↓ (Finish Action)
                           Finish
```
## 연관 토픽
- [[랭체인]] - LLM 앱 프레임워크
- [[멀티 에이전트 시스템]] - 다중 에이전트 협업
- [[AI Agent]] - 단일 에이전트 개념
- [[에이전틱 AI]] - 자율 목표 수행 AI
