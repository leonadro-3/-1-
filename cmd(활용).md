### cmd 활용 (batch script) https://www.youtube.com/watch?v=Qn0aq6XjjA8

### cmd echo on/off, set, %var% 의미

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
근데 심지어 몇몇 값들이 훼손되어 있다면 과연 얼마나 많은 데이터를 다시 복구할 수 있을까? 라는 복구 알고리즘 모델 추천해달라고 코파일럿에 검색하면?  

+ 기본적으로 set으로 잡혀져 있는 변수들이 있다.  

```
흥미로운 상상력을 가지셨군요! 컴퓨터 시스템이 랜덤으로 경로를 수정되어 뒤섞인 상태에서 어떻게 작동할지 상상해 보는 것은 흥미로운 주제입니다. 그럼 복구 알고리즘에 대해 알아보겠습니다.

복구 알고리즘은 데이터 손실이 발생했을 때 데이터를 복구하는 데 사용되는 방법과 절차를 정의합니다. 여러 가지 데이터베이스 복구 모델이 있으며, 각각의 특성과 적용 범위가 다릅니다. 여기서 몇 가지 주요한 복구 모델을 살펴보겠습니다1:

단순 복구 모델 (Simple Recovery Model):
트랜잭션 로그를 자동으로 관리하여 로그 공간을 최소화합니다.
로그 백업이 없으며, 특정 시점 복원이 지원되지 않습니다.
데이터 손실이 발생하면 최근 백업 이후의 변경 내용을 재실행해야 합니다.
전체 복구 모델 (Full Recovery Model):
트랜잭션 로그를 상세하게 기록하며, 로그 백업이 필요합니다.
특정 시점 복원이 가능하며, 임의의 시점으로 복구할 수 있습니다.
데이터 손실이 발생해도 로그 백업을 통해 변경 내용을 복구할 수 있습니다.
대량 로그 복구 모델 (Bulk-Logged Recovery Model):
대량 작업에 최적화된 모델로, 로그 공간을 최소화합니다.
특정 시점 복원은 지원되지만, 로그 백업이 필요합니다.
대량 작업 시 최소 로깅을 사용하여 성능을 향상시킵니다.

복구 알고리즘은 데이터베이스 관리자가 데이터 손실 시 어떤 방식으로 복구를 수행할지 결정하는 중요한 요소입니다. 데이터베이스의 특성과 요구 사항에 따라 적절한 복구 모델을 선택해야 합니다.
만약 데이터 손실이 발생했다면, 데이터베이스 복구를 위해 백업 집합을 복원하는 순서를 정확하게 따라야 합니다. 이를 통해 데이터를 안전하게 복구할 수 있습니다2.
또한, 데이터 손상이 발생했을 때 특정 알고리즘을 사용하여 데이터를 복구하는 경우도 있습니다. 예를 들어 RAID (Redundant Array of Independent Disks)에서는 여러 디스크를 조합하여 데이터를 보호하고 복구하는 방법을 사용합니다.
복구 알고리즘은 데이터 손실 시 어떤 방식으로 복구를 수행할지 결정하는 중요한 요소입니다. 데이터베이스의 특성과 요구 사항에 따라 적절한 복구 모델을 선택해야 합니다. 데이터 손상이 발생했다면, 데이터베이스 복구를 위해 백업 집합을 복원하는 순서를 정확하게 따라야 합니다. 이를 통해 데이터를 안전하게 복구할 수 있습니다2. 또한, 데이터 손상이 발생했을 때 특정 알고리즘을 사용하여 데이터를 복구하는 경우도 있습니다.
```

라고 한다. 물리적으로 기판이 부서진 경우엔 어차피 그걸 만든 설계도가 있다면 재구성이 가능할 것이다. 아무런 연결이 안된 장소를 구현하는 것이 가능할까?  
이론적으로 생각해보면 사람들이 가지고 있는 일반적인 지식보다 월등히 높거나 존재하지 않았던 지식들을 나혼자 발전시켜 알고 있다면 미래가 어떤 모습인지 혼자만 알 수 있다.  
한 가지 더 좋은 방법이 있다. 남들이 이해하지 못하는 방식으로 기록을 하면 된다. 근데 그것도 사람인 이상 언젠가 알게 되지 않을까?  
마지막 방법이 있다. 사람이 아니면 된다.  (정신병자들이 정신병자인 이유~)


### cmd에서 변수 자료형 선언

```
@echo off
set sum=10+10
echo The sum is %sum%
```

> 결과값은 The sum is 10+10이 된다. 이를 해결하기 위해 set /?을 하여 변수 선언시 사용법을 확인해보면 /a를 추가하면 숫자로 계산된다.

```
@echo off
set /a sum=10+10
echo The sum is %sum%
```

> 결과값으로 The sum is 20가 출력된다.

```
@echo off
set /a sum=10+10
set /p pause=pause
echo The sum is %sum%, %pause%
```

> 처음 pause가 나오고 값을 입력하여 엔터를 누르면 The sum is 20, 입력한 값으로 추가가 된다.

```
@echo off
set /a sum=10+10
set /a minus=10-10
set /a mulit=10*10
set /a divide=10/10

echo 10+10=%sum%
echo 10-10=%minus%
echo 10*10=%mulit%
echo 10/10=%divide%
echo 그룹짓기
```

> 만약 한글이 깨진다면 chcp 65001로 utf-8 인코딩으로 바꾸어줘야 한다.

비트를 움직이는 연산자들도 있으나 이후에 컴활 책에 다시 나올 때 다시 해보도록 하자 
