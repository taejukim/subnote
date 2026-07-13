#정보관리기술사 #자료구조 #AVL트리 #BalancedTree
## 정의
AVL 트리(AVL Tree)
- 각 노드의 왼쪽 서브트리 높이와 오른쪽 서브트리 높이 차이(Balance Factor)가 절대값 1 이하인 균형 이진 탐색 트리
- 삽입·삭제 시 자동으로 회전하여 균형을 유지하는 자가 균형 BST
## 키워드
* Balance Factor, BST, LL/RR/LR/RL Rotation, Self-Balancing, O(log n)
## 암기법
* LRLR: LL·RR·LR·RL 회전
## 특징
- 균형성: BF |≤ 1|로 균형 유지
- 자가 균형성: 회전으로 자동 재균형
- 효율성: 검색·삽입·삭제 모두 O(log n)
- 메모리 비용: 각 노드에 BF/높이 정보 저장
## 목적
- 일반 BST의 편향(Skew) 문제 해결
- 데이터 변동에서도 검색 성능 보장
## 구성요소
- Balance Factor: 왼쪽 높이 - 오른쪽 높이
- 회전 4종: LL, RR, LR, RL
- 삽입/삭제 후 BF 검사·회전 트리거
- 시간 복잡도: 검색·삽입·삭제 O(log n)
- 비교: Red-Black Tree(완화된 균형, 회전 적음)
## 구성도
```
        [Balance Factor: -1, 0, +1 만 허용]

LL 회전:    A           B
           /          / \
          B    →     C   A
         /
        C

RR/LR/RL 회전 등 4가지 회전 케이스로 BF 복원
```
## 연관 토픽
- [[이진 탐색 트리]] - BST
- [[Red-Black Tree]] - 또 다른 균형 BST
- [[B-Tree]] - 디스크용 균형 트리
- [[해시 테이블]] - 검색 자료구조 비교
