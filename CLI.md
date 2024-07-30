### 파워쉘








### cmd 활용 (batch script) https://www.youtube.com/watch?v=Qn0aq6XjjA8

[참고] https://nilssoderman.com/downloads/  
[batch runner] : vs code에서도 .bat을 실행할 수 있게 해준다. (https://marketplace.visualstudio.com/items?itemName=NilsSoderman.batch-runner)  

```
powershell : New-Item example.bat
```

> example.bat 파일이 만들어진다.

```
echo hello batch
```

> ctrl + j을 눌러 콘솔창을 열고 example.bat tap에서 f5를 누르면 실행이 된다.

```
echo on
echo 1
echo 2
echo 3
echo off
echo 4
echo 5
```

> on을 했을 때는 한줄에 하나씩 실행되어 결과가 표시되고 off을 했을 때는 한번에 남은 줄들을 실행한 결과를 모두 표시한다.

![1](https://github.com/user-attachments/assets/50ce01f6-a03b-49cd-8a89-9ee4501d0d4e)

ctrl + shift + ` : new terminal  
ctrl + shift + e : file explorer tap  
ctrl + tap : tap move  

```
@echo 1
```
> 명령줄 없이 결과만 표시되어 지저분 하지 않음. 모든 명령어에 @을 사용함.  

```
@echo "drive info and windows version"
@vol
@ver
```

> 미리 만들어 놓고 해당 명령어에 대한 설명을 추가하는 식으로 .bat 파일을 만들 수도 있다.  


```
ps: new-item example.bat
@echo "no info"
ps: new-item example_1.bat
set var=example
%var%
@echo %var%
```

> 두 개의 .bat을 만들고 example.bat을 변수로 집어넣어 example_1.bat을 실행할 때 사용할 수 있다.

set (변수명)=(변수 데이터)  
%변수명% : 해당 변수 데이터
:: : 주석처리  
rem : 주석처리  

```
set var=time(time cmd 명령어)
rem @echo %time%
```

> 결과를 보면 %time%은 time의 실행 결과인 현재 시간을 지칭하는 것을 알 수 있다.





### git bash
### node (cli-api)
https://nodejs.org/api/cli.html
### web console (DOM)
### unreal engine console (C++)
### blender console (python)
