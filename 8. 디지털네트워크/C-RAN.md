#정보관리기술사 #디지털네트워크 #CRAN #5G #NEW
## 정의
C-RAN(Centralized / Cloud RAN)
- 기지국의 DU와 RF를 분리해 다수 기지국의 DU를 중앙 집중 처리하고 RF(RU/RRH)는 서비스 지역에 분산하는 무선 접속망
- 클라우드형 중앙 DU로 셀 간 간섭 조정·협력 통신을 용이하게 함
## 키워드
* DU·RF 분리, RU, CPRI, OBSAI, ORI
## 암기법
* 중분: 중앙 DU + 분산 RU
## 특징
- 기능 분리: 디지털부(DU) 집중, 무선부(RU/RRH) 분산
- Fronthaul: DU–RRH를 CPRI/OBSAI/ORI로 연결
- 간섭 조정: 중앙 DU에서 셀 간 협력·품질 향상
- 클라우드화: DU를 데이터센터형으로 집약
## 목적
- 기지국 처리 효율화·운영비 절감
- 협력 통신·간섭 제어로 무선 품질 향상
## 구성요소
- RU(RRH): DU 디지털→RF 변환·증폭, 안테나 송수신
- Centralized DU: 클라우드 집중 처리, 셀 간 간섭·협력 통신
- CPRI: REC(DU)–RE(RU) 간 사용자·제어·동기 프레임 송수신
- OBSAI: 모듈 간 RP로 개방형 기지국 구조 지향(CPRI 경쟁)
- ORI: ETSI 주도, CPRI 호환 한계 개선·벤더 상호운용
## 구성도
```
[RRH]─┐
[RRH]─┼─ Fronthaul(CPRI/ORI) ─ [Centralized DU] ─ [PoP] ─ [Packet Core]
[RRH]─┘
```
## 연관 토픽
- [[O-RAN]] - 개방형 RAN 아키텍처
- [[RAN Sharing]] - 무선접속망 공유
- [[NFV]] - 클라우드·가상화 기반
- [[5G IMT-2020]] - 5G 무선접속
