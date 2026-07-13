#정보관리기술사 #디지털서비스 #SLAM #자율주행
## 정의
SLAM(Simultaneous Localization And Mapping)
- 미지의 환경에서 자기 위치를 추정하면서 동시에 주변 지도를 작성하는 동시 위치추정·지도작성 기법
- 로봇·자율주행·AR/VR의 핵심 인지 기술
## 키워드
* LiDAR-SLAM, Visual SLAM, EKF, ORB-SLAM, Loop Closure, Sensor Fusion
## 암기법
* 위지동: 위치추정·지도작성·동시수행
## 특징
- 동시성: 위치 추정과 지도 작성을 동시 수행
- 센서 융합성: LiDAR·카메라·IMU 결합
- 동적 적응성: 환경 변화에 맞춰 지도 갱신
- 확률 기반성: EKF·Particle Filter 활용
## 목적
- GPS 부재 환경에서도 자기 위치 인식
- 로봇·자율주행 등 동적 환경 운영 지원
## 구성요소
- 센서: LiDAR, 카메라, IMU, GPS
- 알고리즘: EKF-SLAM, Particle Filter SLAM, Graph SLAM, ORB-SLAM
- 단계: 위치 추정 → 특징점 추출 → 매핑 → Loop Closure
- 응용: 자율주행, AMR, 청소 로봇, AR/VR, 드론
- 분류: LiDAR-SLAM(정확·고가), Visual SLAM(저가·풍부 정보)
## 구성도
```
[센서] LiDAR/Camera/IMU → 특징점 추출
                              ↓
                        [위치 추정]
                              ↓
                        [지도 작성] → Loop Closure (정확도 보정)
                              ↓
                        [지도 + 위치 출력]
```
## 연관 토픽
- [[AMR]] - 자율 이동 로봇
- [[ADS(Automated Driving System)]] - 자율주행
- [[센서 퓨전]] - 센서 퓨전
- [[VLA 모델]] - VLA 모델
