#정보관리기술사 #AI #Dropout #AI/딥러닝_기초_학습/최적화 #NEW
## 정의
Dropout
- 신경망의 과적합을 방지하기 위해 은닉층의 일부 노드를 무작위로 비활성화하여 정규화(성능 일반화)하는 신경망 학습 기법
## 키워드
* 노드 비활성화, Overfitting, co-adaptation(동조현상), dropout rate
## 암기법
* Fast·Adhoc·Connect: Fast Dropout, Ad-hoc Dropout, DropConnect
## 특징
- 무작위 비활성: dropout rate(예: 0.5)로 노드 랜덤 제거
- 동조 회피: co-adaptation 완화, 모델 복잡도 감소
- 앙상블 효과: 매 스텝 다른 부분망 학습 → Voting 효과
- 테스트 시: 노드 복원 후 확률 p와 가중치 w 곱 연산
## 목적
- 과적합 예방 및 일반화 성능 향상
- 은닉층 노드 간 과도한 의존 방지
## 구성요소
- Fast Dropout: 가우시안 마스크로 속도 개선
- Ad-hoc Dropout: 0~1 균일분포 마스크
- DropConnect: 노드 대신 가중치 비활성화
- 학습: Rate 입력 → 노드 비활성 → 학습 → 오류역전파 반복
- 테스트: 비활성 노드 복원 후 p·w 스케일링 추론
## 구성도
```
(a) Standard Net: 전체 연결
(b) Dropout: 은닉 노드 X 표시·연결 제거
학습: Net → 비활성(rate=0.5) → 역전파 → 다른 노드 비활성 반복
```
## 연관 토픽
- [[과적합(Overfitting) 문제]] - 직접 대응
- [[배치 정규화]] - 내부 정규화로 Dropout 대체 가능
- [[정규화 규제화 표준화]] - 규제화 계열
- [[앙상블 학습(Ensemble Learning)]] - 앙상블·Voting 효과
