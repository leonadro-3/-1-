## VBA의 장단점들

### 에디터의 좋지 않은 기능과 긍정적인 면
엑셀에서 제공하는 Microsoft Visual Basic for Applications는 오래된 에디터이다.   
사용해보면 vs code나 pycharm과 같은 에디터가 왜 좋은지 이해할 수 있다.  
그러나 자격증이나 관습적으로 사용된 프로그램이기도 하다.  
무엇보다도 구글의 스프레드시트와 비교해서 자동으로 모든 파일이 업로드 되는 클라우드 환경에서 벗어날 수 있다는 장점이 있다.  

ctrl + j를 눌러서 숨을 쉴 수 있다.  

### 기존 언어와 매우 다른 형식
빠르게 사용하고 싶다면 파이썬으로 엑셀 vba을 대체하여 사용하는 것이 좋다.   
파이썬의 엑셀과 vba의 엑셀은 진입장벽의 차이가 체감될 정도로 크다. 


### vba의 파일 확장자명
vba를 저장하면 .xlsx파일로 저장이 되는데 사실 vba 코드만 적힌 파일은 .cls 파일로 저장된다.

![1](https://github.com/user-attachments/assets/d8378e79-c7e6-48e6-a41a-303ffe152b7e)
![2](https://github.com/user-attachments/assets/9d4708d9-e63c-4fb9-b491-c4a850dcf4d8)
![3](https://github.com/user-attachments/assets/f1454a5f-98be-4fbc-a8de-7053b0cbf98e)
![4](https://github.com/user-attachments/assets/5db98f92-3f07-49ae-8be1-808b5fa81015)

### Solver (SOLVER.XLAM)의 암호화
암호를 설정하지도 않았는데 SOLVER.XLAM에 암호가 걸려져 있다.  
![스크린샷 2024-08-17 161837](https://github.com/user-attachments/assets/94e9dd79-7ab9-43b9-a2c4-597993f3cadb)
https://stackoverflow.com/questions/42345254/excel-solver-password-what-is-it-and-where-can-it-be-acquired-bought
이는 solver를 개발한 유료회사의 소스이기 때문이다.    

## vba에 존재하는 파일 확장자명들

통합문서 .xlsx  
모듈파일 .bas  
클래스파일 .cls  
폼파일 .frm  
솔버파일 .xlam (접근 x)  

![11](https://github.com/user-attachments/assets/81c00c29-d9e1-4e11-b003-a491ccd4231d)
![22](https://github.com/user-attachments/assets/73e60ba3-1a12-4791-a376-21c221565bab)
![파일들](https://github.com/user-attachments/assets/6162049d-2016-46ec-ad65-0ac06acc4e6b)

하나씩 열어보자

Class1.cls  

```
VERSION 1.0 CLASS
BEGIN
  MultiUse = -1  'True
END
Attribute VB_Name = "Class1"
Attribute VB_GlobalNameSpace = False
Attribute VB_Creatable = False
Attribute VB_PredeclaredId = False
Attribute VB_Exposed = False
```

Module1.bas  

```
Attribute VB_Name = "Module1"
```

UserForm1.frm  

```
VERSION 5.00
Begin {C62A69F0-16DC-11CE-9E98-00AA00574A4F} UserForm1 
   Caption         =   "UserForm1"
   ClientHeight    =   3036
   ClientLeft      =   108
   ClientTop       =   456
   ClientWidth     =   4584
   OleObjectBlob   =   "UserForm1.frx":0000
   StartUpPosition =   1  '¼ÒÀ¯ÀÚ °¡¿îµ¥
End
Attribute VB_Name = "UserForm1"
Attribute VB_GlobalNameSpace = False
Attribute VB_Creatable = False
Attribute VB_PredeclaredId = True
Attribute VB_Exposed = False
```

해당 값들이 어떤 의미인지 현재로써는 모르지만 어떤 object나 class를 상속받아 해당하는 abttribute 값의 상수를 입력하면 excel이 해당 파일을 읽을 때 사용하는 것으로 보인다.  


## vba 단축키
vs code로 사용할 수 없기 때문에 단축키를 사용해야 한다.  
![스크린샷 2024-08-17 165951](https://github.com/user-attachments/assets/5616d35a-ae65-4bce-ad50-1de1cf4860e2)

vs code와 차이점으로 스니펫이 tap이 아니라 ctrl + space bar를 눌러야 한다. enter를 눌러도 되지만 커서의 위치가 바뀐다.   
Application를 vs code처럼 입력하고 싶다면 a + ctrl + j + Application + ctrl + space bar를 눌러야 한다.  

## vba 진짜 간략한 튜토리얼 (https://learn.microsoft.com/en-us/office/vba/library-reference/concepts/getting-started-with-vba-in-office#when-to-use-vba-and-why)




