#정보관리기술사 #디지털서비스 #AI데이터센터 #AIDC
## 정의
AI 데이터 센터(AI Data Center)
- 대규모 AI 모델 학습·추론을 위해 고성능 AI 전용 HW, 초저지연 NW, 첨단 냉각·전력 시스템을 통합한 고밀도 컴퓨팅 인프라
- AI 워크로드에 최적화된 차세대 데이터 센터 형태
## 키워드
* GPU/TPU, HBM, 액체 냉각, 고밀도 전력, K-클라우드, SMR
## 암기법
* 에AI지AI: Energy·AI HW·지원Infra·AI Cloud
## 특징
- 고성능: GPU/TPU 등 AI 가속기 중심 구성
- 고밀도: 단위 면적당 고전력·고연산
- 첨단 냉각: 액체·몰입식 냉각 도입
- 초저지연 NW: 고대역폭 인터커넥트 필수
## 목적
- 대규모 AI 학습·추론 워크로드 최적 지원
- 국가 AI 인프라 자립과 경쟁력 확보
## 구성요소
- 4대 영역: Energy Production, AI Computing HW, Support Infrastructure, AI Cloud Services
- 컴퓨팅 인프라: AI 가속기, 이기종 컴퓨팅, 병렬 처리, 고속 인터커넥트, 고대역폭 NW, 저지연 통신, HBM, 계층형 메모리, 병렬 스토리지
- 지원 인프라: 고전력 밀도 대응, 액체·몰입식 냉각, 전력 스케줄링, AI 프레임워크, 쿠버네티스, 컴파일 기술
- 데이터/운영: 데이터 파이프라인, 고속 데이터 로딩, 데이터 거버넌스, 고가용성, 운영 자동화, Zero Trust
- 일반 DC와 차이: AI 학습·추론 vs 일반 IT, GPU/TPU vs CPU, 고밀도 vs 저밀도, 액체 vs 공기 냉각, 초저지연 vs 표준 NW
- 이슈: 고전력, 공급 병목, 탄소 배출, 수자원, 사이버 보안, 데이터 주권
- 개선: 특별 구역, 삼각 협력, 에너지 혁신, 차세대 냉각, 인센티브, 법적 틀
- 국가 전략: 미국(SMR), 중국(동수서산), EU(그린 디지털), 한국(K-클라우드)
## 구성도
```
[Energy] SMR·재생에너지 → [Cooling] 액체/몰입식
                                 ↓
[AI Computing] GPU/TPU 클러스터 + HBM → 초고속 인터커넥트(NVLink/NVSwitch)
                                 ↓
[Support Infra] K8s·MLOps → [AI Cloud] 학습·추론 서비스
```
## 연관 토픽
- [[TPU]] - 텐서 처리 장치
- [[GPGPU - CUDA]] - GPU 컴퓨팅
- [[HBM]] - 고대역폭 메모리
- [[소버린 클라우드(Sovereign Cloud)]] - 데이터 주권
