# 😃 설계와 테스트
</hr>

설계의 방향
-----  
> 상향식설계, 하향식설계 의 기준을 설명하시오 
* 설계의 세부사항, 인터페이스의 완성도가 아님  
* **결합의 여부**가 상향식이냐 하향식이냐

설계분석론
----
> Wrfs-Block
* 분석과 설계의 구분없이 고객명세서부터 설계작업까지 연속적 수행을 하는 설계론
> Rumhaugh
* 객체, 동적, 기능순으로 분석하는 분석론
> Booch
* Micro와 Macro로 나눠서 분석하는 방식
> Jacobson
* UseCase로 분석하는 방식
> Coad Yorudon
* E-R 다이어그램을 사용하여 객체 행위 모델링을 통해 분석하는 방식
> LOC : 낙관 / 기대 / 비관   
> 테일러링   
> PUTNAM   
* 소프트웨어 개발 주기의 간 단계별로 요구할 인력의 분포를 가정하는 모형입니다.
Putnam 모형과 Rayleigh Noden 곡선을 기초로 개발한 자동화 추정 도구로 SLIM이 있습니다.
> SLIM    
> FP   
* 기능점수(FP) 모형 (비용산정)
> PERT   
* 프로그램 평가(Program Evaluation) 및 검토 기법(Review Technique)
> 델파이기법  
* 전문가들의 의견수립, 중재, 타협의 방식으로 반복적인 피드백을 통한 하향식 의견 도출 방법으로 문제를 해결하는 기법
> Effort Per Task   
* 개발 단계별 인월수 기법은 LOC 기법을 보완하기 위한 기법으로, 각 기능을 구현시키는 데 필요한 노력을 생명 주기의 각 단계별로 산정

UI 설계도구
-----  
> 와이어프레임~프로토타입의 순서를 설명하시오  
* 와이어프레임 > 목업 > 스토리보드 > 프로토타입    

Agile Scrum에서 각각의 단어를 설명하시오
-----  
> Backlog   
> Sprint(2~4w)   
> Velocity   

요구분석
----
> 기능적 요구
* 주로 코드상의 내용
> 비기능적 요구
* 주로 품질에 대한 내용

아키텍처
----
> 마스터 슬레이브 아키텍쳐
* > 슬레이브의 제한사항
  * 슬레이브는 마스터의 기능(연산,통신,조정) 외에 제한없음

UML 
----
> 정적 다이어그램
  * > 클래스
    * > 구성요소
      * 이름, 속성, 오퍼레이션
  * > 객체
  * > 컴포넌트
  * > 배치
  * > 복합체
  * > 패키지
> 동적 다이어그램
  * > 유스케이스
  * > 순차
  * > 커뮤니케이션
  * > 상태
  * > 활동
> 포함과 집합
  * 포함은 집합의 특수한 형태
> 사물이 해야하는 기능(오퍼레이션)을 지정하는 UML
  * 실체화 UML

개발모형
----
> 나선형
* 리스크관리
> 폭포수 변환
* V모델
> HIPO 
* Hierarchy Input Process Output
* 하향식 소프트웨어 개발을 위한 문서화 도구
> 라우터   
* 컴퓨팅 디바이스와 네트워크를 다른 네트워크에 연결하는 네트워킹 디바이스
> RAD   
* 도구로 디자인하고 Code Generator를 활용해 빠르게 개발하는 기법

테스트
----
> 스텁이란?
* 서버가 구현, 하위모듈을 대체
* 하향식 통합테스트, 파라미터 전달
> 태스트 드라이버란?
* 클라이언트가 후현, 상향모듈을 대체
* 인자값을 넘겨주는 상향식 통합테스트
> CASE(Computer Aided SoftWare Enginerring)
* 자동화 도구, 테스트 방법론
  > 상위 케이스
    * 문제를 기술, 설계 지원
  > 하위 케이스
    * 코드 작성테스트, 문서화 지원
  > 통합 케이스
    * 생명주기에 포함되어있는 전과정 지원

