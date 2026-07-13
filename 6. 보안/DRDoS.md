#정보관리기술사 #보안 #DRDoS #반사증폭 #NEW
## 정의
DRDoS(Distributed Reflection DoS)
- 별도 에이전트 설치 없이 네트워크 프로토콜 구조 취약점을 이용해, 정상 서비스 시스템을 경유 에이전트로 활용하는 DDoS 기법
## 키워드
* 프로토콜 취약점, Source IP Spoofing, Bot 감염 불필요, 경유지 서버, 반사, 증폭, NTP/DNS/SNMP/CHARGEN, PPS·BPS
## 암기법
* 스반거: Spoofing → 반사(Reflection)·증폭 → 서비스거부
## 특징
- Bot 불필요: 정상 서비스 서버를 반사체로 활용
- IP Spoofing: 송신 IP를 피해자로 위조
- 증폭성: 소량 Request → 대량 Response (예: 30B → 3,000B)
- 프로토콜 의존: DNS·NTP·SNMP·CHARGEN 등
## 목적
- 피해자 서버에 대량 응답 폭주로 서비스 거부
- Botnet 없이 대규모 DDoS 수행
## 구성요소
- 절차: IP Spoofing → Reflection·Amplification → Service Down
- DNS: RR(ANY/TXT 등) 대량 조회
- NTP: MONLIST로 최근 접속 목록 요청
- SNMP: GetBulkRequest로 MIB 대량 요청
- CHARGEN: 대량 문자열 응답 유도
- 대응: 피해자 IP/Port 필터링, 반사체 SYN 소스 블랙리스트, ISP Egress Filtering, RAW Socket 제한
## 구성도
```
[해커] --① IP Spoofing(Victim IP)--→ [경유지: DNS/NTP/SNMP/CHARGEN]
                                              |
                         ② Reflection·Amplification (대량 Response)
                                              ↓
                                         [Victim] ③ DoS
```
## 연관 토픽
- [[DoS, DDoS, Model DoS]] - 서비스 거부 공격
- [[스니핑과 스푸핑]] - IP Spoofing
- [[DNS 싱크홀]] - 봇넷 C&C 차단
- [[DNSSEC]] - DNS 보안 확장
