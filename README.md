# 컴퓨터 활용 1급을 따야 하는 이유~

1. 공기업 가산점
2. 학점
3. 2급보단 1급이 재밌음
4. 상시로 볼 수 있음 (필기, 실기)
5. 깊게 들어가기 위한 주제로 나눠서 멍 때리며 읽기 좋음.
  
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
컴퓨터관리(win + r + compmgmt.msc) + 디스크 관리 + 파일 시스템에 보면 NTFS을 확인할 수 있다.  
compmgmt.msc : (comp)uter(m)a(g)e(m)en(t).(m)icro(s)oft(c)osole의 약자인 것 같다.

운영체제가 설치된 곳이 컴퓨터 하드 디스크이지만 폴더(파티션)를 나누어서 C 드라이브에는 ntfs로 (부팅, 페이지 파일, 크래시 덤프, 기본 데이터 파티션)을 구성하고 있고  
(디스크 0 파티션 1)인 곳에는 efi 시스템 파티션, (디스크 0 파티션 4)인 곳에서는 복구 파티션으로 사용하고 있다.  

부팅(booting)은 컴퓨터 전원을 키고나서 로딩 화면시 뒤에서 작동되는 프로그램 이라고 생각하면 된다.  
페이지 파일(page file)은 다양한 목적으로 사용되는데 주로 메모리 관리와 관련되어 있다.  
크래시 덤프(crash dump)는 비정상적인 종료시 당시 상황을 수집하는 데이터이다.  
그래서 가끔 컴퓨터하다가 엄마가 전원 차단기 내리고 다시 키면 안전모드로 진입하는 경우가 있는데 이럴 때 쓰는 용도라고 생각 하면 된다.  
하지만 노트북은 배터리이기 때문에 선을 뽑아도 상관 없다. 즉, 컴퓨터를 살 때 노트북으로 사는게 훨씬 안정성이 높다는 것이다.  

windows11의 라이브러리(library) 기능과 개발에서의 library는 의미가 다름. 이건 마치 어둠속에서 아무것도 안보이는데 불꺼진 도서관속을 헤집고 다니는 행위를 뜻함.  

장치 스테이지(device stage) : 무대에 올린다. 하드웨어는 현실에서 꼿으면 됨. 근데 소프트웨어는 머리속으로 꼿아야 됨. staging area(임시 저장공간)  

### 한글 windows의 시작과 종료

### 안전모드로 부팅

안전모드는 네트워크에 연결되지 않아 바이러스나 악성코드 등에 감염될 우려가 없다. 최악의 상황에서 안전모드를 기반으로 다른 사람에게 공유되지 않는 업무를 처리할 수 있음.  
보수적인 일본 사회에서 그나마 대안이 될 수 있는 선택지 중 하나 : 안전모드로 os를 킨다음 업무를 보고 USB에 담아서 제출, 그리고 일주일마다 USB 모아서 성과, 진행 상황 보고 하게 한다면  
확실하게 일을 얼마나 했는지 측정할 수 있음. 즉, 세상의 모든 사람들을 쿠팡 노동자처럼 관리할 수 있게 됨.  

### 멀티 부팅

여러개의 운영체제를 사용한다고 되어 있지만 실제로 해보면 한 모니터에 여러가지 OS를 실행시키는 것은 아니다.  
LDplayer의 경우 휴대폰의 구글 마켓이나 앱스토어를 연결하여 데스크탑으로 실행시킬 수 있다. 즉, 한 컴퓨터와 수십개의 구글 계정과 LDplayer를 연결하여 모바일 게임 환경을 구축할 수 있다.  
또한 vmware도 마찬가지로 성능이 좋은 컴퓨터를 여러대의 가상 컴퓨터로 나누는 프로그램이다. 기존 컴퓨터에서 제공하는 메모리와 CPU, 하드 디스크를 이용하여 실질적으로 컴퓨터 안에 컴퓨터를 사용할 수 있다.  
즉, 인터넷에서 어떤 데이터를 얻기 위해 반복적으로 해야 한다면 이러한 방법을 통해서 더 효율적으로 습득을 할 수 있다는 것이다.  
게임내 재화를 판매하거나 교환할 수 있는 시스템이 있는 곳이나 방문자 수, 광고 수와 같은 데이터들은 항상 가상 컴퓨터와 클라우드 서버를 이용하여 조작을 할 수 있다는 점을 명심해야 한다.  

