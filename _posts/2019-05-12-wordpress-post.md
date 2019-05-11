---
title: "Welcome to Jekyll!"
date: 2019-05-12 01:46:02 -0400
categories: jekyll update
---
# 1. CMS란 
  
  인터넷을 통해 제공하는 각종 정보나 그 내용물들을 관리하는 시스템이다. ex) wordpress,drupal,joomla
  
# 2. WordPress 설치하기

## 1. mysql database 추가 및 설정
  이 과정은 root권한에서 실행해야된다.

![wordpress1](https://user-images.githubusercontent.com/49421197/57210204-c187ba80-7016-11e9-8883-57aa27f105cd.png)
  다음 명령어로 mysql에 접속
    $mysql -uroot -p
 
![wordpress2](https://user-images.githubusercontent.com/49421197/57210229-d9f7d500-7016-11e9-8037-38c5cf49aafc.png)

  나만의 database를 추가한다.

![wordpress3](https://user-images.githubusercontent.com/49421197/57210235-df551f80-7016-11e9-8b60-2d6a3216c586.jpg)

  사용자 계정을 만들고 동시에 데이터베이스 사용권한도 부여해준다.

## 2.  wordpress 설치하기
이 과정은 사용자 권한에서 수행해야된다.

![wordpress4](https://user-images.githubusercontent.com/49421197/57210282-0dd2fa80-7017-11e9-8c14-a10b6bb1e812.png)

wordpress.org홈페이지에 들어가서 다운로드 주소를 복사한다.

![wordpress5](https://user-images.githubusercontent.com/49421197/57210307-23e0bb00-7017-11e9-93dc-5a523b3335f1.png)

  pgkim사용자 계정으로 전환한 다음 html디렉토리에 들어가 wordpress를 설치한다.
    $weget [복사한 주소]

![wordpress6](https://user-images.githubusercontent.com/49421197/57210308-26dbab80-7017-11e9-9c3c-bf9333e84079.png)

  latest.tar.gz라는 압축파일이 생성된다.
    $tar xvzf latest.tar.gz
  다음 명령어로 압축파일을 풀어준다.
![wordpress8](https://user-images.githubusercontent.com/49421197/57210333-4541a700-7017-11e9-814d-6a38438b5815.png)

documentroot를 /home/pgkim/html/wordpress로 변경해줘야 된다.

## 3. wordpress config 파일 수정하기
  압축파일을 풀면 wordpress라는 디렉토리가 생성된다.
  디렉토리에 있는 wp-config-sample.php를 복사한다.
    $cp wp-config-sample.php wp-config.php
  wp-config.php파일이 주요 설정내용이 저장되는 곳이다.
![wordpress7](https://user-images.githubusercontent.com/49421197/57210326-3bb83f00-7017-11e9-9c24-fb3a61c3c393.jpg)

  전에 설정해주었던 database이름과, 사용자 계정 정보를 적어주면 된다.
  
  pgkim.com에 들어가면 다음과 같은 화면이 나온다.
  
![wordpress9](https://user-images.githubusercontent.com/49421197/57210340-483c9780-7017-11e9-88cf-2e27447c1bec.png)

  내용을 차례로 다 입력해준다.

![wordpress10](https://user-images.githubusercontent.com/49421197/57210344-4d014b80-7017-11e9-9aea-aec1b29eb25d.png)




