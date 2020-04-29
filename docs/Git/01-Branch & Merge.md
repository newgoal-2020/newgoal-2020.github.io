---
layout: default
title: '01. Branch & Merge'
parent: '[2020-04-21] Git - VSCODE'
nav_order: 1
#nav_exclude: true
---
# Branch란?  
브랜치란 독립적으로 어떤 작업을 진행하기 위한 개념이다.  
기능 추가, 버그 수정 등 각각의 작업 영역 관리를 위한 분기이다.  
![](/assets/images/2020-04-21/branch_01.png){: style="border:1px solid rgb(0,0,0);"}  


1. 통합 브랜치  
- 제품으로 출시될 수 있는 브랜치로 가장 최상위의 브랜치이다. 즉, 배포 가능한 상태만을 관리한다.  
- 일반적으로 저장소를 처음 만들었을 때에 생기는 'master' 브랜치를 통합 브랜치로 사용한다.  
- 토픽 브랜치에서 특정 작업이 완료되면 다시 통합 브랜치에 병합하는 방식으로 진행된다.  


2. 토픽 브랜치(Feature branch)  
- 기능 추가나 버그 수정과 같은 단위 작업을 위한 브랜치이다.  
- 통합 브랜치로부터 작업 단위로 만들어낸다.  


# Merge란?  
Merge에 관한 설명  