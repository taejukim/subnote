#정보관리기술사 #데이터베이스 #FP-Growth #데이터베이스/빅데이터/분석 #NEW
## 정의
FP-Growth(Frequent Pattern-Growth)
- 후보 항목집합을 생성하지 않고 트랜잭션을 압축한 FP-Tree에서 빈발 항목집합을 빠르게 찾는 알고리즘
## 키워드
* FP-Tree, 조건부 패턴 베이스, 조건부 FP-Tree
## 암기법
* 지지트조패트: 지지도·정렬·Tree·패턴베이스·조건부Tree
## 특징
- 후보 생성 제거: Apriori/DHP와 차별
- 압축 구조: 공통 경로 공유 FP-Tree
- Header Table + Node Link로 빠른 탐색
## 목적
- 후보 폭증 없이 빈발 패턴을 효율적으로 마이닝
## 구성요소
- ① 지지도 계산·빈발 항목 추출
- ② 지지도 내림차순 정렬
- ③ FP-Tree·Header Table 생성(공통경로 공유, count 저장)
- ④ 조건부 패턴 베이스 수집
- ⑤ 조건부 FP-Tree 생성·가지치기
- ⑥ 재귀적 빈발 패턴 확장 → Frequent Itemsets
## 구성도
```
[트랜잭션] → 빈발추출·정렬 → [FP-Tree + Header]
  → 조건부 패턴 베이스 → 조건부 FP-Tree
  → 빈발 항목집합
```
## 연관 토픽
- [[Apriori]] - 후보 생성 방식
- [[DHP]] - 해시·가지치기
- [[연관성 분석]] - 연관규칙
