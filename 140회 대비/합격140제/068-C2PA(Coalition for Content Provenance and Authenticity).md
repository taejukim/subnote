#정보관리기술사 #보안 #C2PA #콘텐츠출처인증
## 정의
C2PA(Coalition for Content Provenance and Authenticity)
- 디지털 콘텐츠의 생성·편집·유통 이력을 암호화 서명된 메타데이터로 기록해 출처·편집이력·무결성을 검증하는 국제 개방형 표준
- 딥페이크·AI 생성 콘텐츠 확산에 대응하는 콘텐츠 진위 검증 표준
## 키워드
* Manifest, Assertion, 디지털서명, PKI, JUMBF, 해시 링크, Claim
## 암기법
* 매어디제바: Manifest·Assertion·디지털서명·PKI·바인딩(JUMBF) - C2PA 5대 기술요소
## 특징
- 위변조방지성: 개인키 서명으로 Manifest 변조를 원천 차단
- 이력추적성: Assertion 체인으로 생성부터 편집까지 전 과정 기록
- 표준기반성: JUMBF(ISO/IEC 19566-5) 국제표준 포맷으로 파일 내부 저장
- 신뢰체계성: PKI 기반 CA 인증으로 검증 공개키의 신뢰성 보장
## 목적
- 위·변조 불가능한 서명으로 콘텐츠 무결성 및 진위 검증 지원
- 저작권 보호와 유포경로 추적을 통한 오정보 확산 차단
## 구성요소
- Manifest: 메타데이터·편집이력·생성도구 정보를 담는 핵심 데이터 블록
- Assertion: 생성일자·카메라모델·AI모델명 등 개별 사실 정보
- Claim: 모든 Assertion을 해시링크로 묶은 암호화 참조 구조
- Claim Signature: X.509 인증서 기반 개인키로 서명한 결과물
- JUMBF: Manifest·Assertion을 이미지/영상 파일에 저장하는 ISO 국제표준 포맷
- 해시 링크: SHA-256 기반으로 콘텐츠-Manifest 연결, 변경 여부 추적
## 구성도
```
[Digital Content] --해시링크(SHA-256)--> [Assertion들: 생성일자/AI모델 등]
                                                │
                                          [Claim: Assertion 묶음]
                                                │ 개인키 서명(PKI/X.509)
                                          [Claim Signature]
                                                │
                                    [Manifest: JUMBF로 파일 내 저장]
```
## 연관 토픽
- [[딥페이크]] - C2PA 검증 대상이 되는 위협 콘텐츠
- [[디지털워터마킹]] - 콘텐츠 출처 표시 보완 기술
- [[PKI]] - 공개키 기반 신뢰 체계
- [[생성형 AI]] - 콘텐츠 진위 검증 필요성 촉발 기술
