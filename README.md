# Git Practice

## Git

> 대표적인 분산형 버전 관리 시스템(DVCS)
> 핵심기능은 버전 관리(Version Control), 백업(Backup), 협업(Collaboration)
>
> 깃의 동작 : 초기화, 커밋, 브랜치, 병합, 푸시



## Git 설치 및 환경 설정

### 윈도우 설치

깃 공식 사이트(https://git-scm.com/) 접속 > 설치 파일 내려받기 > 설치(default)

### config 명령어

### 로컬 사용자

```bash
$ cd 저장소 폴더
$ git config user.name "user_name"
$ git config user.email "user_email"
```

### 글로벌 사용자

```bash
$ git config --global user.name "user_name"
$ git config --global user.email "user_email"
```



## Git 개념 잡기

### 초기화

```bash
$ mkdir '폴더명'
# make directory
$ cd '폴더명' 
# change directory
$ git init
$ ls -a
# ls : 파일 목록 출력, -a : 숨겨진 파일도 함께 출력
```

깃의 저장 공간은 다음과 같다.
작업을 하는 공간(working) / 임시로 저장하는 공간(stage) / 실제로 저장하여 기록하는 공간(repository)

### 워킹 디렉토리

파일의 untracked 상태와 tracked 상태
추적(tracked) 상태로 변경해 주기 위한 명령어 '**git add**'

### 스테이지(=임시 영역)

