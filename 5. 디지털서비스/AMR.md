#정보관리기술사 #디지털서비스 #AMR #자율이동로봇
## 정의
AMR(Autonomous Mobile Robot)
- 환경을 자율적으로 인식하고 경로를 동적으로 계획해 이동하는 자율형 이동 로봇
- AGV와 달리 SLAM·AI 기반으로 가이드 인프라 없이 운영 가능
## 키워드
* SLAM, LiDAR, RaaS, AGV 비교, Fleet Management, 물류 자동화
## 암기법
* 인경자: 인식·경로계획·자율이동
## 특징
- 자율성: 가이드 라인·마커 없이 동적 경로 생성
- 적응성: 장애물·동적 환경 대응
- 통합성: WMS·MES·ERP와 연계
- 확장성: Fleet 운영·다대다 협업
## 목적
- 물류·제조·서비스 산업의 자동화·생산성 향상
- 인력 의존 감소와 24/7 운영 가능
## 구성요소
- 센서: LiDAR, 카메라, IMU, 초음파
- 인지·판단: SLAM, 객체 인식, 경로 계획
- 제어: 모션 제어, 안전 정지
- 운영: Fleet Management System, RaaS
- AGV 비교: AGV(가이드 의존, 정해진 경로) vs AMR(자율, 동적 경로)
## 구성도
```
[센서: LiDAR/Camera] → [SLAM·인지]
                          ↓
                    [경로 계획·판단]
                          ↓
                    [모션 제어·안전]
                          ↑ Fleet Management 통신 ↑
```
## 연관 토픽
- [[Robot as s service]] - RaaS
- [[SLAM]] - 동시 위치추정·지도작성
- [[휴머노이드 로봇]] - 휴머노이드
- [[스마트 팩토리(Smart Factory)]] - 스마트 팩토리
