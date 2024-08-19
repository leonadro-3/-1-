### 예제코드

```
Sub Macro1()
'
' Macro1 Macro
'
'
    Range("B1").Select
    ActiveCell.FormulaR1C1 = "Hello World"
    Range("B2").Select
End Sub
```

### Sub Macro1() ~ End Sub
Macro()는 보통 함수 표현이다. F12를 누르고 console 탭에서 alert("안녕")을 입력하면 alert() 함수가 안녕이라는 문구가 담긴 메세지 창을 크롬창에 표시하게 해준다.  
하지만 vba에서는 프로시저라고 하며 매크로와 같이 어떠한 동작을 순차적으로 실행만 한다. 즉, 함수처럼 문구를 반환하지 않는다는 것이다.  
문서에서는 record mecro의 기능을 이용하여 예시를 보여주고 있다.  

### 매크로 기록을 이용하여 vba 코드들을 이해할 수 있다.

#### 매크로 기록 위치
![1](https://github.com/user-attachments/assets/7b9ecba6-015f-4a65-aedf-bcbe5e060cdd)
#### 매크로 기록시 설정
![2](https://github.com/user-attachments/assets/6006efdc-9a4e-4ff5-946e-f430f6eb6eb7)
#### 아무 작업후 매크로 편집으로 VBA 코드 확인
![3](https://github.com/user-attachments/assets/95341636-6521-4e44-b34d-46905c6c020c)
![4](https://github.com/user-attachments/assets/fafe405a-218a-4fda-9188-f68b4a2de259)
#### 새로운 시트를 만들고 해당 작업을 반복
![5](https://github.com/user-attachments/assets/045e49b3-bf9c-453d-ac4f-0ac94944a80c)
![6](https://github.com/user-attachments/assets/381c1496-9a84-4c0d-9502-90141670c86f)

### 예제 코드

```
Sub 매크로1()
'
' 매크로1 매크로
' 테스트"&chr(13)&"
'

'
    Range("F5").Select
    ActiveCell.FormulaR1C1 = "안녕"
    Range("G5:G11").Select
    ActiveCell.FormulaR1C1 = "1"
    Range("G5:G11").Select
    Range("G6").Activate
    ActiveCell.FormulaR1C1 = "2"
    Range("G5:G11").Select
    Range("G7").Activate
    ActiveCell.FormulaR1C1 = "3"
    Range("G5:G11").Select
    Range("G8").Activate
    ActiveCell.FormulaR1C1 = "4"
    Range("G5:G11").Select
    Range("G9").Activate
    ActiveCell.FormulaR1C1 = "5"
    Range("G5:G11").Select
    Range("G10").Activate
    ActiveCell.FormulaR1C1 = "6"
    Range("G5:G11").Select
    Range("G11").Activate
    ActiveCell.FormulaR1C1 = "7"
    Range("G5:G11").Select


End Sub
```

### Range("F5").Selct
F5의 셀을 클릭하는 것과 동일하다.  
구체적으로 Range()에 ""로 특정 셀 위치값을 주면 해당 위치에 접근하는 것이고  
.Selct는 클릭을 의미한다.  

### ActiveCell.FormulaR1C1 = "안녕"
F5의 셀에 안녕을 입력하는 것과 같다.  
구체적으로 ActiveCell은 Range("F5").Selct가 된 이후에  
해당 셀의 데이터를 입력하기위해 Cell을 활성화하는 것이다.  
.FormularR1C1은 상대주소의 값이라는 걸 의미한다.  

### Range("G5:G11").Select
Range 메소드 혹은 함수에 셀의 범위 G5:G11까지의 col의 범위를 클릭한 것이다.  

### VBA 주석

```
'
' 매크로1 매크로
' 테스트"&chr(13)&"
'

'
```
'를 입력하고 한칸을 비운 다음 주석을 입력할 수 있다. 특히하게 바로 색깔 변화가 보이지 않고 커서를 이동해야 색깔이 변화한다.  

### VBA 모르는 속성 빨리 찾아보기

```
ActiveCell.FormulaR1C1 = "7"
```
여기서 의미를 유추하기 어렵거나 모르는 속성값이 나오면 해당 속성을 드래그 한 이후 F1를 누르면 자동으로 해당 속성에 관한 문서를 검색해준다.  
즉, vs code에서 제공하는 parameter hint 기능이 없기 때문에 매우 귀찮은 상황이 생긴다는 것이다.  
하지만 이를 어느정도 해결하는 방법이 있다.  

```
Range("G5:G11").Select
```
이러한 메소드를 사용할 때 "G5:G11"의 의미를 엑셀 수식을 만져본 사람이라면 누구나 알지만  
마찬가지로 드래그를 한 이후 Ctrl + Shift + i를 눌러주면 어느정도 힌트가 뜬다.  
물론 상세한 설명은 제공되지 않는다.  

![10](https://github.com/user-attachments/assets/c73aa198-affe-4b76-b1ad-bdbb542809c4)
![11](https://github.com/user-attachments/assets/4e0bb57c-63f1-4f11-96b7-78e43384a4ce)

> Cell 선택, 특정 셀 범위 지정, 셀에 데이터 입력, 주석 입력, 매크로 사용시 모르는 코드가 있을 때 이를 검색하는 방법에 대해 알아보았다.
> 맨 땅에 삽질을 해도 어떻게 삽질을 하느냐에 따라 숙련도가 달라진다.   

###
