---
title: "Welcome to Jekyll!"
date: 2019-05-12 01:47:02 -0400
categories: jekyll update
---
# 1. phpmyadmin 설치

![phpmyadmin 설치](https://user-images.githubusercontent.com/49421197/57193274-3fdf5080-6f74-11e9-98b6-ec9559d6da66.png)

apt-get install phpmyadmin을 사용햇 phpmyadmin 설치

# 2. localhost/phpmyadmin에 들어가지는 지 확인

![phpmyadmin 설치했지만 안됨](https://user-images.githubusercontent.com/49421197/57193314-7d43de00-6f74-11e9-83f9-1cce34fdb04a.png)

localhost/phpmyadmin에 들어가지 않는 것을 확인 할 수 있음

# 3. apache2.conf파일의 내용을 변경

![apache2 conf내용 변경](https://user-images.githubusercontent.com/49421197/57193325-a06e8d80-6f74-11e9-8f98-a15643c9bbe7.png)

/etc/phpmyadmin/apache2.conf에 들어간다.

![내용변경](https://user-images.githubusercontent.com/49421197/57193403-a749d000-6f75-11e9-8e83-838aea8fb52a.png)

Include /etc/phpmyadmin/apache.conf을 맨 마지막줄에 추가한다.

# 4. 다시한번 되는지 확인

![되는거 확인](https://user-images.githubusercontent.com/49421197/57193419-c5173500-6f75-11e9-9d7b-436b2df9d7f2.png)
 
확인하면 되는 것을 볼 수 있다.
