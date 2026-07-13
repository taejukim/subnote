#정보관리기술사 #데이터베이스 #ANN #데이터베이스/NoSQL/분산 #NEW
## 정의
ANN(Approximate Nearest Neighbor)
- 고차원 벡터 공간에서 주어진 쿼리 벡터에 가장 가까운 이웃을 빠르게 찾기 위한 근사 최근접 이웃 알고리즘
## 키워드
* 고차원 벡터 유사성 탐색, k-d tree, LSH, HNSW, NSG, IVF, PQ, Vector DB
## 암기법
* 공그압: 공간분할·그래프·압축/양자화
## 특징
- 근사성: 정확 NN 대신 근사로 속도 확보
- 고차원 대응: Exact NN의 차원의 저주 완화
- 인덱스 다양성: 트리·해시·그래프·양자화
## 목적
- 벡터 DB·유사도 검색에서 빠른 최근접 이웃 탐색
## 구성요소
- 공간 분할 기반: 벡터 공간을 부분공간으로 분할 후 관련 영역 탐색 (k-d tree, Annoy, LSH)
- 그래프 기반: 근접 그래프로 이웃 탐색, 정확·효율 높고 구축 비용 큼 (HNSW, NSG)
- 압축·양자화 기반: 차원 축소·이산 코드로 거리 계산 가속 (PQ, IVF)
- 절차(예): 임의 두 점으로 hyperplane 분할 → 이진트리 갱신 → K개 초과 시 재분할 → subspace에서 NN 탐색
## 구성도
```
[쿼리 벡터] → [인덱스 탐색]
  ├─ Space Partition (k-d/LSH)
  ├─ Graph (HNSW/NSG)
  └─ Quantization (PQ/IVF)
        ↓
   [근사 최근접 이웃]
```
## 연관 토픽
- [[Vector DB]] - 벡터 데이터베이스
- [[NoSQL]] - 비정형·분산 저장
- [[해시 테이블]] - LSH 기반
