#운영체제 #inode #Unix #필수 #운영체제/파일시스템 #NEW
## 정의
유닉스의 inode
- UNIX 파일 시스템에서 파일 속성과 저장 위치를 관리하는 메타데이터 구조체
## 키워드
* Direct/Single/Double/Triple Indirect, owner ID, mode, TimeStamp, link count
## 암기법
* Direct→Single→Double→Triple: 대용량 파일
## 구성요소/특징/유형
| 구성 | 내용 |
| ---- | ---- |
| Attribute | mode, owner, group, permission, size, timestamp, link |
| Index | Direct(4KB), Single(1024×4KB), Double, Triple |
| 할당 | Super block remembered i-node, free list |
| 반납 | free count↑, remembered i-node 갱신 |
## 연관 토픽
- [[파일 시스템]] - Unix FS 구조
- [[Paging 기법]] - 블록·인덱스
- [[직접 사상과 연관 사상 페이징 기법]] - 주소 변환
