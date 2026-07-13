#정보관리기술사 #데이터베이스 #MapReduce #빅데이터처리
## 정의
MapReduce
- 대규모 데이터를 분산 환경에서 병렬 처리하기 위한 프로그래밍 모델
- Map(매핑) → Shuffle → Reduce(집계) 단계로 데이터를 분산 처리하는 빅데이터 처리 패러다임
## 키워드
* Hadoop, HDFS, Map, Reduce, Shuffle, 분산 처리, YARN
## 암기법
* 매셔리: 매핑·셔플·리듀스
## 특징
- 분산 처리성: 다수 노드에서 병렬 실행
- 단순 모델성: Map·Reduce 함수만 작성
- 확장성: 수평 확장 용이
- 내고장성: 노드 장애 시 자동 재시도
## 목적
- 페타바이트급 데이터의 분산 병렬 처리
- 단순한 프로그래밍 모델로 빅데이터 활용
## 구성요소
- Map 단계: 입력 → (key, value) 매핑
- Shuffle 단계: 동일 key 데이터 그룹화·정렬
- Reduce 단계: key별 집계
- 인프라: HDFS(저장), YARN(자원 관리)
- 사례: WordCount, Log Analysis, ETL
- 한계: 디스크 기반 → Spark 등장으로 메모리 기반 대체
## 구성도
```
[Input Data]
     ↓ Split
[Map] (key1, val1) (key1, val2) (key2, val3) ...
     ↓ Shuffle/Sort (같은 key 모음)
[Reduce] key1 → 집계 / key2 → 집계 ...
     ↓
[Output]
```
## 연관 토픽
- [[Hadoop HDFS]] - HDFS 분산 파일시스템
- [[NoSQL]] - NoSQL DB
- [[데이터 파이프라인]] - 데이터 파이프라인
- [[데이터 레이크하우스]] - Lakehouse
