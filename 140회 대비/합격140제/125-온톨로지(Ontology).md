#정보관리기술사 #AI #온톨로지 #지식그래프
## 정의
온톨로지(Ontology)
- 특정 도메인의 개념·속성·관계·규칙을 체계적으로 정의하여 컴퓨터가 의미를 이해하고 추론하게 하는 지식 표현 모델
- 지식그래프·의미추론을 통한 지능형 의사결정의 기반 체계
## 키워드
* Class, Instance, Property, Relation, Rule, Axiom, RDF, SPARQL, Property Graph, Cypher, GraphRAG
## 암기법
* 클인속관규: Class·Instance·Property·Relation·Rule(온톨로지 6대 구성요소)
## 특징
- 의미표현성: 개념·관계를 명시적으로 정의해 의미 이해 지원
- 추론가능성: 규칙 기반으로 명시되지 않은 새로운 사실 도출
- 표준기반성: RDF/OWL 등 W3C 표준으로 상호운용성 확보
- 설명가능성: 추론 근거를 명시해 LLM 환각 완화
## 목적
- 데이터 간 의미·관계 기반의 맥락·인과 중심 의사결정 지원
- 생성형 AI와 결합해 설명가능하고 신뢰할 수 있는 판단 근거 제공
## 구성요소
- Class: 개념·범주 (예: 고객, 상품)
- Instance: 실제 객체 (예: 고객A)
- Property: 속성 및 관계 (예: 구매일, 가격)
- Relation: 객체 간 관계 (예: 고객→상품 구매)
- Rule/Axiom: 추론 규칙 및 제약조건 (예: VIP 판정 규칙)
## 구성도
```
[Ontology Layer: Class·Property·Rule 정의]
        ↓
[Knowledge Graph Layer: 데이터-온톨로지 연결]
        ↓
[Reasoning Layer: Rule Engine 의미추론] → [Decision/Action Layer]
```
## 연관 토픽
- [[지식그래프]] - 온톨로지 기반 데이터 연결 구조
- [[RDF]] - Triple 기반 의미 데이터 표현 표준
- [[GraphRAG]] - 그래프 기반 검색증강생성
- [[Property Graph]] - Node-Edge 기반 관계 데이터 모델
