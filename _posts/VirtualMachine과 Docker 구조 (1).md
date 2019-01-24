# Docker

### 컨테이너 기반의 오픈소스 가상화 플랫폼



#### 기존의 가상 머신

![Virtual Machine과 Docker](../_posts/VirtualMachine_Docker.png)



#### Virtual Machine

편하기는 하지만 성능이 좋지 않음

느린 속도를 개선하기 위해 반가상화 (Paravirtualization)



**프로세스를 격리**하는 방식의 등장



#### Docker

**반가상화 보다 더 경량화 된 방식**으로, Guest OS 설치 없이 Docker image에 서버 운영에 필요한 프로그램과 라이브러리만 격리해서 설치 할 수 있다. OS 자원은 호스트와 공유해서 사용한다. 이런 방식을 취하면서, 이미지 용량이 크게 줄어들었고, 그림에서 보는 것과 같이 가상화 레이어가 없기 때문에, File System, Network 속도도 가상 머신에 비해서 월등히 빠르다고 할 수 있다. Docker 자체는 Docker image 를 위한 실행 환경으로 보면 된다.



1. Docker image
2. Docker Container



##### 1. Docker image

Docker image는 필요한 프로그램과 라이브러리, 소스를 설치한 뒤 파일로 만든 것이다. 즉, **컨테이너 실행에 필요한 파일과 설정값등을 포함하고 있는 것**으로, 상태값을 가지지 않고 변하지 않는다.



##### 2. Docker Container

Docker Container는 **이미지를 실행한 상태**로, 이미지로 여러 개의 컨테이너를 만들 수 있다. OS로 비유해보면, Docker image는 실행 파일이고, Docker Container는 프로세스라고 할 수 있다.



새로운 서버가 추가되면, Docker image를 다운 받고 컨테이너 생성만 하면 된다.




참고 : https://subicura.com/2017/01/19/docker-guide-for-beginners-2.html
