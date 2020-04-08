---
layout: default
title: '04. 원격저장소 업로드'
parent: '[2020.04.09] git & github'
nav_order: 4
#nav_exclude: true
---

# 원격저장소에 업로드하기
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 명령어로 파일 업로드하기
 1. 원격저장소에서 로컬저장소로 가져오기 (Pull)
    ```bash
    $ git pull
    ```

 2. 파일 추가 및 수정, 업로드할 파일 인덱스에 추가하기 (add)
    ```bash
    $ git add 파일경로/파일명
    ```

 3. 원격저장소에 기록하기 (Commit)
    ```bash
    $ git commit -m "커밋내용"
    ```

 4. 원격저장소로 업로드하기 (Push)
    ```bash
    $ git push
    ```

---

## 소스트리로 파일 업로드하기
1. 소스트리에서 github 계정 로그인하기

    ![]({% link assets/images/2020-04-09/04-markdown-01.png %}){: style="border:1px solid rgb(0,0,0);"}

    <br/>

2. 로컬저장소 생성 및 소스 복제하기

    ![]({% link assets/images/2020-04-09/04-markdown-02.png %}){: style="border:1px solid rgb(0,0,0);"}

    <br/>

3. 파일 수정하기
4. 업로드할 파일 선택(Add) 및 기록(Commit)하기
5. 원격저장소로 업로드(Push)하기

    ![]({% link assets/images/2020-04-09/04-markdown-03.png %}){: style="border:1px solid rgb(0,0,0);"}

---

[03. 로컬저장소 환경설정]({{ site.baseurl }}{% link docs/2020-04-09/03-local-repository.md %}#typography){: .btn .btn-outline }
[05. MarkDown 문법]({{ site.baseurl }}{% link docs/2020-04-09/05-markdown.md %}#typography){: .btn .btn-outline }

---