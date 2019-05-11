---
title: "HW7"
date: 2019-05-12 01:54:02 -0400
categories: jekyll update
---
# 1. Virtual Hosting이란

  하나의 물리적인 서버에서 2개 이상의 웹 사이트를 서비스 할 수 있도록 하는 방법
  
# 2. html 세팅  
## 1. 계정 추가

![계정 추가](https://user-images.githubusercontent.com/49421197/57215197-20edc680-7027-11e9-9be6-9d3f21259136.png)

## 2. 추가한 계정에 /home/kim에 html 디렉토리 만들기

![html디렉토리 생성](https://user-images.githubusercontent.com/49421197/57215277-54c8ec00-7027-11e9-8b58-8c9c365716ac.png)

![index html](https://user-images.githubusercontent.com/49421197/57215316-7033f700-7027-11e9-9005-97d51fdaa2fa.png)

html디렉토리에 index.html파일 생성

## 3. conf 파일 복사 후 수정
![2019-05-06 (35)](https://user-images.githubusercontent.com/49421197/57215406-be48fa80-7027-11e9-8c8a-a3da22ffb276.png)

[전에 했던거 참고하기](https://github.com/PyeongGangKim/21500185pyeonggangkim.github.io/blob/master/_posts/22019-05-02-%EB%8F%84%EB%A9%94%EC%9D%B8%20%EC%9D%B4%EB%A6%84%20%EC%84%B8%ED%8C%85%20%EB%B0%8F%20%ED%98%B8%EC%8A%A4%ED%8A%B8%20%EB%B3%80%EA%B2%BD-post.md)

![2019-05-06 (37)](https://user-images.githubusercontent.com/49421197/57215737-c35a7980-7028-11e9-8410-f1695c74ed52.png)

도메인 이름으로 구분할수 있다!!

## 4. 결과

![2019-05-06 (36)](https://user-images.githubusercontent.com/49421197/57215601-5b0b9800-7028-11e9-9124-9ba9b8f2f3c5.png)

## 5. 또 다른 계정 pg13

위와 동일한 방법으로 한다!!

![2019-05-06 (45)](https://user-images.githubusercontent.com/49421197/57215812-f7ce3580-7028-11e9-94be-91a50f8a34ac.png)

이것도 다른 도메인 이름을 사용해서 구분한다!!

![2019-05-06 (46)](https://user-images.githubusercontent.com/49421197/57215853-1a604e80-7029-11e9-8225-49bcabe9f83b.png)

# 3. wordpress 세팅!

## 1. database 만들기!!
[전에 했던 방법](https://github.com/PyeongGangKim/21500185pyeonggangkim.github.io/blob/master/_posts/2019-05-12-wordpress-post.md)

root 계정으로 들어가서
mysql -uroot -p 
명령어로 mysql에 접속

![2019-05-06 (39)](https://user-images.githubusercontent.com/49421197/57215912-4ed40a80-7029-11e9-83bc-3b52239903b4.png)

database을 만들기

![ss1](https://user-images.githubusercontent.com/49421197/57216076-c1dd8100-7029-11e9-93ac-0b3aaf1d3544.jpg)

생성한 데이터베이스의 사용자계정 만들기

![2019-05-06 (41)](https://user-images.githubusercontent.com/49421197/57216131-f3eee300-7029-11e9-8ebb-5006ce6cb925.png)

생성한 사용자 계정에게 데이터 베이스 사용 권한을 부여

![2019-05-06 (42)](https://user-images.githubusercontent.com/49421197/57222768-bea0c000-703e-11e9-87b2-f0c09630bcdc.png)

변경사항을 저장하고 종료한다.

## 2.wordpress 설치 및 config 파일 수정

wordpress 설치하고 config파일 수정은 전에 했던 아래 링크를 참고하면 된다.

[wordpress](https://github.com/PyeongGangKim/21500185pyeonggangkim.github.io/blob/master/_posts/2019-05-12-wordpress-post.md)

![2019-05-06 (46)](https://user-images.githubusercontent.com/49421197/57222888-3b339e80-703f-11e9-9152-f234848c3720.png)

kim의 wordpress가 만들어 졌다.

## 3.또 다른 계정 pg13

다른 계정인 pg13도 위에 방법 그대로 따라하면된다.

![2019-05-06 (48)](https://user-images.githubusercontent.com/49421197/57222986-89e13880-703f-11e9-99f8-b565c09ef8c4.png)

pg13계정에도 wordpress가 만들어진 것을 확인할 수 있다.


