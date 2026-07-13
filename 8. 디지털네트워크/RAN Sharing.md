#정보관리기술사 #디지털네트워크 #RANSharing #5G #NEW
## 정의
RAN Sharing(Radio Access Network Sharing)
- MOCN·MORAN·GWCN 방식으로 기지국·코어·게이트웨이 등을 공유하는 무선 인프라 공유 기술
- 동일 주파수 사용 시 간섭을 줄이고 CAPEX/OPEX를 절감
## 키워드
* MOCN, MORAN, GWCN
## 암기법
* 공유깊이: MORAN(RAN) < MOCN(+주파수) < GWCN(+코어일부)
## 특징
- MORAN: 기지국·제어기 공유, 주파수·코어는 사업자별 분리(차별화↑)
- MOCN: 주파수·기지국·제어기 공유, 코어만 분리(구현·비용 유리)
- GWCN: 주파수~MME/S-GW까지 공유, P-GW만 분리(비용 최대↓)
- 트레이드오프: 공유 범위↑ → 비용↓, 구현복잡도↑·차별화↓
## 목적
- 이통사 간 인프라 중복 투자·간섭 문제 해소
- 망 구축·운영 비용 절감
## 구성요소
- MOCN: Spectrum·eNB/gNB·Controller 공유 / Core 분리
- MORAN: eNB/gNB·Controller 공유 / Spectrum·Core 분리
- GWCN: Spectrum·RAN·MME·S-GW 공유 / P-GW·서비스플랫폼 분리
## 구성도
```
MORAN: CoreA/B ─ Shared RAN ─ SpecA | SpecB
MOCN : CoreA/B ─ Shared RAN ─ Shared Spectrum
GWCN : P-GW A/B ─ Shared(MME/S-GW+RAN+Spec)
```
## 연관 토픽
- [[C-RAN]] - 중앙집중 RAN
- [[O-RAN]] - 개방형 RAN
- [[Network Slicing]] - 논리망 분리·공유
- [[5G 특화망]] - 특화 무선망