테스트 이론
----
> FTR (Formal Technical Review)
* 검토에만 집중하기 위해, 검토 이외의것을 모두 제한하는 방식(논쟁,인원 등등)
> Revese Engineering
* 일반적인 개발 단계와는 반대로 기존 코드를 복구하거나 소프트웨어 관계를 추출하는 방식
> Alien Code
* 참고문서와 관리하는 개발자가 없어 유지보수가 어려운 프로그램 코드
> 화이트박스 검사, 블랙박스 검사
* 실행 경로의 기초(내부적)를 정의하는 검사와, 내부를 보지않고 입력과 출력에 중점을 둔 검사의 차이

인터페이스 구현 검증 도구
---
> xUnit   
> TAF   
  * >  Test Automation Framwork
    * STAF, NTAF
> FitNesse
  * Test Wiki
> watir
  * Ruby Test

기타개념
----
> Cocomo Model Line Standard
* 5만, 30만 -> 조직, 반분리, 내장 
> Basis Path
  * 수행가능한 모든 경로 
> LOC기법   

</br></br>

# 😃 개발 디자인
</hr>

SOLID
----
> S
* Solo Responsibility
> O
* Open-close
> L
* Liskov : super()
> I
* Interface Segregation
> D
* Dependency : child -> parent

GoF 디자인패턴의 종류
----
> 3가지 분류 기준
* 생성 / 구조 / 행위
* 정의 / 확장 / 상호작용
  > 생성의 네가지 종류  
    * 팩토리 , 빌더 , 프로토 , 싱글톤
    * > 팩토리   
      * > 추상팩토리  
        * 인터페이스
      * > 팩토리 메소드 
        * 객체 생성을 서브클래스에서
    * > 빌더
      * 인스턴스의 조합
    * > 프로토
      * 원본객체를 복사
    * > 싱글톤   
  > 구조
    * > 구조값이라고 상상 가능한 패턴
      * > 어뎁터
        * 호환성 없는 클래스들을 이용할수 있도록 변환
      * > 브릿지
        * 구현부에서 추상층 분리, 독립적 확장
      * > 데코레이터
        * 객체간의 결합을 통해 기능확장
      * > 프록시
        * 접근하기 어려운 객체에 연결
    * > 구조값이라고 상상 불가능했던 패턴
      * > 컴포지트
        * 복합객체, 단일객체 구분없이 사용
      * > 퍼싸드
        * 복잡한 서프클래스를 피해 더 상위 인터페이스
      * > 플라이웨이트
        * 인스턴스를 가능한한 공유해서 씀
  > 행위
    * > 행위값이라고 상상 가능했던 패턴
      * > 책임연쇄
        * 객체가 둘 이상 존재하면, 한객체가 처리하지 못할시에 다음으로 넘어가는 패턴
      * > 옵저버
        * 변화하는 상태를 전달
    * > 행위값이라고 상상 불가능했던 패턴
      * > 상태
        * 객체의 상태값에 따라서 동일한 동작을 다르게 처리
      * > 방문자
        * 데이터 구조에서 처리기능을 분리, 별도의 클래스로 구성하는 패턴
      * > 커맨드
        * 요청을 객체의 형태로 캡슐화 하고, 로그에 남기는 패턴
      * > 인터프리터
        * 언어에 문법 표현을 정의
      * > 반복자
        * 동일한 인터페이스를 사용
      * > 중재자
        * 수많은 객체간의 복잡한 상호작용을 캡슐화
      * > 메멘토
        * 특정 시점의 객체 내부상태를 객체화
      * > 전략
        * 동일계열 알고리즘을 개별적으로 캡슐화
      * > 템플릿메소드
        * 상위 클래스에서 골격을 정의, 하위클래스에서 세부처리

> 디자인패턴에 대한 새로운 표현
* 자주 발생하는 문제에 대한 반복적인 해결방법

