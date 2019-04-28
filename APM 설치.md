# 1.APM이란

APM은 apache+php+mysql이다.
apache는 apache재단에서 만든 HTTP서버로 다양한 추가기능에, 구축이 쉽다는 장점으로 많이 쓰인다.
MySQL은 DBMS의 종류중 하나로서, 우리가 데이터베이스구축하는데 쓰는 프로그램 중 하나이다.
PHP는 웹 서버상에서 쓰는 언어로, 일반 HTML+CSS+JS로는 DB접속을 구현하다거나, 그 외 고급기능은 구현 못하므로, 쓰는 언어이다.

출처 https://gwonhouse.tistory.com/2

## 2.Apache2 설치하기

먼저 root권한으로 변경한다.

    sudo su
   
Apache2 설치

    #apt-get install apache2

버전체크
   
    apache2-v
### 3.Php 설치하기

앞에서 root권한으로 변경했기 때문에 또 변경할 필요가 없다.

바로 php설치하기

    #apt-get install php

#### 4. mysql 설치하기

이것도 앞에서 root권한으로 변경해서 따로 변경할 필요가 없다.

mysql 설치하기

    #apt-get install mysql-server
    
참고자료:https://blog.lael.be/post/73
참고자료:https://zetawiki.com/wiki/%EC%9A%B0%EB%B6%84%ED%88%AC_MySQL_%EC%84%A4%EC%B9%98
