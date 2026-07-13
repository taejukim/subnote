#정보관리기술사 #디지털네트워크 #PassiveWiFi #IoT #NEW
## 정의
Passive WiFi
- 전력 소모가 큰 RF 생성부를 분리하고 후방산란(Backscatter)로 데이터를 전송하는 초저전력 WiFi 기술
- 후방산란: 전파가 진행 반대 방향으로 되돌아가는 현상 이용
## 키워드
* 사물인터넷, Backscatter, Digital Equipment, Analog RF
## 암기법
* 분후초: 분리·후방산란·초저전력
## 특징
- 초저전력: Passive Device는 RF를 직접 생성하지 않음
- 구조 분리: Plugged-in(아날로그 RF) ↔ Passive(반사 전송)
- 기존 WiFi: Baseband(~10μW)+RF(~100mW)가 한 기기에 집약
- IoT 적합: 배터리 수명 연장·대기 전력 최소화
## 목적
- IoT 단말의 장기 배터리 구동
- WiFi 모듈 RF 전력 소모 획기적 감소
## 구성요소
- Plugged-In: RF Transfer(Up/Down Converter), RF Calibration, MAC
- Passive Device: Backscattering로 공중 신호 반사·정보 전송
- WiFi Receiver: 스마트폰 등에서 WiFi 신호 수신
## 구성도
```
[Plugged-in RF Source] ──전파──▶ [Passive Device]
                                      │ Backscatter
                                      ▼
                               [WiFi Receiver]
기존: [Digital~10μW + Analog RF~100mW] 단일 기기
```
## 연관 토픽
- [[Wi-Fi7(IEEE 802.11be)]] - 고속 WiFi 표준
- [[매터(Matter)]] - IoT 상호운용
- [[SDR]] - 소프트웨어 정의 라디오