지금 당신이 보고 있는 데이터가 조작된 데이터인지 아닌지 명확히 구별하는 방법을 아는 것이 정보화 사회에서 가장 중요한 능력이다.  
그리고 그러한 방법들을 이용해 악용하는 산업의 집단이나 구성원들을 어떻게 처리할 것인지 고민해야 하는 것이 정보화 사회의 리더들이 해야 하는 것이다.  

### 한글 windows의 종료

시스템 종료는 어떤 상황일 때 시스템 종료일까?  
전기가 공급되지 않는 상황에서만 전기적 신호가 발생하지 않으므로 이러한 상황에 놓여 있는 것이 시스템 종료이다.  
휴대폰과 노트북은 배터리 시스템이기 때문에 소프트웨어적으로 시스템 종료를 한다고 하더라도 실질적으로 종료가 안되어 있을 가능성이 있다.  
이것은 음모론이 아니라 재시작 기능이 있다는 것을 보면 알 수 있는 점이다. 즉, 초초초초절전 모드라고 생각한다.   

과거의 휴대폰은 탈부착이 가능했지만 현대의 휴대폰은 "방수"를 이유로 탈부착이 어려운 구조이다.  
또한 무선 통신망의 발전으로 인해 언제 어디서든 방대한 데이터를 송수신 할 수 있는데 생각을 해보면  
휴대폰에 있는 "통화 기능"이나 "카메라"와 같은 것들, 그리고 "다양한 센서들"을 반대로 생각하면 유출시키는 도구가 된다.  

따라서 현대 정보통신기기들의 매우 확실한 종료 방법은 기판을 뜯고 해당 센서들이 달려있는 PCB 판의 소자들을 제거하여 완전 분해 시키는 것이다.  
매우 강력한 보안을 요구하는 곳이라면 이러한 방법을 통해서 보안을 확보 할 수 있을 것이다.  
하지만 매우 귀찮은 방법으로 차선책으로 비행기 모드를 켜두는 거나 안가져 가면 된다.  

### 한글 windows의 종료 예약 및 취소

윈도우 + r키로 실행창을 만든다음 shutdown /s /t 1800을 입력하면 1800초 이후에 시스템 종료 버튼을 누른 것처럼 종료가 된다.  
근데 만약에 이 시간을 1로 바꾸었다면 1초마다 켜지고 1초마다 꺼지게 된다. 재밌는 것은 원격모드에서도 이러한 명령을 할 수 있다는 것이다. (https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-xp/bb491003(v=technet.10)?redirectedfrom=MSDN)  
이론적으로 모든 OS의 재시작 명령어를 알고 원격으로 해당 명령어를 실행시킨다면 매우 효율적으로 전세계의 컴퓨터가 꺼졋다 켜졌다를 반복하게 만들 수 있다. (컴퓨터 전문가와 비전문가를 구별하는 방법~)  
쓸모 없다고 생각되는 사람이 있는 경우 합법적으로 내보내기 위해서 준비된 컴퓨팅 환경을 만들 수 있다.  

### 마우스 및 키보드 사용법(Pointing device gesture)

클릭(click) 한번 누르는 것  
더블클릭(double click) 두번 누르는 것  
드래그(drag) 한번 누르고 움직이는 것  
드래그 앤 드롭(drag and drop) 한번 누르고 움직인 다음 때는 것  

스마트폰에서는 touch gesture라고 한다.  
터치(touch, tap) 한번 손가락을 화면에 접촉 시키고 때는 것 마우스에서는 탭, 스마트폰에서는 터치라고 한다.  

