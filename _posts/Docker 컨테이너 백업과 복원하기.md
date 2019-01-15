---
layout: post
title: "Docker 컨테이너 백업과 복원"
date: 2019-01-10
categories: docker
---

# Docker 컨테이너 백업과 복원하기

## Docker 컨테이너 백업

백업 절차는 commit 후 image save를 한다.



### Commit

```shell
$ sudo docker ps -a | grep mysql # mysql 컨테이너가 있는지 확인
```

```zsh
$ sudo docker commit mysql mysql_backup # mysql 컨테이너를 mysql_backup 이라는 이미지로 저장
```



### Image Save

```shell
$ sudo docker save mysql_backup > ~/Desktop/docker_backup/mysql.tar # mysql.tar 라는 이름으로 .tar 파일 저장
```



## Docker 컨테이너 복원

복원 절차는 .tar 로 저장된 파일을 도커 이미지로 load 한다.



### Docker image load

```shell
$ sudo docker load < ~/Desktop/docker_backup/mysql.tar # mysql.tar 파일로부터 docker image 복원
```



위와 같은 방식은 Docker 컨테이너를 Docker Hub에 push, pull 없이 docker 컨테이너 백업 후 .tar 파일로 변경하고, 

.tar 파일을 다른 컴퓨터에서 docker image로 load 하여 사용할 때도 유용하다.



