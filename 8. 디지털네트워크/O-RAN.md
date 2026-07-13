#정보관리기술사 #디지털네트워크 #ORAN #5G #NEW
## 정의
O-RAN(Open Radio Access Network)
- RAN 구간에 가상화를 적용해 H/W·S/W를 분리하는 Apache 2.0 기반 개방형 아키텍처
- 멀티 벤더 상호운용과 지능형 RAN 제어를 목표로 함
## 키워드
* 무선접속망 규격 통일, 가상화, O-RU, O-DU, O-CU
## 암기법
* RU-DU-CU: 라디오·분산·중앙 단위
## 특징
- 개방성: 표준 인터페이스·Apache 2.0 라이선스
- 분리: RU/DU/CU 기능 분리·가상화
- 지능화: RIC(near-RT / non-RT)로 자원·간섭 최적화
- 멀티벤더: Fronthaul/Midhaul/Backhaul 개방 연동
## 목적
- 벤더 종속 해소 및 CAPEX/OPEX 절감
- AI 기반 RAN 자동화·최적화
## 구성요소
- RIC: 데이터 수집·분석으로 RAN 자원 제어(near-RT, non-RT)
- O-CU: RRC·SDAP·PDCP, CU-CP/CU-UP, Midhaul로 다수 O-DU 제어
- O-DU: RLC·MAC·High PHY, O-RU 인접 분산 단위
- O-RU: DFE·RF·Low PHY·Beamforming, Fronthaul로 O-DU 연결
- 인터페이스: A1(non-RT↔near-RT), E2(RIC↔CU/DU), F1(CU↔DU), Open FH(DU↔RU)
## 구성도
```
[SMO / RIC non-RT]
        │ A1
[RIC near-RT] ──E2──┐
        │           │
   [O-CU CP─E1─UP]  │
        │ F1        │
     [O-DU] ←───────┘
        │ Open Fronthaul
     [O-RU]
```
## 연관 토픽
- [[O-RAN AI-RAN]] - O-RAN 지능화
- [[AI-RAN]] - AI 접목 RAN
- [[C-RAN]] - 중앙집중형 RAN
- [[NFV]] - 네트워크 기능 가상화
