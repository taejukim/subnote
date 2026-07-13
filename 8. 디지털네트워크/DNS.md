#정보관리기술사 #디지털네트워크 #DNS #디지털네트워크/OSI/프로토콜
Domain name System
## 정의
- Host Name 또는 URL을 IP Address로 변환하기 위한 프로토콜
## 키워드
- Recursive, Iterative

## 동작 원리 개념도
![[Pasted image 20260325233238.png|600]]

## 동작원리 설명
| **단계** | **설명**                                                               |
| ------ | -------------------------------------------------------------------- |
| **1**  | Client는 자신에게 등록된 DNS 서버에 `www.test.com`의 IP 질의 (**Recursive Query**) |
| **2**  | 로컬 DNS 서버에 등록되지 않은 이름은 Root DNS 서버에 질의 (**Iterative Query**)         |
| **3**  | Root DNS 서버는 자신이 관리하는 TLD(`.com`)의 DNS 서버 IP 제공                      |
| **4**  | 로컬 DNS 서버는 TLD(`.com`) DNS 서버에 질의                                    |
| **5**  | `.com` DNS 서버는 `test.com` 도메인의 DNS 정보 제공                             |
| **6**  | 로컬 DNS 서버는 `test.com`의 DNS 서버인 `ns.test.com`에 질의                     |
| **7**  | `ns.test.com`은 자신의 레코드 중 `www` 호스트명의 IP를 제공                          |
| **8**  | 로컬 DNS 서버는 Client에 해당 IP를 제공                                         |
| **9**  | Client는 로컬 DNS 서버로부터 제공받은 IP Address로 `www.test.com`에 접속             |

## 주요 기능
| **기능**                   | **상세 내용**                                       |
| ------------------------ | ----------------------------------------------- |
| **Name Resolution**      | URL을 IP Address로 변환                             |
| **Host Aliasing**        | 단일 IP Address를 보유한 호스트에 다양한 별칭(CNAME 등) 부여      |
| **Mail Server Aliasing** | 해당 도메인의 메일 서버(MX 레코드) 정보 제공                     |
| **Load Distribution**    | 단일 URL(Host Name)에 복수개의 IP Address 설정을 통한 부하 분산 |