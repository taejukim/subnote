#정보관리기술사 #데이터베이스 #Elasticsearch #분산검색
## 정의
엘라스틱서치(Elasticsearch)
- 아파치 루씬 기반으로 문서 데이터를 색인·검색·조회·랭킹하는 자바 오픈소스 분산형 검색 DBMS
- RAG 시스템의 벡터 데이터베이스 구성요소로도 활용되는 분산형 문서 검색 플랫폼
## 키워드
* Apache Lucene, Schema-less, Coordinating Node, Shard, Index, Data Node, Master Node, RAG
## 암기법
* 루스하: 루씬기반·스키마리스·하이가용성(HA)/전문검색(FTS)이 핵심 특징
## 특징
- Lucene 기반: 검색·질의 처리 로직을 루씬 엔진으로 구성
- Schema-less: 명시적 스키마 정의 없이 문서 색인 가능
- 고가용성: 다수 노드 클러스터로 결함 내성(FTS) 확보
- 벡터 활용성: RAG 시스템의 벡터 DB로 자연어 검색 지원
## 목적
- 대용량 문서 데이터의 실시간 색인·검색·랭킹 제공
- 생성형 AI 시대 RAG 파이프라인의 지식 검색 기반 마련
## 구성요소
- Master Node: 클러스터 상태 관리, 인덱스 생성/삭제, 샤드 할당
- Data Node: 데이터 복제·저장, 인덱싱·검색 수행
- Shard/Index: 데이터 저장 최소단위(Shard)와 논리적 묶음(Index)
- Coordinating Node: 검색·색인 요청 분산 처리 및 결과 병합
- Ingest Node: 색인 전 데이터 전처리(필드 추가·정제)
- Client API: REST API로 Kibana·Filebeat 연계(ELK 스택)
## 구성도
```
Client → [Coordinating Node] → 분산 라우팅
                 ↓
          [Master Node] ── 클러스터 관리
                 ↓
  [Data Node1][Data Node2][Data Node3]
       (Shard + Replica 저장)
```
## 연관 토픽
- [[RAG]] - 검색증강생성
- [[벡터 데이터베이스]] - Milvus, FAISS 비교
- [[ELK 스택]] - Elasticsearch·Logstash·Kibana
- [[역인덱스]] - 전문검색 인덱싱 구조
