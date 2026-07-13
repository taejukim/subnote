#정보관리기술사 #디지털네트워크 #NWDAF #디지털네트워크/5G/6G
Network Data Analytics Function
## 정의
- 네트워크 운영 중 발생하는 다양한 정보를 수집해 AI 모델을 만들고, 이 모델을 기반으로 네트워크를 실시간으로 제어 기능을 수행하는 3GPP에서 정의한 표준기술이며 네트워크 장비
## 키워드
- AnLF, MTLF, DCCF, ADRF, MFAF
## 구성도
![[Pasted image 20260326002954.png|500]]
## 표준기능
| **구분**                                                           | **핵심 기능**                       | **설명**                                                                                                              |
| ---------------------------------------------------------------- | ------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **AnLF**<br>(Analytics Logical Function)                         | - 분석 논리 함수<br>- 머신 러닝(ML) 기반 추론 | - 추론을 수행하는 NWDAF의 논리적 기능으로, 분석 정보를 도출(Analytics Consumer 요청 기반 통계/예측)하여 분석 서비스 제공<br>- 분석 요청을 수집하고 소비자에게 응답을 보내는 역할 |
| **MTLF**<br>(Model Training Logical Function)                    | - 모델 학습 논리 함수<br>- 머신 러닝(ML) 학습 | - ML 모델을 학습하고, 새롭게 학습된 모델을 제공<br>- 모델 추론 마이크로 서비스를 학습하고 배포하는 역할                                                     |
| **DCCF**<br>(Data Collection Coordination and Delivery Function) | - 데이터 요청 관리                     | - 동일 요청이 있을 경우 기존 결과를 NWDAF에 직접 전송<br>- 새로운 요청일 경우 데이터 공급자(OAM/NF)로부터 데이터 전송 수행                                     |
| **ADRF**<br>(Analytical Data Repository Function)                | - 분석 데이터 저장소                    | - 분석 및 학습에 필요한 과거 데이터를 저장                                                                                           |
| **MFAF**<br>(Messaging Framework Adaptor Function)               | - 메시징 프레임워크 어댑터 기능              | - 수집된 데이터를 NWDAF(AnLF)에게 전달하는 가교 역할                                                                                 |