#정보관리기술사 #SW공학 #IOD #UML #NEW
## 정의
Interaction overview diagram
- 액티비티 다이어그램의 순서 흐름에서 액티비티 대신 시퀀스로 상세 상호작용을 표현하는 행위 다이어그램
- Activity와 Sequence의 결합
## 키워드
* Activity, Sequence, sd frame, Decision, Interaction
## 암기법
* Act+Seq: 흐름은 Activity, 상세는 Sequence(sd/ref)
## 특징
- Activity 요소: ActionState, Initial/Final, Decision, Transition
- Sequence 요소: 활성 객체, 메시지, 제어 사각형(Activation)
- sd/ref 프레임으로 상호작용 단위 참조
- 분기(Decision)로 시나리오 경로 표현
## 목적
- 전체 제어 흐름과 객체 상호작용을 한 다이어그램에서 조망
- 복잡한 시나리오의 흐름·상세 메시지 동시 표현
## 구성요소
- Activity State: 워크플로 작업 단계
- Initial/Final: 시작·종료
- Decision: 조건 분기
- Transition: 제어 흐름
- Active Object/Message/Activation: 시퀀스 상호작용
## 구성도
```
(●) → [sd Enter Code: User→ACS enter/check]
         ↓
       <> code OK?
      /          \
 [ref Release]   (◉)  [code not OK]
```
## 연관 토픽
- [[활동 다이어그램]] - 제어 흐름
- [[Sequence diagram]] - 메시지 상호작용
- [[UML-Diagram 전체]] - UML 체계
