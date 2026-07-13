#정보관리기술사 #디지털서비스 #12Factor #15Factor
## 정의
12 Factor / 15 Factor
- 12 Factor App: Heroku가 제안한 SaaS·클라우드 네이티브 앱 설계 12가지 원칙
- 15 Factor App: 12 Factor에 인증·텔레메트리·API First 등 3가지 원칙을 추가한 확장 모델
## 키워드
* SaaS, Cloud Native, Stateless, 12-Factor, API First, Telemetry
## 암기법
* 코설구의: 코드베이스·설정·구성요소·의존성
## 특징
- 클라우드 친화성: 컨테이너·K8s 환경 최적
- 무상태 지향성: 수평 확장 용이
- 환경 분리성: 설정 환경 변수 분리
- 운영 친화성: 로깅·모니터링·텔레메트리 표준
## 목적
- 클라우드 네이티브 SaaS 앱 설계 표준 제공
- 확장성·유지보수성·이식성 확보
## 구성요소
- 12 Factor:
  1. Codebase 2. Dependencies 3. Config 4. Backing Services
  5. Build/Release/Run 6. Processes 7. Port Binding 8. Concurrency
  9. Disposability 10. Dev/Prod Parity 11. Logs 12. Admin Processes
- 15 Factor 추가:
  13. API First
  14. Telemetry
  15. Authentication and Authorization
- 실제 적용: K8s, Docker, CI/CD, GitOps
## 구성도
```
[12 Factor] 클라우드 네이티브 앱 설계 12원칙
       +
[+3 (15 Factor)] API First · Telemetry · Auth
       =
[Cloud-Native SaaS App] (K8s/Container 친화)
```
## 연관 토픽
- [[클라우드 네이티브]] - 클라우드 네이티브
- [[컨테이너(Container)]] - 컨테이너
- [[쿠버네티스(Kubernetes)]] - K8s
- [[GitOps]] - GitOps
