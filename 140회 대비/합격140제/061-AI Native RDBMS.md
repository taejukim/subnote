#정보관리기술사 #디지털서비스 #AINativeRDBMS #벡터검색
## 정의
AI Native RDBMS
- 관계형 데이터 처리 역량 위에 벡터 임베딩 인덱싱·유사도 검색(ANN)을 스토리지 엔진 레벨에서 네이티브 통합한 차세대 DBMS
- LLM 및 RAG 파이프라인을 직접 지원하는 하이브리드 데이터베이스
## 키워드
* ANN, 유사도 검색, 벡터 임베딩, HNSW, IVF, DiskANN, Pre-filtering, Post-filtering
## 암기법
* 벡관하런확: 벡터스토리지·관계처리·하이브리드쿼리·런타임임베딩·확장성 (AI Native RDBMS 5대 구성요소)
## 특징
- 네이티브통합성: VECTOR(dim) 타입을 WAL·MVCC 엔진에 기본 타입으로 내장
- 하이브리드검색성: B-Tree(정형)와 HNSW/IVF(벡터) 인덱스를 동시 스캔
- 인메모리 최적화: HNSW 등 그래프 인덱스는 대규모 메모리 점유 요구
- ACID 보장성: 벡터·관계 연산 결과를 트랜잭션 통제 하에 병합 반환
## 목적
- LLM 환각 방지를 위한 RAG 파이프라인의 신뢰성 있는 데이터 기반 마련
- Polyglot 인프라 복잡도와 TCO를 줄이는 통합 데이터 아키텍처 실현
## 구성요소
- 스토리지 및 인덱서: HNSW(계층적 근접그래프), IVF(Voronoi 클러스터링), DiskANN(디스크 기반 대규모 인덱스)
- 하이브리드 쿼리 최적화: Pre-filtering(조건 우선), Post-filtering(벡터검색 후 필터), CBO 기반 산정
- 런타임 환경: In-Database 모델 실행 엔진으로 API 호출 없이 임베딩·추론 수행
- 확장성 계층: 기존 WAL/MVCC 엔진에 VECTOR 타입을 네이티브 통합하는 추상화 계층
## 구성도
```
[자연어 질의] → [임베딩 변환(벡터화)]
                       │
        ┌──────────────┴──────────────┐
   [B-Tree 인덱스(정형)]     [HNSW/IVF/DiskANN(벡터)]
        └──────────────┬──────────────┘
              [CBO 하이브리드 실행계획]
                       │
        [RDBMS 연산: ACID 트랜잭션 결과 병합] → 응답
```
## 연관 토픽
- [[RAG(Retrieval-Augmented Generation)]] - 검색증강생성 파이프라인
- [[벡터 데이터베이스]] - 순수 벡터 전용 저장소
- [[옵티마이저(Optimizer)]] - 실행계획 비용 산정 엔진
- [[데이터 레이크하우스(Data Lakehouse)]] - AI/BI 통합 데이터 아키텍처
