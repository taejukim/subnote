#정보관리기술사 #보안 #DRM #디지털저작권 #NEW
## 정의
DRM(Digital Right Management)
- 디지털 콘텐츠의 불법 사용·복제 방지와 과금 서비스를 통해 정상 사용자를 검증하는 저작권 보호 기술
## 키워드
* CP, CD, CC, CH, Packager, Secure Container, XrML, ODRL, Watermark, Fingerprint
## 암기법
* CPCDCCCH: 제공자·분배자·소비자·클리어링하우스
## 특징
- 패키징: 암호화 콘텐츠·메타데이터·사용정보를 Secure Container로 구성
- 라이선스 중심: 클리어링하우스가 권한정책·라이선스 발급
- 식별·표현: DOI/URI, XrML·ODRL·XMCL
- 불법유통 추적: Watermark·Fingerprint 연계
## 목적
- 디지털 콘텐츠 불법 사용·복제 방지
- 정상 사용자 검증 및 과금·권리 관리
## 구성요소
- DRM 서버: DRM 콘텐츠(암호화·메타·사용정보), Packager → Secure Container
- 클리어링하우스: Policy, License, 관리정보, Usage
- DRM 클라이언트: 단말기/셋톱, Secure Container 복호화
- 기술 - 식별: DOI, URI(MPEG-21)
- 기술 - 메타데이터: INDECS, MPEG-7
- 기술 - 권한표현: XrML, ODRL, XMCL
- 기술 - 적발: Watermark, Fingerprint
- 흐름: 등록 → 라이선스요청 → 요금지불 → 라이선스발급 → 콘텐츠다운로드
## 구성도
```
[제공: Packager] ──등록/라이선스등록──→ [분배: Store Front]
         │                                    ↕ 라이선스요청
         └──────────→ [클리어링하우스] ←──요금── [소비: DRM Controller]
                              │ 라이선스발급          ↑
                              └─────────────────────┘
                         Store Front → 콘텐츠 다운로드
```
## 연관 토픽
- [[디지털 워터마킹]] - 저작권 정보 삽입·추적
- [[핑거프린팅]] - 구매자 추적
- [[SW난독화]] - SW 무단복제 방지
- [[전자봉투]] - 암호·키 보호 유통
