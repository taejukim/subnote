#정보관리기술사 #보안 #SSRF #보안/개발보안
Server Side Request Forgery
## 정의
- 서버 측에 위조된 HTTP 요청을 발생시켜 직접적인 접근이 제한된 서버 내부 자원에 접근하여 외부로 데이터 유출 및 오동작을 유발하는 공격

## 키워드
- 서버측 요청 조작, 내부 네트워크 스캔, 원격 코드 실행, Non-Blind SSRD, Blind SSRF

## SSRF 공격 절차
![[1. ITPE/0. Sub-Note/99.attached_file/Pasted image 20260409003547.png|600]]

| 절차             | 설명                                     |
| -------------- | -------------------------------------- |
| 1. URL 변조 요청   | 네트워크 스캔 통해 SSRF 취약점 웹서버 발견, URL 변조 요청  |
| 2. 백엔드로 요청 전달  | 웹 서버는 방화벽이 있는 Private Network 서버 요청 전달 |
| 3. 내부 주요 정보 요청 | Private Network의 서버가 내부 작업(DB 등) 수행    |
| 4. 백엔드 결과 응답   | 공격자에게 필요한 정보 전송                        |

## SSRF(Server-Side Request Forgery) 공격 유형

| 내용                 | 설명                                                   |
| ------------------ | ---------------------------------------------------- |
| **Non-blind SSRF** | 공격자가 악의적 요청을 하고 그 결과 서버가 반환되는 데이터가 노출되는 SSRF 공격 유형   |
| **Blind SSRF**     | 공격 데이터를 유출시키는 것이 아니라 유해한 작업을 수행하는 데 초점을 둔 SSRF 공격 유형 |

## SSRF(Server-Side Request Forgery) 대응 방안

|내용|설명|
|---|---|
|One Time Token 사용|예측 불가능한 토큰 값을 매 요청 인증 시 사용|
|입력값 검증|입력된 값, 전송 파라미터의 유효성 검증|
|쿠키 관리|쿠키 내 중요정보 미포함, 쿠키 외 추가 인증 처리|
|인증 강화|민감 데이터에 대한 인증 강화 (재인증 요청 등)|
|From Network Layer|- Segment remote resource access functionality  <br>- Enforce "deny by default" firewall policies|
|From Application Layer|- Enforce the URL schema, port with a positive allow list  <br>- Disable HTTP redirections|


## SSRF와 CSRF(Cross-Site Request Forgery) 비교

|비교 항목|SSRF|CSRF|
|---|---|---|
|공격 위치|Server-Side|Client-Side|
|공격 대상|직접 접속 불가능한 내부 서버|Client에서 연결 가능한 서버|
|공격 요청|신뢰된 서버로부터의 요청|인가된 사용자의 요청|
|필수 요소|외부 접근 가능한 SSRF 취약 서버|정상 사용자|
