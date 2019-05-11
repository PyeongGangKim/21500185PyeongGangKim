# 1.웹 서비스 가동 체크

리눅스에서 firefox에 들어가서 localhost라고 친 후 

it works라고 써여있으면 웹 서비스가 가동되는 것이다.
그리고 그것은 default로 설정되어있는 홈페이지이다.

## 2.localhost index 파일 수정

![localhost변경1](https://user-images.githubusercontent.com/49421197/56878218-e8ca0f00-6a8d-11e9-98eb-ea03f1a74e77.png)

root에 읽기 쓰기 권한이 있기 때문에 root로 들어간다.
![localhost변경2](https://user-images.githubusercontent.com/49421197/56878230-01d2c000-6a8e-11e9-9111-df899dc55e7e.png)


절대 경로를 사용해 root에 있는 var를 들어간다.

![localhost변경3](https://user-images.githubusercontent.com/49421197/56878231-039c8380-6a8e-11e9-8f7c-f2d017fbb256.png)


var에 있는 www디렉토리에 들어간다.
![localhost변경4](https://user-images.githubusercontent.com/49421197/56878232-07300a80-6a8e-11e9-84fd-592620996daa.png)



www에 있는 html디렉토리에 들어간다.

![localhost변경5](https://user-images.githubusercontent.com/49421197/56878234-09926480-6a8e-11e9-84b5-c5562db32d78.png)


index.html에 있는 내용을 hello world로 변환한다.


![localhost변경6](https://user-images.githubusercontent.com/49421197/56878245-14e59000-6a8e-11e9-8557-77c7e823d6c8.png)


localhost의 내용이 아까 변경한 것처럼 hello world가 나타난다.
 





