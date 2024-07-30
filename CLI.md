### 파워쉘








### cmd 활용 (batch script) https://www.youtube.com/watch?v=Qn0aq6XjjA8

### cmd echo on/off, set, %var% 의미미

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

```
@echo off
set filename=test.txt
echo The file name is %filename%.
```

> @echo off로 계속 하여 실행 결과를 출력하게 하고 filename을 변수로 set한 이후 echo로 해당 변수를 가져다가 사용함.  

```
const filename = 'test.txt';
console.log(`this filename is ${filename}`);
```

> 자바스크립트에서 템플릿 리터럴 사용법과 흡사하다. 차이점은 변수를 어떻게 선언하여 가져오느냐이다.  
> 그외에도 파이썬, C++에서도 string의 템플릿 리터럴이 사용된다.  


### cmd 변수들을 작성하여 특정 파일의 경로나 명령여들을 변수화 한다.  

![2](https://github.com/user-attachments/assets/bb276500-b2ab-482b-a0a6-aed9af76cd5a)

엄청난 노가다.. 변수명을 어떻게 관리하느냐가 더 큰 문제가 된다.  
만약 cmd 모든 명령어들과 해당 명령어에 사용될 주요 파일 경로들이 미리 정해져있다면 해당 경로를 입력하여 .bat 파일로 관리할 수 있을 것이다.  
그러나 만약 경로가 섞인다면 이러한 변수 사용은 의미가 없어진다. 절대 경로를 랜덤으로 수정하여 랜덤으로 돌려버린다면 컴퓨터는 어떻게 될까?  
이건 마치 레지스트리 값들의 위치와 값들을 랜덤한 경로와 값들로 바꾸어 우주만한 거대한 루빅스 큐브를 섞어 놓은 것과 같지 않을까?  

만약 그러한 상황에 놓인 컴퓨터라면 당연히 정상적인 작동은 되지 않겠지만 최소한의 기능만 남겨두고 섞어 버린다면 다시 맞추는 데 걸리는 예상 시간은 몇 시간일까?  
근데 심지어 몇몇 값들이 훼손되어 있다면 과연 얼마나 많은 데이터를 다시 복구할 수 있을까?  


### git bash
### node (cli-api)
https://nodejs.org/api/cli.html
### web console (DOM)
### unreal engine console (C++)
### blender console (python)
