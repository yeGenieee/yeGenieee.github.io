---
layout: post
cover: 'assets/images/cover2.jpg'
navigation: True
title: Docker 기본 명령어 (Docker command)
date: 2019-01-10
tags: mac, ssh
subclass: 'post tag-fiction'
logo: 'assets/images/ghost.png'
author: yeGenieee
categories: docker
---
# Docker 기본 명령어

### docker run

도커 이미지로 도커 컨테이너를 생성하는 명령어

```shell
docker run [옵션] [image 이름 or ID] [명령] [args]
```

##### run 옵션

-v, --volume=[] : 데이터 볼륨 설정, 호스트와 공유할 디렉토리를 설정하여 파일을 컨테이너에 저장하지 않고 호스트에 바로 저장 (***Docker 데이터 볼륨 찾아보기***)

-w, --workdir="" : 컨테이너 내 프로세스가 실행될 디렉토리 설정

-rm=false : 컨테이너 안의 프로세스가 종료되면 컨테이너를 자동으로 삭제 (-d 옵션과 함께 사용할 수 없음)