마우스, 스마트폰 터치, GPS, GPU, 지도 간의 공통점은 좌표계를 사용한다는 것이다. (x,y로 이루어져있는 사분면을 사용한다.)  
다양한 computer screen을 만들 때 사용되는 수학적 원리들이 있다. (https://www.sciencedirect.com/topics/mathematics/computer-screen)  
하지만 어디에 사용되느냐에 따라서 만드는 방식이 달라진다. 웹에서는 event를 가져와 웹 화면에 유저들의 마우스 움직임을 가져올 수 있고  
어떤 사람들은 nannou를 사용하여 만든다. (https://guide.nannou.cc/why_nannou)  

일반적으로 대량의 데이터를 모두 일괄적으로 표현하는 것보다 일정 단위나 패턴으로 나누어 이해하기 쉽게 만드는 것이 더 어렵다.  
마우스의 이벤트들이나 키보드의 입력값들이 의미가 있으려면 어떤 서비스에 해당 값들을 보내는지 알아야 한다.  
예를들어 내가 15432라는 값을 키보드로 입력했을 때 로그인 페이지(주소)에서 입력한다면 높은 확률로 아이디나 비밀번호일 확률이 높다는 것을 알 수 있다.  
왜냐하면 로그인 페이지에서 값을 입력하는 대부분 경우는 아이디가 아니면 비밀번호이기 때문이다.  

사람이 로그인 페이지에 접속하고 무언가를 입력하여 인증되는 과정을 컴퓨터의 프로세스로 확인하고 이 과정속에서 문제점이나 악용점들을 발견하는 것이  
IT인들의 역량이기도 하다. 재밌는 사실 중 하나는 현대 사회에서는 클릭 몇번으로 굉장히 많은 돈을 송수신할 수 있는데 표현하는 것도 bit라는 것이다.  
bit는 여러가지가 되지만 사용자들에게 돈으로 인식되는 bit는 어떤 bit인지 알고 만들 수 있다면 발행자가 될 수 있다. (비트 코인이 bitcoin인 이유~)  

현실에서 노동을 하여 돈을 받을 때 현금으로 주는 사람은 거의 없다. 현금 기반의 금융체계와 데이터 기반의 금융체계, 중 어떤 것이 누구에게 더 이익이 되는지 따져볼 필요가 있다.  
마찬가지로 가상화폐 기반의 금융체계가 과연 나에게 이익이 되는지 따져볼 필요가 있다. 어떤 선택지든 비용이 증가하거나 신뢰성이 떨어지거나 생산성이 떨어진다면 선택되지 않을 것이다.  
가상화폐로 돈을 버는 사람들 vs 현대 금융체계로 돈을 버는 사람들간에 싸움은 둘 중 하나가 무너질 때까지 계속될 예정이다.  

### 키보드 주요 key 기능 (매우 중요)

키보드의 키 중에서 가장 좋은 유용한 키는 뭘까?  
이를 알기 위해서 모든 단축키의 목록과 자주 사용하는 단축키의 데이터를 가지면 된다. 즉, 많이 컴퓨터를 써보면서 의미있는 단축키를 확인하는 것이다. 한편 기존의 단축키를 제외하고 더 유용한 단축키를 만들 수도 있을 것이다.  
새로운 단축키를 만드는 기능은 소개되고 있지 않지만 코드로 개발을 하면 특정 상황에서 매우 유용한 단축키들을 만들어 매크로 처럼 사용할 수 있을 것이다.  

크롬에서 F1, 윈도우에서 F1은 cmd에서 help 명령어와 같다. 어떤 것이 나에게 쓸모 있는지 확인하기 위해서 한번 쭉 보면 나쁘지 않다.   
일단은 책에 있는 것들을 기준으로 확인해보려고 한다.  
[w11]는 윈도우11에서, [c]는 크롬에서 단축키이다., [vs]는 visualstudio에서의 단축키이다.  

[w11] f2 : 파일이나 폴더 명을 gui로 선택하여 바꿀 때 편리하다. 기존 방식(오른쪽 클릭 - 추가옵션표시 - rena(m)e)은 3번 눌러야 하는데 1번 누르면 된다.  
[c] f2 : 아무 기능 없음.  

=> f2 : 파일/폴더 이름 바꾸기 단축키인데 윈도우 11에서는 쓸만 한듯.  

[w11] f3 : 윈도우 파일 탐색기 폴더에서 검색 기능  
[c] f3 : ctrl + f 기능과 동일  
[vs] f3 : 현재 디렉토리 폴더로 잡혀 있는 곳에서 검색 기능 ex) .js, .html 등으로 검색할 수 있음.  

=> f3 : 검색과 관련된 기능  

vs code에서 특이하게 파일 탐색기 영역에서 f3와 파일내에서 f3가 검색 기능이 다름.(아무도 모르는 숨겨진 기능~)  
크롬탭에서 ctrl + shift + a를 하면 수많은 탭과 최근에 닫은 탭을 찾을 수 있다.(방대한 탭으로 띄어 놓고 비교 및 참고 쓰는 방법)  

[w11] f4 : 주소 표시줄로 바로 감.   
[c] f4 : 아무 기능 없음. 똑같은 기능으로 f6이 있음.
[vs] f4 : 아무 기능 없음.  

=> f4 : 윈도우 폴더 탐색기에서 주소창 바로가기 기능인데 이와 비슷한 유용한 단축키로 크롬에서 ctrl + k, /가 있다.  
마크다운에서 ctrl + k를 누르면 다음과 같이 url이 뜬다. "([](url))"  

[w11] f5 : 새로고침
[c] f5 : 새로고침
[vs] f5 : 디버깅

=> 새로고침은 매우 재밌는 기능이다. restart, refresh, reload, reboot 등 다양한 표현으로 사용된다. re와 new의 차이점은 re는 기존의 것을 반복하는 것이지만 new는 기존의 것에서 새로운 것을 추가하는 것이다.    
그래서 new file(새 파일 만들기)는 매우 이상한 번역이다. 프로그램 관점에서 사용자가 새로운 파일을 만드는 것은 엄밀하게 불가능한 일이다. 왜냐하면 기존의 템플릿을 가져다가 빈 파일을 만드는 것이기 때문이다.  

한편 크롬탭 전부를 모두 한꺼번에 새로고침을 하는 방법이 있다. 첫번째 탭 안에서 맨 끝 탭을 shift + 클릭을 하면 다 선택이 된다. 그리고 f5를 누르면 모든 탭에 새로고침을 명령이 들어간다.  
=> alt + space + t를 눌러서 ctrl + shift + t를 누르는 방법도 있다.

[w11] f6 : 전환  
[c] f6 : 주소창, 탭 메모리 사용량 표시  
[vs] f6 : 아무 기능 없음  

=> 크롬에서 쓰는 것 말고는 쓸모가 없다. 윈도우에서 f6와 tap의 차이점이 있긴 하지만 큰 의미는 없다.  

[w11] f7 : 아무 기능 없음
[c] f7 : 캐럿 브라우징
[vs] f7 : 아무 기능 없음

=> 캐럿 브라우징이 도대체 뭘까? tap키와 비슷한 기능인데 웹 페이지에 있는 것들을 마우스가 아닌 키보드 커서로 탐색하는 기능이다.  
재밌는 기능은 커서의 위치에 따라서 접속할 수 있는 url이 크롬 하단에 검은색으로 뜨게 된다. 이러한 기능을 이용하여 한 페이지에서 다른 페이지의 url들을 탐색할 수 있다.  
평상시에는 쓰이지 않지만 숨겨져 있는 url을 찾을 때 쓸모 있을 것 같다.  

[w11] f8 : 아무 기능 없음  
[c] f8 : 아무 기능 없음  
[vs] f8 : 아무 기능 없음  
[github] f8 : 하이라이트 기능?  

=> 깃헙 페이지에서 내가 선택된 ui의 영역을 확인하기 위해 빈 공간을 누르고 f8를 누르면 해당 영역이 하이라이트 된다.  

f9는 아무런 기능이 없다.(다른 프로그램에서 사용할 때 쓰면 좋은 키이지 않을 까 싶다.  
키보드에 f1 ~ f12까지 있는데 만약 예비 키보드를 추가하여 단축키로써 사용할 수 있게 추가하고 해당 키보드 버튼을 눌러 특정한 기능을 수행하도록 플렛폼을 만든다면 재밌는 사업이 생길 것 같다.  

[w11] f11 : 파일 탐색기에서 보기로 하이라이트 된다.   
[c] f11 : 전체 화면으로 변경된다.  
[vs] f11 : 전체 화면으로 변경된다.  

=> 전체화면 모드는 창을 종료하는 버튼이 사라지고 하단에 있는 작업 표시줄이나 상단에 있는 탭의 자리까지 현재 사용하고 있는 창을 넓힌다.  
듀얼모니터를 사용할 때 전체화면 버튼은 사용되지 않는다. 윈도우에서 휴대폰과 연결이라는 기능이 있는데 휴대폰과 pc가 연결되어 휴대폰으로 전화가 오면 pc에서 확인할 수 있는 기능이다.  
cross device라고도 한다. 이와 비슷한 기능을 제공하는 (https://connect.oppo.com/en-US/agreement)이라는 곳이 있는데 잘 사용되지 않는 것같다.  

일반적이지 않는 가상의 화면을 기존의 그래픽 카드로 만들기 위해선 어떻게 해야할까? Randr12, nouveau, cuda와 같은 것들이 있는데 리눅스에서 xorg로 구현할 수 있다고 한다.  (https://www.youtube.com/watch?v=EZEMK-C-nSo)
