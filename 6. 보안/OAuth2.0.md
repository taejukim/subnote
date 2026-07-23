#정보관리기술사 #보안 #OAuth2 #보안/인증/접근제어
Open Authorize 2.0
## 정의
- Third-Party 프로그램에게 리소스 소유자를 대신하여 리소스 서버에서 제공하는 자원에 대한 접근 권한을 위임하는 개방형 표준 프로토콜

## 키워드
- 권한 부여 방식 
	- Authorization Code
	- Implicit
	- Password Credentials
	- Client Crendentials
- Token Type
	- SAML
	- Simple Web Token
	- JSON Web Token
## Oauth 인증 절차
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260410223407.png|500]]

|구성요소|설명|
|---|---|
|자원 소유자 (Resource Owner)|보호된 자원(데이터/서비스)에 접근 권한을 부여하는 사용자|
|클라이언트 (Client)|자원 소유자의 자원 접근을 요청하는 애플리케이션 (제3자 서비스)|
|자원 서버 (Resource Server)|Access Token을 검증하고 자원을 제공하는 서버|
|권한 서버 (Authorization Server)|인증 후 Access Token을 발급하는 서버|
|액세스 토큰 (Access Token)|보호된 자원 접근을 위한 권한 증명|
|리프레시 토큰 (Refresh Token)|Access Token 만료 시 재발급을 위한 토큰|
|클라이언트 ID|클라이언트를 식별하는 값 (권한 서버 발급)|
|클라이언트 시크릿|클라이언트 인증을 위한 비밀값|
## Oauth 인증 유형
| 유형                                        | 설명                                                     |
| ----------------------------------------- | ------------------------------------------------------ |
| Authorization Code Grant                  | - Authorization Code를 발급받아 토큰으로 교환- 보안성이 높고 가장 권장되는 방식 |
| Implicit Grant                            | - 별도 교환 과정 없이 Access Token 즉시 발급- 보안 취약으로 현재는 사용 지양    |
| Resource Owner Password Credentials Grant | - ID/PW로 직접 토큰 발급- 신뢰 관계에서만 제한적으로 사용                   |
| Client Credentials Grant                  | - Client ID/Secret으로 토큰 발급- 서버 간 통신에 사용                |
