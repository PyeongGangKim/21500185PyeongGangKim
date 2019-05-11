---
title: "Welcome to Jekyll!"
date: 2019-05-12 01:50:02 -0400
categories: jekyll update
---
# 1.apt-get install

![apt-get install](https://user-images.githubusercontent.com/49421197/57180228-90e23c80-6ec1-11e9-986d-62171872e84b.png)

새 패키지를 설치할 때 사용하는 명령어이다. 이전에 설치해놨기 때문에 따로 설치는 되지 않는다.

# 2.apt-get update
![apt-get update1](https://user-images.githubusercontent.com/49421197/57181804-6dc08880-6ed3-11e9-8687-41b1ab69a3de.png)

![apt-get update2](https://user-images.githubusercontent.com/49421197/57181805-6dc08880-6ed3-11e9-8959-95c483fe816d.png)

사용 가능한 패키지들과 그 버전들의 리스트를 업데이트 하는 명령어. 

실제 패키지 버전을 업그레이드하는 것이 아니라 최신 버전 패키지가 있는지를 확인하고 내 우분투에 알려주는 용도.

그래서 이거는 따로 인수를 받을 필요가 없다.


# 3.apt-get upgrade

![apt-get upgrade2](https://user-images.githubusercontent.com/49421197/57181923-96954d80-6ed4-11e9-85bc-a3f94b77fb95.png)

![apt-get upgrade3](https://user-images.githubusercontent.com/49421197/57181925-98f7a780-6ed4-11e9-8673-54af7553f151.png)

내 우분투에 있는 패키지들을 실제로 최신 버전으로 업그레이드 시키는 명령어다.

![apt-get upgrade](https://user-images.githubusercontent.com/49421197/57180240-9fc8ef00-6ec1-11e9-9d9d-0a14751a0c08.png)

다음에 보는 것 같이 인수로 특정한 패키지를 받으면 그 패키지만 업그레이드 시킬 수 있다.

# 4.apt-get remove

![apt-get remove](https://user-images.githubusercontent.com/49421197/57180242-a6576680-6ec1-11e9-9617-18d6ceeb7c79.png)

apt-get remove mysql-server는 mysql-server패키지만 삭제하고 설정파일은 지우지 않는 명령어다.

# 5.apt-get autoremove

![apt-get autoremove](https://user-images.githubusercontent.com/49421197/57180247-ace5de00-6ec1-11e9-8de4-58bcdc1cee36.png)

인자를 받지 않으면 알아서 필요없는 것을 지워준다.
apt-get autoremove mysql-server는 패키지와 패키지가 삭제되면 필요하지 않는 패키지까지 삭제된다.
즉 mysql-server에 의존성이 있던 모든 패키지가 삭제된다.

# 6.apt-get purge

![apt-get purge](https://user-images.githubusercontent.com/49421197/57180252-b4a58280-6ec1-11e9-8d55-90b192ec2622.png)

패키지뿐만 아니라 설정파일도 삭제하는 명령어이다.

# 시스템 설정 파일이란
커널 그 자체는 "프로그램"이다. 커널에 설정 파일이 필요한 이유는? 커널은 시스템의 사용자와 그룹의 리스트를 알고 있어야 한다. 파일 권한도 관리해야 한다. 이러한 파일들은 프로그램에 의해 읽히지 않고 시스템 라이브러리의 함수에 의해 읽혀지며 커널에 의해 사용된다는 것에 주목하라. 예를 들어, 사용자의 (암호화된) 패스워드를 필요로 하는 프로그램은 /etc/passwd 파일을 열어서는 안된다. 대신, 시스템 라이브러리 함수인 getpw()를 호출해야 한다. 이러한 종류의 함수는 시스템 호출(system call)로 알려져 있다. /etc/passwd 파일을 열고 요청된 사용자의 패스워드를 찾는 것은 커널의 몫이다.
Red Hat Linux 시스템의 설정 파일 대부분은 /etc 디렉토리에 있다. 설정 파일들은 다음과 같은 카테고리로 광범위하게 구분된다

참고문서:https://www.cyber.pe.kr/2013/11/linux_9648.html
