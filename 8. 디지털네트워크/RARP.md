#정보관리기술사 #디지털네트워크 #RARP #디지털네트워크/OSI/프로토콜
Reverse Address Resolution Protocol
## 정의
- IP호스트가 자신의 물리 네트워크 주소(MAC)는 알지만 IP주소를 모르는 경우, 서버로 부터 IP주소를 요청하기 위해 사용하는 프로토콜
## 키워드
- MAC을 IP로 변환

## 동작원리
- RARP Request
	- ![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260326000732.png|500]]
	- RARP의 주소를 모르기 때문에 RARP Request Broadcast
	- RARP Request는 네트워크 모든 컴퓨터가 수신, RARP서버만 응답
	- RARP Request is Broadcast
- RARP Response
	- ![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260326000744.png]]
	- RARP 서버가 2대 이상 있을 경우, 두 대 모두 응답
	- A는 Response가 2개 이상일 때는 첫번째 Response만 수신, 나머지 무시
	- RARP Replay is Unicast

