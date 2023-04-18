# Computer Sciense Study Memo
</hr>   

설계
-----  
> 상향식설계, 하향식설계  
* 설계의 세부사항, 인터페이스의 완성도가 아님  
* **결합의 여부**가 상향식이냐 하향식이냐

UI설계도구  
-----  
> 순서대로 명칭과 형태를 인지  
* 와이어프레임 > 목업 > 스토리보드 > 프로토타입    

Agile Scrum
-----  
> Backlog, Sprint(2~4w), Velocity

UML 
----
> 정적 다이어그램과 동적 다이어그램에 대한 이해
* 구조를 설명하는것, 흐름을 설명하는것의 워딩 구분

SOLID
----
> 객체지향론
* Solo Responsibility
* Open-close
* Liskov : super()
* Interface Segregation
* Dependency : child -> parent

GoF 디자인패턴의 종류
----
> 생성 / 구조 / 행위
* 객체의 입장에서 정의 / 확장 / 상호작용
> 디자인패턴에 대한 새로운 표현
* 자주 발생하는 문제에 대한 반복적인 해결방법

데이터베이스 설계
----
> 개념 / 논리 / 물리 단계 순으로 설계
* 스키마 / 인터페이스 / 트래픽 관련 설계
* 뒤에 단계는 앞에 단계를 검증하는것을 포함할수있다

E-R 다이어그램
----
> 사각형 / 마름모 / 타원 / 이중타원 / 밑줄 타원 / 복수타원 / 선
* Entity / Relaction / Attribute / 다중속성 / PK / 복합속성 / Link

DB SC 용어
----
> Degree   
> Cardinality   
> Tupel : 수정 불가한 객체를 의미하기도함   
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

정규화 과정
----
> 도메인이 원자값   
> 부분적 함수 종속 제거 : 부분키로도 특정이 가능하다면   
> 이행적 함수 종속 제거 : X->Y Y->Z라면   
> 결정자이면서 후보키 아닌것 제거   
> 다치 종속 제거   
> 조인 종속 제거   

C언어 포인터 정리
----
> 연산자 우선순위
* [] , *
> 참조와 역참조
* *p *(*p)
* 역참조 할때마다 한단계 위로 올라간다고 생각하면 편함(다차원배열에서)
> 포인터 배열과 배열의 포인터
* int *p[3]
* int (*p)[3]

IPv4와 IPv6정리
----
>IPv4
* 호스트 주소 자동설정 (유티캐스트 지원 - 1:1 통신에 사용)
* 클래스별로 4개
>IPv6
* 16비트 8개 -> 128비트
* 40옥텟 해더
* 주소 자동설정
* 속도가 비교적 빠르고 v4와 호완

TCP/IP
----
>ARP(Address * *)
* IP to MAC Address
>ICMP
>PPP
* 각각 서버와 클라이언트가 둘다 될수있는 방식(Point to Point)의 프로토콜

응집도과 결합도
----
> 좋은소프트웨어
* 응집도는 높게(명령에 대한 구조) , 결합도는 낮게

개발모형
----
> 나선형
* 리스크관리
> 폭포수 변환
* V모델

스토리지 시스템
----
> DAS
* Direct
> NAS
* Network
> SAN
* Nas + Das

시스템 공격에관한 SC용어
----
> Buletooth(Blue + )
* Bug - 원격조정, 전화, 감청
* Snarf - 파일에 접근
* Printing - 검색을 하는 활동
* Jacking - 명함을 익명으로 퍼뜨림

> DOS
* Smaurfing - ICMP(error)를 활용하여 집중적으로 대용량 데이터 공격
* Ping of Death - 정상크기보다 큰 ICMP를 쪼개서 보내어 패킷을 처리하게 만듬
* SYN Flooding - 존재하지 않는 클라이언트가 접속하여 다른 사용자 사용불가능하게 만듬
* Land - 출발지와 목적지 IP를 동일하게 만듬

> Honeypot
* 비정상적인 접근 탐지
* 침입자를 속여 쉽게 공격이 가능한것처럼 보임

> DPI (Deep Packet Inspection)
* 해킹 탐지, 트래픽 조정, OSI 전 레이어 탐지

> PLCP (Packet Level Control Processor)
* 패킷 교환 시스템에서 정보 처리와 통계 등을 담당

암호화
----
> DES
* 64비트 알고리즘
> AES
* DES를 발전, 128비트 알고리즘

리눅스
----
> umask
* 초기 권한 설정값으로 파일은 666, 폴더는 777 에서 뺴는값

처음들어보는 SC 용어들정리
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
> FTR (Formal Technical Review)
* 검토에만 집중하기 위해, 검토 이외의것을 모두 제한하는 방식(논쟁,인원 등등)
> Revese Engineering
* 일반적인 개발 단계와는 반대로 기존 코드를 복구하거나 소프트웨어 관계를 추출하는 방식
> Alien Code
* 참고문서와 관리하는 개발자가 없어 유지보수가 어려운 프로그램 코드
> YAML 은 YML과 문법이 동일
> 분할정복에 기반하여 피봇을 사용하는 정렬
* Quick Sort
> 화이트박스 검사, 블랙박스 검사
* 실행 경로의 기초(내부적)를 정의하는 검사와, 내부를 보지않고 입력과 출력에 중점을 둔 검사의 차이
> ISO/IEC 25000
* 소프트웨어 품질 관련 국제 표준, 2501n은 외부 품질, 2502n은 내부 품질 기준
> 임계 구역 접근 상호 배제
* Semaphore (신호깃발이라는 뜻)
> Best , Worst, First Fit의 정의   
> FIFO, FLU, 페이지부재, 후순위 순회(LRR)   
> Python print 는 자동개행       
> << 시프트 기호의 의미   
* 2진수를 하나밈 
> Scrapy
* 파이썬 기발 크롤링 프레임 워크
> Secure 코딩
* 공격자가 프로그램 코드를 실행시키게 만드는 방식 - 작동이 목적임
> FAT -> NTFS
* 상대적 대용량, 대신 속도가 늘려짐 
> LOC : 낙관 / 기대 / 비관   
> 테일러링   

처음 보는 SC관련 IMG
----
>  NS Chart
* http://itnovice1.blogspot.com/2019/08/nsnassi-schneiderman.html

> 관계해석 논리 기호
* https://velog.io/@ln1992/16-%EC%9D%BC%EC%B0%A8-%EB%85%BC%EB%A6%AC-%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4-%EC%84%A4%EA%B3%84


