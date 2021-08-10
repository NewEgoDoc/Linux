## 마운트

리눅스에서 여러가지 하드웨어 장치들을 사용하기 위해 리눅스라는 운영체제에 인식시켜야하는데 이를 가능하게 해주는 것이 마운트(mount) 작업

마운트란 특정장치를 하나의 디렉토리처럼 사용하기 위해 수행하는 작업

/etc/mtab 현재 리눅스 시스템의 마운트된 정보를 보관하고 있는 파일

mount 명령어 = /etc/mtab 파일 내용

마운트 해제 명령어: unmount 

... 너무 당연해서 당황함

![공유폴더 속성](https://user-images.githubusercontent.com/53653597/128816192-92ac1ae5-160c-411a-a3cd-f14016a8b4b1.png)

```
yum install cifs-utils

mount -t cifs  //윈도우IP주소/공유폴더이름 리눅스폴더경로/공유될폴더이름 -o username=윈도우아이디,password=윈도우패스워드

```