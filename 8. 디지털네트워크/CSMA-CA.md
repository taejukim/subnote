#정보관리기술사 #디지털네트워크 #CSMA-CA #디지털네트워크/MAC/매체접근
CSMA-CA(Carrier Sense Multiple Access/Collison Avoidance)
## 정의
- **무선랜** 환경에서 회선 상태를 모니터링하여 충돌을 미리 예측, 충돌 가능성을 최소화하는 접속기법

## 키워드
- DIFS, RTS, SIFS, CTS, SIFS(NAV)

## 동작 원리
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260325224054.png|500]]
1. 채널 사용 여부 검사
	1. RTS 프레임을 보내고 CTS응답 받기
	2. CTS 응답이 없으면 반복
2. IFS(Inter Frame Space) 주기 동안 대기 
	1. SIFS(Short IFS), PIFS(PCF IFS), DIFS(DCF IFS)
3. Back off time 동안 대기
4. 프레임 전송
5. ACK 메시지 수신 : ACK 메시지를 수신하여 프레임의 정상 전달 여부 확인

## IFS(Inter Frame Space)와 Contention Window
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260325224315.png|500]]
- IFS(Inter Frame Space) 
	- 휴지 상태릐 채널이 발견되면 지국을 즉시 전송하지 않고 IFS라는 일정 시간을 기다림
	- IFS 시간으로 인해 멀리 떨어진 지국이 보낸 신호의 앞부분이 도달할 수 있도록 여유를 둠
	- 만약 IFS시간 동안에도 휴지 상태이면 지국은 보낼 수 있으나 아직 경쟁 구간이라 불리는 시간동안 기다림 
- 경쟁윈도우(Contention window)
	- 시간 슬롯으로 나뉘어 있는 일정 시간, 임의의 수를 선택하여 기다리는 휴지 시간
	- 1개 슬롯으로 시작, 매범 휴지 채널을 발견 못할 때마다 두배씩 슬롯 증가(p-지속 방식과 유사)
	- 채널이 사용 중인 것이 감지되면 지국은 과정을 다시 시작 하지 않고 타이머만 멈추기 때문에 가장 오랜 기다린 지국이 우선순위를 가짐