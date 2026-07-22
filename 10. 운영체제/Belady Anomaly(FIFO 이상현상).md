#운영체제 #Belady #FIFO #필수 #운영체제/메모리관리 #NEW
## 정의
Belady's Anomaly (FIFO 이상현상)
- FIFO 페이지 교체에서 프레임 수를 늘렸음에도 Page Fault가 오히려 증가하는 현상
## 키워드
* FIFO, Page Fault 증가, Frame 증가, LRU, OPT, Locality, PFF, Working Set
## 암기법
* 프레임↑인데 Fault↑ = Belady
## 구성요소/특징/유형
| 항목 | 내용 |
| ---- | ---- |
| 원인 | FIFO가 Locality 미고려 |
| 영향 | 성능 저하, Thrashing 유발 |
| 극복 | LRU·OPT 사용, PFF·Working Set |
## 연관 토픽
- [[페이지 교체 알고리즘]] - FIFO
- [[스레싱]] - 연쇄 영향
- [[지역성]] - 극복 원리
