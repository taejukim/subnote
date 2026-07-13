#정보관리기술사 #프로젝트관리 #NoOps
## 정의
NoOps(No Operations)
- 운영 업무의 자동화·서버리스화로 별도 운영 인력의 개입을 최소화하는 운영 패러다임
- 클라우드 관리형 서비스를 활용해 개발자가 운영을 책임지는 형태
## 키워드
* Serverless, FaaS, IaC, 자동화, 관리형 서비스, GitOps
## 암기법
* 자관무서: 자동화·관리형·무인·서버리스
## 특징
- 자동화: 배포·확장·복구 자동화
- 추상화: 인프라 관리 부담 제거
- 관리형: 클라우드 관리형 서비스 의존
- 책임전이: Dev 팀이 운영 책임
## 목적
- 운영 인력 부담 최소화로 개발 속도 향상
- 클라우드 자원 효율화와 신뢰성 확보
## 구성요소
- Serverless/FaaS: AWS Lambda, Cloud Run
- 관리형 DB: Aurora, Cloud SQL
- IaC: Terraform, CloudFormation
- 관측성: 메트릭·로그·알림 자동화
## 구성도
```
Code 커밋 → CI/CD → IaC 프로비저닝 → Serverless 배포 → 자동 모니터링·복구
DevOps(협업) → DevSecOps(보안 통합) → NoOps(운영 추상화)
```
## 연관 토픽
- [[DevOps]] - 운영 협업 문화
- [[GitOps]] - Git 기반 운영 자동화
- [[서버리스 아키텍처]] - 인프라 추상화
- [[클라우드 네이티브]] - 운영 표준 패턴
