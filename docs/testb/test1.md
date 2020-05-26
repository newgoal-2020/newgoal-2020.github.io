---
layout: default
title: 'test1'
parent: 'testb'
nav_order: 1
#nav_exclude: true
---

# Git & Github 기본설명
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Git
 - 컴퓨터 파일의 변경사항을 추적하고 여러 명의 사용자들 간에 해당 파일들의 작업을 조율하기 위한 **분산 버전 관리 시스템**

 1. **작업 트리(Work Tree)**
   - 우리가 작업하고 있는 폴더, 디렉터리를 말함

 2. **인덱스**
   - 커밋을 실행하기 전의 **저장소와 작업 트리 사이에 존재하는 공간**
   - Staging Area라고도 불림

 3. **스테이징(Staging)**
   - 인덱스에 파일 상태를 기록하는 것

---

## Github
 - **Git을 호스팅해주는 웹 서비스**
 - Git 저장소 서버를 대신 유지 및 관리해주는 서비스

---

## Git Repository (저장소)
 - 파일이나 폴더를 저장해 두는 곳

 - **원격 저장소(Remote Repository)**
   - 파일이 원격 저장소 전용 서버에서 관리되며 여러 사람이 함께 공유하기 위한 저장소
 - **로컬 저장소(Local Repository)**
   - 내 PC에 파일이 저장되는 개인 전용 저장소

---

## Public Repository vs Private Repository

### Public Repository (공개 저장소)
{: .no_toc }
 - 모든 사람들이 접근 및 확인 가능하도록 공개된 저장소

### Private Repository (비공개 저장소)
{: .no_toc }
 - 본인 및 Collaborator로 지정된 사람만 볼 수 있는 비공개 저장소
 - 기존에는 유료로만 지원. 2019년 초 최대 3명까지 Collaborators을 지정 가능한 선에서 무료로 변경

---

## Collaborator vs Contributor

### Collaborator (협력자)
{: .no_toc }
 - 프로젝트의 공동 책임자로 GitHub의 push, pull 권한을 모두 가지고 있는 사람
 - 하나의 프로젝트를 중점적으로 개발하는 개발자들은 Collaborator로 등록하여 작업하는 것이 효율적
 - __Private일때는 최대 3명까지 Collaborators을 지정 가능. 그 이상을 지정해 주려면 비용을 지불해야 함__

### Contributor (기여자)
{: .no_toc }
 - 한 프로젝트의 커밋에 관여하는 모든 사람 (Pull Request가 받아들여진 사람)

---

## Collaborators 등록 방법
 1. Collaborator 추가 할 Repository로 이동
 2. Setting > Manage access 이동
 3. Invite a collaborator 클릭하여 추가할 Github 계정 ID 입력
 4. 초대된 Github 계정 가입 메일 발송되어 승인 시 collaborator 등록 완료

---

[02. Git 개념 및 명령어]({{ site.baseurl }}{% link docs/2020-04-09/02-git-basic-grammar.md %}#typography){: .btn .btn-outline }

---