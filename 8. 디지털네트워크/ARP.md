#정보관리기술사 #디지털네트워크 #ARP #디지털네트워크/OSI/프로토콜
Address Resolution Protocol
## 정의
- LAN 환경에서 논리 주소인 IP 주소를 물리 주소인 MAC 주소로 변환해 주는 네트워크 계층의 프로토콜
## 키워드
- IP를 MAC으로 변환

## 동작 원리
- MAC Address 요청
![[Pasted image 20260325235857.png|500]]
1. 호스트A는 호스트D의 IP를 인지한 상태에서 호스트D와의 통신을 위해 D의MAC 주소 획득 필요
2. 호스트A는 ARP Request 패킷을 생성(Source IP와 MAC은 자신의 주소로, Destination IP는 호스트D의 IP로 Destination MAC은 FF:FF:FF:FF:FF:FF로 채워 넣음)
3. 호스트A는 생성된 ARP 패킷을 네트워크로 브로드 캐스트
- MAC Address 회신
	- 호스트D는 수신받은 ARP Request 패킷에서 Destination IP가 자신의 주소인 것을 확인하고 ARP 처리 시작
	- 호스트D는 ARP Replay 패킷을 생성(Destination IP와 MAC은  ARP Reuqest 패킷의 Source IP와 MAC으로 Source IP와 MAC은 자신의 주소로 채워 넣음
	- 호스트D는 ARP 패킷을 호스트A로 유니 캐스트
	- 호스트 A는 ARP Replay 패킷을 가지고 해당 MAC으로 자신의 ARP Cache 테이블을 수정하고 호스트D와 통신
