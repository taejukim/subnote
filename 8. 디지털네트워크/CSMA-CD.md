#정보관리기술사 #디지털네트워크 #CSMA-CD #디지털네트워크/MAC/매체접근
CSMA/CD(Carrier Sense Multiple Acess/Collision Detection)
## 정의
- 각각의 호스트가 링크를 사용하기 전에 링크의 사용 상태를 감지하여 전송 충돌을 최소화 하기 위한 프로토콜
## 키워드
- 1-Persistent, Non-Persistent, P-Persistent, 충돌, Back-off

## 동작 원리
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260325223518.png|500]]
- 송진 준비
	- 송싱데이터 준비 : 송신이 필요한 디바이스에서 송신을 위해 데이터 준비
- 채널 감시
	- 채널 Free : 데이터 송신 후 채널 감시, 미충돌 시 프에니 전송 완료
	- 충돌 발생 : Jamming Signal 전송하여, Back-off 방식에 따라 대기 및 재전송 시도
	- 채널 Busy : 데이터 송신을 위해, 채널 재 탐색 수행
## 1-Persistent의 동작 원리
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260325223659.png|500]]
- 지국이 회선이 휴지 상태인 것을 감지하면 즉시 프레임을 전송
- 채널이 Idlee 상태일 때마다 1의 확률을 가지고 프레임을 전송

## Non-Persistent의 동작 원리
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260325223752.png|500]]
- 전송할 프레임이 있는 지국이 회선을 감지하는 특징
- 채널 사용되는 것 감지 시, 임의의 시간동안 데이터 전송 지연

## P-Persistent의 동작 원리
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260325223840.png|500]]
- 1-Persistent와 Non-Persistent의 장단점을 상호 보완하는 특징
- 확률값(p)를 이용하여 전송여부 결정