응집도과 결합도
----
> 좋은소프트웨어
* 응집도는 높게(명령에 대한 구조) , 결합도는 낮게
> 응집도 순서 (아웃풋이 얼마나 스노우볼이 구르는지)
* 기능적
* 순차적 (순차가 끝나면 그다음은)
* 통신적 (통신한 모듈끼리 모이면)
* 절차 (절차들이 모이면)
* 시간 (시간이 모여야)
* 논리 (논리가 된다)
* 우연 : 어떤 의미도 없이 연관관계가 없는것
> 결합도 순서 
* (전체에서 점점 작아지고나서, 작아진것에서도 신호 -> 인터페이스 -> 파라미터순으로 작아짐)
* 내용
* 공통
* 외부
* 제어
* 스탬프 (스탬프가 인터페이스를 의미)
* 자료

</br></br>

# 😃 네트워크
</hr>

경로제어 routing 프로토콜
---
> IGP
  * > Interior Gateway Protocol (동일그룹)
  * > OSPF
    * Open Shortest Path First
  * > RIP
    * > Routing Infomation Protocol
      * Hop Counting
> EGP   
  * > Exterior Gateway Protocol (외부그룹)
> BGP   
  * > Boarder Gateway protocol (종속 게이트웨이)

> 임계 구역 접근 상호 배제
* Semaphore (신호깃발이라는 뜻)
> FAT -> NTFS
* 상대적 대용량, 대신 속도가 늘려짐 
> VLAN   
* 논리적으로 분할된 스위치 네트워크 : 동적인 조직에서 작업 그룹을 구성할 수 있음
> STP   
* Spannging Tree Protocol
* 2개 이상의 스위치가 여러 경로로 연결될때, 무한 루프 현상을 막기 위해 우선순위에 따라 1개로 통신하는 프로토콜
> L2AN
* OSI의 2계층에 속하는 장비로, MAC 주소를 기반으로 프레임을 전송하고 동일 네트워크 간의 연결만 가능
> SDS 
* 물리적인 데이터 스토리지를 가상화하여 여러 스토리지를 하나처럼 관리하거나, 여러 스토리지로 나눠 사용하는 소프트웨어
> MLFQ  
* Multi-level Feedback Queue 
> MQTT   
* 경량 머신 대 머신 통신에 사용되는 표준 기반 메시징 프로토콜
* 발행 - 구독 기반의 메세징 프로토콜
> Zingbee   
* 소형, 저전력 디지털 라디오를 이용해 개인 통신망을 구성하여 통신하기 위한 표준 기술
> MessageBus   
> Hub & Spoke   
> HyBrid   
> MBR
* 파티션된 기억 장치(이를테면 하드 디스크)의 첫 섹터 (섹터 0)인 512 바이트 시동 섹터이다   
> NAC  
* 네트워크 접근제어(Network Access Control)는 네트워크에 접속하는 장치에 대해 접속 가능 여부를 확인하여 인가된 장치만이 접속할 수 있도록 제한하는 것
> NIC   
* 네트워크 인터페이스 컨트롤러(network interface controller, NIC)는 컴퓨터를 네트워크에 연결하여 통신하기 위해 사용하는 하드웨어 장치
> Topology   
* 단어 그 자체로 망 구성방식
* 컴퓨터 네트워크의 요소들(링크, 노드 등)을 물리적으로 연결해 놓은 것, 또는 그 연결 방식
> SNMP  
*  UDP/IP(사용자 데이터그램 프로토콜/인터넷 프로토콜)를 사용하여 이더넷 연결을 통해 네트워크 관리 작업을 수행하는 응용 계층 프로토콜 
> FLSM   
* Fixed Length Subnet Mask  <-> VariableLength Subnet Mask
> ARQ  
* ARQ는 Automatic Repeat Request의 약자로, 자동 재전송을 의미한다 쉽게 말해, 에러가 발생할 경우 재전송을 요구하는 방식이다. 

IPv4와 IPv6정리
----
> 유티캐스트(1:1 통신 주소 자동설정)
* IPv4 
> 클래스별로 4개
* IPv4 
> 16비트 8개 -> 128비트
* IPv6
> 40옥텟 해더
* IPv6
> 속도가 비교적 빠르고 v4와 호완
* IPv6

TCP/IP
----
> ARP(Address * *)
* IP to MAC Address
> ICMP
* Error Message - Internet Control Message Protocol
> Point to Point
* 각각 서버와 클라이언트가 둘다 될수있는 방식(Point to Point)의 프로토콜

