# 컴퓨터 활용 1급을 따야 하는 이유~

1. 공기업 가산점
2. 학점
3. 2급보단 1급이 재밌음
4. 상시로 볼 수 있음 (필기, 실기)
5. 깊게 들어가기 위한 주제로 나눠서 멍떄리며 읽기 좋음.
  
# 시험 과목

컴퓨터 일반, 스프레드시트 일반, 데이터 베이스 일반으로 되어 있음. "일반"이라고 되어 있어서   
컴공 전공한 사람들의 엄격한 잣대를 들이 밀면 안됨.   
컴퓨터 학원에서 컴활 1급 강사 모집하기도 함.   

# 컴퓨터 일반 
## 운영체제 사용

### 운영체제(OS:Operation System)가 뭘까?

MS(Microsoft) : 회사  
Windows : 운영체제의 일종  
Windows 11 : 가장 최신 OS  
Linux : 무료 운영체제, 명령어가 영어라 쓰기 어려움. (개발자 전용 운영체제)  

### 운영체제의 목적이 뭘까?

처리능력(Throughput) : 쓰루/풋 (in : 들어오다, out : 나가다, input : 입력, output : 출력, *put : ~량 옛날 미국 MZ식 표현)  
응답시간(Turnaround Time) : Turn(턴), return : 되돌아오다, turn : / (퍼) 단위계, time : 시간  
신뢰도(Reliability) : rely(의존하다), ability(능력), 신뢰할 수 있는 능력  
사용가능도(Availability) available(이용할 수 있는), ability(능력), 사용할 수 있는 능력  

=> data type, data unit등의 정의가 아님. 왜냐하면 컴퓨터의 처리 능력에는 수많은 변수들이 존재하기 때문임.  
=> 다나와에 CPU 성능 검색 했을 때 코어와 쓰레드가 나오는데 보통 스펙이라고 함.  
=> 클럭을 hz(주파수) 단위로 표현이 가능함. 근데 더 자세하게 알고 싶으면 '컴퓨터 구조 및 설계'라는 책을 보면 됨.  
=> 맥락에 따라서 다른 용어를 사용하기도 함.  
=> 윈도우 운영체제의 성능을 보고 싶다면 작업관리자 리소스 모니터를 키면 됨  
=> 리눅스가 더 좋다고 하는 이유는 커맨드 라인으로 카톡이나 유튜브를 실행시켜 보기가 일반적으로 어렵기 때문임.  

### 운영체제의 발달과정

일괄처리시스템(Single-stream Batch Processing Systems)  
실시간처리시스템(real-time system)  
다중프로그래밍시스템(Multi-programming system)  
시분할처리시스템(Time sharing system)  
다중처리시스템(multiprocessing system)  
분산처리시스템(Distributed processing system)  

내가 읽고 있는 교재에는 별다른 설명 없이 이렇게 발전했다고 하는데 솔직히 이걸 비교해서 차이점을 이해하는 지식을 요구하지 않는다.  

ex)   

컴퓨터 책상 위 쓰레기를 쌓아 두고 나중에 한번에 버리는 사람 = 일괄 처리 시스템  
집 청소 안했는데 갑자기 여친이 저녁에 집에 온다고 할 때 빨리 집가서 청소 하는 사람 = 실시간 시스템  
자기 쓰레기만 비우는게 아닌 다른 사람 쓰레기도 함께 청소해주는 훌륭한 사람 = 다중 프로그래밍 시스템  
쓰레기 청소 뿐만 아니라 여러 사람들이 같이 다양한 청소를 분담하여 항상 청결 상태를 유지하는 집단 = 시분할 시스템  
노션을 쓰면서 개발을 하는 사람들 = 분산 처리 시스템  

### 운영체제의 구성  

제어프로그램(Control Program)  
처리프로그램(Process Program)  

제어프로그램은 순서도(flow chart)을 생각하면 되고 처리프로그램은 의사코드(pesudocode)라고 생각하면 된다.  

### 한글 윈도우의 특징 및 새로운 기능

그래픽 사용자 인터페이스(GUI) : 리눅스(CLI)와 가장 큰 차이점. 근데 사실 리눅스도 GUI가 있다.   

선점형 멀티태스킹(Preemptive Muti-tasking) : 언제 어디서나 문제가 생기면 ctrl + shift + esc를 눌러서 재부팅이 가능하다.  

[1] 사실 최근에 앤비디아 그래픽 카드 업데이트를 장기간 안했다가 이런 명령어가 실행되지 않는 상황에 놓인 적이 있다.   
보통은 자동으로 업데이트로 설정하는데 나는 아무런 업데이트를 하지 않는 아주 훌륭한 유저이다.  
그 버그가 왜 생겼는지 문제가 지속적으로 발생하는 컴퓨터를 가지고 있다는 것은 아주 재밌는 실험환경을 가지고 있다는 것이다.  

[2] 만약 당신이 방송을 하려고 OBS을 켰다. 라이브 도중 윈도우 키를 누르면 최근 항목이 뜨는데 게임을 하다가 실수로 윈도우키를 누를 수 있다.  



플러그 앤 플레이(Plug & Play) : 보통 마우스 선을 USB에 꼿아서 쓰는데 이게 가능한 이유가 이러한 기능을 지원해줘서이다.  
USB도 꼿으면 자동으로 실행되는데 이러한 점 때문에 군대 컴퓨터에 USB 꼿으면 좆되는 것이다. 물론 지금은 휴대폰 써서 그럴 일이 거의 없겠지만...  
요즘에는 모두 클라우드 환경이기 때문에 이러한 구시대적 발상은 통하지 않는다. ^^  

NTFS 지원 : 약자가 New Technology File system임... 엔지니어들의 작명 센스 ㄷㄷㄷ  
bitlocker, pcr7 binding이 이러한 보안 기능에 해당한다.  
컴퓨터관리(ctrl + r + compmgmt.msc) + 디스크 관리 + 파일 시스템에 보면 NTFS을 확인할 수 있다.  
compmgmt.msc : (comp)uter(m)a(g)e(m)en(t).(m)icro(s)oft(c)osole의 약자인 것 같다.

운영체제가 설치된 곳이 컴퓨터 하드 디스크이지만 폴더(파티션)를 나누어서 C 드라이브에는 ntfs로 (부팅, 페이지 파일, 크래시 덤프, 기본 데이터 파티션)을 구성하고 있고  
(디스크 0 파티션 1)인 곳에는 efi 시스템 파티션, (디스크 0 파티션 4)인 곳에서는 복구 파티션으로 사용하고 있다.  

부팅(booting)은 컴퓨터 전원을 키고나서 로딩 화면시 뒤에서 작동되는 프로그램 이라고 생각하면 된다.  
페이지 파일(page file)은 다양한 목적으로 사용되는데 주로 메모리 관리와 관련되어 있다.  
크래시 덤프(crash dump)는 비정상적인 종료시 당시 상황을 수집하는 데이터이다.  
그래서 가끔 컴퓨터하다가 엄마가 전원 차단기 내리고 다시 키면 안전모드로 진입하는 경우가 있는데 이럴 때 쓰는 용도라고 생각 하면 된다.  
하지만 노트북은 배터리이기 때문에 선을 뽑아도 상관 없다. 즉, 컴퓨터를 살 때 노트북으로 사는게 훨씬 안정성이 높다는 것이다.  

