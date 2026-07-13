#정보관리기술사 #보안 #CWPP #보안/클라우드보안
Cloud Workload Protection Platform & Cloud Security Posture Managerment

## CWPP 정의
- 물리적 컴퓨터, 가상머신 컨테이너 서버리스 워크로드 등에 대한 일괄적인 제거 및 가시성을 확보하고 클라우드 서버 워크로드를 보호하기 위한 솔루션
- 키워드 : 외부, 인프라, 구성, 규정 준수 위반

## CSPM 정의
- 클라우드 기반 시스템 및 인프라에서 위험과 잘못된 구성을 지속적으로 모니터링하는 프로세스
- 키워드 : 내부, 내부 실행 위협, 워크로드

## 가트너에서 제시한 클라우드 보안 서비스 커버리지
![[Pasted image 20260410002142.png|500]]

## CSPM vs CWPP 비교

|구분|CSPM|CWPP|
|---|---|---|
|**정의**|컴플라이언스 또는 기업 **보안 정책**에 따라 클라우드 인프라 **위험요소를 예방/탐지/대응** 등 클라우드 위험을 **지속적**으로 **관리하는 서비스**|개발부터 운영까지 **워크로드에서 보안을 구현**하여 지속적으로 안정적인 **클라우드 구성을 보장**하기 위한 클라우드 **보안 형상 관리 서비스**|
|**특징**|- 클라우드 보안설정 관리|- 워크로드 보호 플랫폼|
|**목적**|- 클라우드 서비스 구성상의 위험평가 및 관리|- 서버 워크로드 보호|
|**적용환경**|- **PaaS**, 일부 IaaS|- **IaaS**, 일부 PaaS|
|**핵심기능**|- 클라우드 환경에서의 컴플라이언스 지속적 확인  <br>- 하나 이상의 어카운트 혹은 멀티 클라우드를 통합하여 한눈에 볼 수 있도록 **자산 가시성 제공**|- 무결성 점검 및 위변조 감시  <br>- 어플리케이션 상태 감시  <br>- 계정 및 로그 감시  <br>- 방화벽 차단 로그 감시  <br>- **호스트 방화벽**|
|**구성요소**|- Compliance Assessment  <br>- Risk Identification  <br>- Operational Monitoring  <br>- DevSecOps Integration  <br>- Threat Protection  <br>- Policy Enforcement|- Exploit Protection  <br>- Application Whitelisting  <br>- System Integrity  <br>- Network Segmentation  <br>- System Monitoring  <br>- Workload Configuration|

> **핵심 구분**: CWPP는 워크로드 보호(애플리케이션, 컨테이너, VM 보안)인 반면, CSPM은 설정 및 규정 준수 관리(클라우드 환경 설정 오류, 정책 위반 탐지) 보안 솔루션