---
layout: default
title: '03. 로컬저장소 환경설정'
parent: '[2020.04.09] git & github'
nav_order: 3
#nav_exclude: true
---

# 로컬저장소 개발환경 설정하기
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 설치하기

### Git 설치
 - 다운로드 링크([https://git-scm.com/downloads](https://git-scm.com/downloads))

### Ruby 설치
 - 로컬저장소에서 임시 서버([http://127.0.0.1:4000/](http://127.0.0.1:4000/))를 실행하기 위해선 Jekyll Theme의 기본이 되는 Ruby를 설치해야 함
 - 다운로드 링크([https://rubyinstaller.org/](https://rubyinstaller.org/))

### VS Code 설치
 - 마이크로소프트에서 오픈소스로 개발하고 있는 소스 코드 에디터
 - 다운로드 링크([https://code.visualstudio.com/download](https://code.visualstudio.com/download))

### SourceTree 설치
 - GIT을 GUI로 사용자가 더 쉽게 사용할 수 있도록 하는 Atlassian에서 개발한 프로그램
 - 개인/기업 모두 무료
 - 다운로드 링크([https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/))

![]({% link assets/images/2020-04-09/03-sourcetree-01.png %}){: style="width:500px;"}


---

## 로컬저장소 생성하기 (init)
 - 로컬PC 내에 Remote Repository를 가져올 Local Repository 위치에 디렉터리 생성
 - git 저장소로 사용하기 위한 기본 설정 (git init)

---

## 원격저장소 복제하기 (Clone)
 1. Clone 명령어를 통해 Remote Repository 가져오기
  - 명령어
 2. 소스트리를 활용하여 Remote Repository 가져오기
  - 캡쳐본?

---

## 로컬에서 웹서버를 띄우기 위한 설정
1. git config 설정
  ```bash
    $ git config --global user.name "mobiliansweb"
    $ git config --global user.email "mobiliansweb@kggroup.co.kr"
  ```

2. 라이브러리 설치
  ```bash
    # 필요한 라이브러리 설치
    $ gem install bundle
    $ gem install bundler
    $ gem install minima
    $ gem install jekyll
    $ gem install just-the-docs

    # 라이브러리 업데이트
    $ bundle update
  ```

3. 웹서버 실행
  ```bash
    # 웹서버 실행
    $ bundle exec jekyll serve
  ```
---

## Jekyll 이란?
{: .no_toc }
 - Github에서 개발한 정적 웹사이트를 Generator하는 Tool
 - HTML/CSS등의 정적파일만으로 사이트를 생성하므로 매우 빠르고 가벼우며 무료임
 - Jekyll Themes ( [http://jekyllthemes.org/](http://jekyllthemes.org/) )

---

[02. Git 개념 및 명령어]({{ site.baseurl }}{% link docs/2020-04-09/02-git-basic-grammar.md %}#typography){: .btn .btn-outline }
[04. 원격저장소 업로드]({{ site.baseurl }}{% link docs/2020-04-09/04-remote-upload.md %}#typography){: .btn .btn-outline }

---