IPv4 Class 정리
----
> A (0)   
* 0.0.0.0 ~ 127.255.255.255
> B (10)   
* 128.0.0.0 ~ 191.255.255.255
> C (110)
* 192.0.0.0 ~ 223.255.255.255
> D    
* 224.0.0.0 ~ 239.255.255.255
> E    
* 240.0.0.0 ~ 247.255.255.255
> 기준값
* 127부터 64 / 32 / 16 / 8을 더함

DRM
---
> Clearing House   
> Contents Provider   
> Packager   
> Contents Distributor   
> DRM Controller   
> Security Container   

DFS
----
> 순회 기준 우선순위
* 자식, 형제, 상위

STACK
----
> 넘어가거나 없는데 포인트를 내리거나
* Overflow, Underflow
> Stack Guard   
* Stack을 이용하여 변조를 탐지, BOF공격 탐지

</br></br>

# 😃 데이터 베이스
</hr>

데이터베이스 설계
----
> 데이터베이스 설계 단계
* 개념 / 논리 / 물리 단계 
* 스키마 / 인터페이스 / 트래픽 관련
* 뒤에 단계는 앞에 단계를 검증하는것을 포함할수있다

E-R 다이어그램
----
> 사각형 / 마름모 / 타원 / 이중타원 / 밑줄 타원 / 복수타원 / 선
* Entity / Relaction / Attribute / 다중속성 / PK / 복합속성 / Link

DB SC 용어
----
> Degree   
> Cardinality   
> Tupel  
> Attribute      
> Domain    
> DISTINCT   
> JOIN   
> UNION   
> UNION ALL   
> INTERSECT   
> EXCEPT   
> CASCADE   
> RESTRICTED   
> View는 SQL의 제한이 있음   

병렬 데이터베이스 수평분할
---
> 데이터 튜닝기법
  * > 목록분할
    * 특정 칼럼을 기준으로 파티셔닝
  * > 조합분할
    * 여러가지를 조합하여(합성) 파티셔닝
  * > 해시분할
    * 해시 함수를 적용하여 파티셔닝
  * > 범위분할
    * 범위에 있는지 여부로 파티셔닝
  * > 라운드 로빈
    * 행의 고른 분포로 파티셔닝

정규화 과정
----
> 도메인이 원자값   
> 부분적 함수 종속 제거
* 부분키로도 특정이 가능하다면
> 이행적 함수 종속 제거 
* X->Y Y->Z라면   
> 결정자이면서 후보키 아닌것 제거   
> 다치 종속 제거   
> 조인 종속 제거   

카티션 프로덕트
----
> 차수
* degree + degree
> 튜블
* cardinary * cardinary

접근통제 기술
----
> 임의    
* DAC, Discretionary Access Control
* GRANT , REVOKE가 예시
> 강제    
* MAC, Mandatory Access Control
> 역할기반    
* RBAC , Role Based Access Control

스토리지 시스템
----
> DAS
* Direct
> NAS
* Network
> SAN
* Nas + Das

관계대수
----
> 순수연산자
  * > Project
  * > Select
  * > Join
  * > Devide    
> 연산이상현상  
  * > 삽입   
  * > 삭제   
  * > 갱신   

정렬과 BIG(O)
----
> 버블
  * > 버블처럼 돌아가면서 계속 비교
    * n^2 / n^2
> 선택
  * > 선(Linear)로 비교
    * n^2 / n^2
> 삽입
  * > 하나씩 빼서 올바른 위치에 비교삽입
    * n^2 / n
> 병합
  * > 반반씩 나누어서 비교후 합치기 (계속해서 나눔)
    * nLogN / nLogN
> 퀵
  * > pivot을 사용하여 분할정렬
    * nLogN / nLogN


</br></br>

# 😃 운영체재
</hr>

