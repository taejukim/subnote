#정보관리기술사 #보안 #SOC #보안관제 #보안/보안관제 #NEW
## 정의
SOC(Security Operations Center)
- 조직의 보안 이벤트·위협을 상시 모니터링·탐지·분석·대응·보고하는 보안 운영 조직/센터
- People·Process·Technology를 통합해 사이버 위협에 대한 가시성과 대응력을 제공
## 키워드
* SOC, 보안관제, Monitor, Detect, Respond, SIEM, SOAR, XDR
## 암기법
* "모디응PPT" - Monitor·Detect·Respond + People·Process·Technology
## 특징
- 24×7 관제: 로그·트래픽·엔드포인트 이벤트의 연속 수집·상관분석
- 계층 대응: L1 트리아지 → L2 분석 → L3 헌팅/IR의 역할 분담
- 자동화 연계: SOAR 플레이북으로 반복 대응 자동화, 분석가 집중도 향상
- 위협 인텔 융합: TI·ATT&CK 기반으로 탐지 규칙·헌팅 가설 고도화
## 목적
- 침해·이상행위의 조기 탐지와 신속한 격리·복구
- 보안 운영의 표준화·가시화·측정(KPI: MTTD, MTTR 등)
## 구성요소
- People: 분석가, 헌터, IR, 매니저 등 역할·숙련도·교대 운영
- Process: 모니터링, 알림 트리아지, 에스컬레이션, IR·사후분석(Post-Incident)
- Technology: SIEM(수집·상관), SOAR(오케스트레이션), XDR/EDR/NDR(탐지 센서)
- 산출물: 대시보드, 티켓, 인시던트 리포트, 개선(Detection Engineering)
## 구성도
```
[로그/텔레메트리] → SIEM ←→ XDR/EDR/NDR
         │              │
         ▼              ▼
      [SOC 관제] ── SOAR Playbook
   Monitor → Detect → Analyze → Respond → Report
         │
    People · Process · Technology
```
## 연관 토픽
- [[SIEM]] - 보안 이벤트 수집·상관·알림의 중심 플랫폼
- [[SOAR]] - 대응 자동화·오케스트레이션
- [[XDR]] - 크로스 레이어 탐지·대응 확장
- [[위협 헌팅]] - 알림 너머 능동 탐색
- [[사이버 레질리언스]] - 탐지·대응을 넘어 비즈니스 연속성
