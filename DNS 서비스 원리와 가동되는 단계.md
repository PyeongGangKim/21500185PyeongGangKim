# 1.DNS란?

DNS는 domain name system으로 사람이 읽을수 있는 도메인 이름을 머신이 읽을수 있는 IP주소로 변환하는 시스템입니다.

# 2.DNS 서비스 원리

웹 브라우저는 입력된 도메인 주소의 서버와 통신을 하기 위해 PC에 설정된 DNS 서버와 DNS 메시지를 교환하여
해당서버의 IP 주소를 획득하고, 사용자의 요청에 따라 원하는 정보들을 받아온다.

이때 PC로부터 DNS 질의를 받아 도메인 주소에 매핑되는 IP 주소를 받아오는 과정을 수행하고, 
결과 값을 전달하는 DNS 서버를 LOCAL DNS서버라 한다.

DNS는 domain name space, name server, resolver로 구성된다.

domain name space:

DNS는 거대한 분산 네이밍 시스템이며, 도메인 네임 스페이스는 이러한 DNS가 저장/관리하는 계층적 구조를 의미한다.

도메인 네임 스페이스는 최상위에 ROOT DNS 서버가 존재하고, 그 하위로 인터넷에 연결된 모든 노드가 연속해서 이어진 계층 구조로 구성되어 있다.

각 레벨의 도메인은 그 하위 도메인 관한 정보를 관리하는 구조이다. 디렉토리 구조와 유사하다.

Name server:

숫자로 구성된 IP주소와 함께 사용하기 편리하고 기억하기 쉬운 도메인 이름을 사용한다. 

실제 웹 클라이언트 - 웹 서버 간의 통신은 숫자로 표현된 IP 주소를 사용하여 통신하는데, 이를 위해서는 문자열로 표현된 도메인 이름을
실제 컴퓨터가 통신할 때 사용하는 숫자로 표현된 IP 주소로 변환시켜주어야 된다. 이러한 동작을 하기 위해서는 Domain Name Space의 트리구조에
대한 정보가 필요하며, 이러한 정보를 가지고 있는 서버가 Name Server다. 도메인 이름을 IP주소로 변환하는 것을 네임 서비스라고 한다.

리졸버로부터 요청 받은 도메인 이름에 대한 IP 정보를 다시 리졸버로 전달해주는 역할을 수행한다.

Resolver:

리졸버는 웹 브라우저와 같이 DNS 클라이언트의 요청을 네임 서버로 전달하고 네임 서버로부터 정보를 받아 클라이언트에게 제공하는 기능을 수행한다.

참고자료: https://m.blog.naver.com/PostView.nhn?blogId=sharp428&logNo=220633341869&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F

# 3. DNS 가동되는 단계

ex1)

(1) 브라우저가 설치된 컴퓨터는 www.google.com 의 IP를 알아내기 위해서 가장 가까운 곳에 위치한(클라이언트에 등록된 ) DNS 서버에 www.google.com 의 IP 주소를 문의 합니다.

(2) 가장 가까운 DNS 서버가 IP주소를 알고 있다면 즉시 IP 주소를 알려 줍니다. 하지만 가장 가까운 DNS 서버가 IP 주소를 모르면 루트 도메인 네임서버에게 문의를 합니다. 

(3) 루트 네임서버는 도메인의 최상위 도메인이 .com인 것을 보고 “.com” 이 등록된 네임서버의 IP어드레스를 전달 합니다. 
이것에 대한 내용을 이해 하기 쉽게 예를 들어 설명 하면 다음과 같이 설명 할 수 있습니다. "나는 IP 주소를 가지고 있지 않지만,“.com” 네임서버에게 물어보면 도와 줄꺼야"  

(4) 가장 가까운 DNS는 “.com” 도메인을 관리하는 네임서버에게 문의합니다. 

(5) “.com” 네임서버는 google의 네임서버의 IP 주소를 알려줍니다. 

(6) 가장 가까운 DNS 서버는 google 의 네임서버에게 문의합니다. 

(7) www 의 네임서버를 알려 줍니다. 

(8) 최종적으로 www 네임서버에게 문의  합니다. 

(9) www.google.com 의 IP 주소를 얻을 수 있습니다. 

(10) 가장 가까운 DNS 서버는 이 IP 주소를 클라이언트에게 알려 주게 됩니다.

참고자료:https://m.blog.naver.com/PostView.nhn?blogId=sthox18&logNo=220411792949&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F


ex2)

(1) www.naver.com이라고 검색하면 사용자의 PC에 설정되어 있는 Local DNS라는 곳에 www.naver.com의 IP주소를 물어봅니다.

(2) Local DNS에 www.naver.com의 IP주소가 없다면, Root Dns에 찾아가서 www.naver.com의 주소를 묻는다.

(3) Root DNS가 www.naver.com의 주소를 알지 못한다면, 최상위 도메인 .com을 보고 .com이 등록된 네임서버의 IP어드레스를 알려준다.

(4) 다시 Local DNS가 .com 도메인을 관리하는 네임서버에게 문의한다.

(5) .com 네임서버는 naver.com의 네임서버의 IP주소를 알려준다.

(6) 다시 Local DNS가 naver.com 네임서버에게 문의하고

(7) naver.com 네임서버는 www.naver.com의 IP주소인 222.122.195.6을 알려준다.

(8) Local DNS는 알게된 IP주소를 PC에게 전달하고 PC는 사용자에게 성곡적으로 인터넷에 접속된 화면을 보여준다.

참고자료:https://m.blog.naver.com/PostView.nhn?blogId=daouidc&logNo=220880345370&proxyReferer=https%3A%2F%2Fwww.google.co.kr%2F