가상기억장치 구현
---
> 보조기억장치(하드디스크)를 주기억장치처럼 사용(RAM)
  * > 페이징
    * 내부단편화
    * 가상과 주기억을 동일하게 나눈뒤 적재
    * > 페이징맵 테이블 
      * 비용증가, 처리속도 느려짐
  * > 세그멘터이션
    * 외부단편화
    * 가상과 주기억을 논리적으로 나눈뒤 적재
    * 세그멘테이션 테이블

운영체재 자원 배분
---
> Best , Worst, First Fit의 정의   
* 어떻게 배치할 것인가
> 스레싱
* 프로레싱 처리기간보다, 쓰레드 배치 시간이 길어지면 나타나는 현상
* 페이지 부재가 많아짐
> 교착상태 해결법 
* > 예방
  * 교착상태 발생조건 제거(부정)
* > 회피
  * 은행원 알고리즘
* > 발견
  * 자원할당 그래프
* > 회복
  * 프로세스 자원 회복


> SSTF Scheduling   
* (Shortest Seek Time First) : 현재 디스크의 헤드 위치에서 가장 가까운 실린더에 대한 요청을 우선적으로 처리한다.

페이지 교체 알고리즘
----
> FIFO
> OPT
* 가장 오래 사용하지 않은것 교체
> LRU
* Least Recently Used <> OPT
> LFU
* Least Frequenly Used
> MFU
* Most Frequenly Used

리눅스
----
> umask
* 초기 권한 설정값으로 파일은 666, 폴더는 777 에서 뺴는값
> 쉘스크립트 Export
* 환경변수를 설정

ISO 용어 정리
----
> ISO/IEC 25000
* 소프트웨어 품질 관련 국제 표준, 2501n은 외부 품질, 2502n은 내부 품질 기준
> ISO 12207와 SPICE 비교
https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=azurecourse&logNo=220041626265

잊기 쉬운 짧은 개념들
----
> Hash함수
* 일방향 함수다.
* HAVAL , SHA-1
> CIDR 서브넷마스크 계산법
* /(1의 갯수) 와 옥텟을 기억

</br></br>

# 😃 언어 개념 
</hr>

C언어 포인터 정리
----
> 연산자 우선순위 총정리
* [] , *
* 나머지는 넘기기
> 참조와 역참조
* *p *(*p)
* 역참조 할때마다 한단계 위로 올라간다고 생각하면 편함(다차원배열에서)
> 포인터 배열과 배열의 포인터
* int *p[3]
* int (*p)[3]
> 비트연산기호   
> 라이브러리   

기타언어
----
> << 시프트 기호의 의미   
* 2진수를 하나밈 
> Scrapy
* 파이썬 기발 크롤링 프레임 워크

</br></br>

# 😃 보안과 오류 
</hr>

* 디버깅은 오류의 수정을 이야기함
> postfix
  * >  연산자가 피연산자 두개뒤에 놓이는 방식
      * Stack으로 연산

Buletooth Attack
----
> Bug 
* 원격조정, 전화, 감청
> Snarf (허겁지겁먹다)
* 파일에 접근
> Printing 
* 검색을 하는 활동
> Jacking 
* 명함을 익명으로 퍼뜨림

DOS
----
> Smaurfing 
* ICMP(error)를 활용하여 집중적으로 대용량 데이터 공격
> Ping of Death 
* 정상크기보다 큰 ICMP를 쪼개서 보내어 패킷을 처리하게 만듬
> SYN Flooding (Sync)
* 존재하지 않는 클라이언트가 접속하여 다른 사용자 사용불가능하게 만듬
> Land 
* 출발지와 목적지 IP를 동일하게 만듬
> Honeypot
* 비정상적인 접근 탐지
* 침입자를 속여 쉽게 공격이 가능한것처럼 보임
> DPI (Deep Packet Inspection)
* 해킹 탐지, 트래픽 조정, OSI 전 레이어 탐지
> PLCP (Packet Level Control Processor)
* 패킷 교환 시스템에서 정보 처리와 통계 등을 담당

코드기입오류 정리
----
* Transcription
* Transposition
* Double Transposition
* Omission
* Addtion
* Random

SSH
----
  * > 기능   
  * > Default Port
    * 22
  * > 공개키 위치
    * SERVER
  * 원격명령, 쉘 서비스

