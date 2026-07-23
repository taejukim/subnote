#정보관리기술사 #디지털네트워크 #DHCP #디지털네트워크/OSI/프로토콜
Dynamic Host Configuration Protocol
## 정의 
- 호스트에 IP 주소 할당을 위해 DHCP, Discover, Offer, Requset, Ack의 4단계 할당 과정 이용하는 동적 호스트 IP 자동 할당 프로토콜
## 키워드
- DISCOVER, OFFER, REQUSET, ACK, DHCP, Starvation

## DHCP IP 할당 과정
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260326000946.png|500]]
1. DISCOVER
	1. 클라이언트가 Broadcast로 DHCP Discover 패킷 전송
2. OFFER
	1. 서버가 유니캐스트로 DHCP Offer 패킷 전송
	2. 제안 IP 주소, 임대시간, DNS 정보 등 전달
3. REQUSET
	1. 클라이언트가 Broadcast로 DHCP Request 패킷 전송
	2. 제안 IP 사용 승인 의사 전달
4. ACK
	1. 서버가 유니캐스트로 DHCP Ack 패킷 전송
	2. 제안 IP 사용 최종 승인 및 할당 종료

## DHCP IP 갱신, 해제 과정
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260326001301.png|500]]
- 갱신 과정
	- REQUEST
		- 클라이언트가 유니캐스트로 IP 연장 의사 전달
		- 임대시간 50% 남은 시점 전달
	- ACK
		- 서버가 유니캐스트로 DHCP Ack 패킷 전송
		- 제안 IP 사용 연장 최종 승인 및 할당 종료
- 해제 과정
	- RELEASE
		- 클라이언트가 유니캐스트로 IP 사용 종료 의사 전달
		- 서버 별도 응답 없이 IP 할당 해제 종료