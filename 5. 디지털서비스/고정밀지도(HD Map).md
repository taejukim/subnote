#정보관리기술사 #디지털서비스 #HDMap #자율주행 #NEW
## 정의
고정밀지도(HD Map, High-Definition Map)
- 자율주행 안전을 위해 도로·차선·표지·구조물을 cm 단위 3D로 표현한 기계 판독형 고해상도 지도
## 키워드
* LiDAR, NDT, SLAM, 4계층, V2X, Edge-Cloud-OTA
## 암기법
* 기차시동: 기하·차선·시설·동적 4계층
## 특징
- 4계층: 기하·지형, 차선·노면, 시설·랜드마크, 동적(V2X)
- 최신화: Crowdsourcing, SLAM/ICP/NDT, Edge-Cloud-OTA
- 자동생성: DL·Semantic Segmentation, 3D NDT, Vectorization
## 목적
- 자율주행 차량 고정밀 위치·경로 계획
- 실시간 교통·신호 연동
## 구성요소
- 생성 5단계: 계획→수집(MMS/LiDAR)→정합→모델링→검수·배포
- 기술: FEAT2MAP, Topology, Point Cloud Mapping
## 구성도
```
LiDAR/GNSS → 4계층 HD Map → V2X 동적정보 → 자율주행
```
## 연관 토픽
- [[LDM]] - Local Dynamic Map
- [[SLAM]] - 동시 위치·지도
- [[ADS(Automated Driving System)]] - 자율주행