암호화
----
> DES
* 64비트 알고리즘
> AES
* DES를 발전, 128비트 알고리즘
> RSA
* 소수로 암호화 비대칭 암호화

보안및 공격방식
----
> Secure 코딩
* 공격자가 프로그램 코드를 실행시키게 만드는 방식 - 작동이 목적임
> C&C Server   
* C&C 서버는 Command & Control 서버, C2 서버, 명령제어 서버 등 다양하게 불리며 사이버 공격에서 두뇌 역할
> Botnet   
* 좀비 PC
> Zero Day Attack  
* 패치가 나오지 않은 시점에서 이루어지는 공격 
> Key Logger Attack   
* 컴퓨터 사용자의 키보드 움직임을 탐지해서 저장하고, ID나 패스워드, 계좌 번호, 카드 번호 등과 같은 개인 중요 정보를 몰래 빼가는 해킹
> Back Door
* 어떤 제품이나 컴퓨터 시스템, 암호시스템 혹은 알고리즘에서 정상적인 인증 절차를 우회하는 기법이다
> Brute-Force Attack   
* 암호학 무차별 대입공격
> Ping Flood   
* system에 ICMP packet을 계속해서 보내서, 대상 system이 Request 에 응답하느라 다른 일을 하지 못하도록 하는 공격
> Opcode   
* 기계어에서 명령코드를 나타내는 부호
> Salt  
* 데이터, 비밀번호, 통과암호를 해시 처리하는 단방향 함수의 추가 입력으로 사용되는 랜덤 데이터이다
> OWASP   
* 오픈 소스 웹 어플리케이션 보안 프로젝트, 가장 큰 오픈소스 웹 애플리케이션 보안 프로젝트로 주로 웹에 관한 정보노출, 악성 파일 및 스크립트, 보안 취약점 등을 연구
> Collision Domain   
* 동일한 collision domain에서 하나의 PC가 통신할 경우, 다른 모든 PC는 통신이 불가
> CSMA/CA   
* Carrier Sense Multiple Access / Collision Avoidance
* 반송파 감지 다중 엑세스 충돌 회피
> CSMA/CD   
* Carrier Sense Multiple Access / Collision Detect
* 반송파 감지 다중 엑세스 충돌 감지
> DSA   
* DSA는 미국의 전자서명 표준이다.
> IPSec  
* 네트워크에서의 안전한 연결을 설정하기 위한 통신 규칙 또는 프로토콜 세트 
* 터널모드와 전송모드
* 전송모드는 헤더로르 제외한 페이로드만 보호
* 터널모드는 전체 패킷을 보호
> nmap  
* NMAP은 port Scanning 툴(해킹방어)

기타 외워야하는 Service및 기술들
---
> 타조   
* 하둡(Hadoop) 기반의 분산 데이터 웨어하우스 프로젝트
> 원세그
* 일본의 이동방송 기술   
> 포스퀘어   
* 위치 기반 소셜 네트워크 서비스이자 이를 개발한 회사의 명칭
> ASLR  
* Address Space Layout Randomization의 줄임말입니다. 직역하면 "주소 공간 배열 무작위화" 입니다. 말 그대로 주소를 매번 실행할 때마다 무작위화시켜 공격을 방해 
> Sqoop 
* Hadoop과 관계형 데이터베이스 간에 데이터를 전송할 수 있도록 설계된 오픈소스 소프트웨어  
> N-Screen   
* 특정한 주제의 콘텐츠들을 여러 개의 스크린에서 동시에 볼 수 있다는 개념
> Memristor   
* Memory registor (이전의 상테를 기억하는 메모리)
> MEMS   
* Micro Electro Mechanical Systems (미세 전기 기계 시스템)의 약자로, 미세한 입체 구조 (3차원 구조)를 지니며, 다양한 입력 · 출력 신호를 취급하는 시스템의 총칭

카테고리화가 되지 않은 CS관련 IMG
----
>  NS Chart
* http://itnovice1.blogspot.com/2019/08/nsnassi-schneiderman.html
> AVL 다이어그램