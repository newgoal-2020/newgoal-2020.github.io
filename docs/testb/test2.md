---
layout: default
title: 'test2'
parent: 'testb'
nav_order: 2
#nav_exclude: true
---

# Git 개념 및 명령어
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 주로 사용하는 Git 명령어

<table class="blog_tbl">
    <tr>
        <th style="width:20%; background:#49483e; color:#f8f8f2;">명령어</th>
        <th style="width:5%; background:#49483e; color:#f8f8f2;">옵션</th>
        <th style="width:20%; background:#49483e; color:#f8f8f2;">예시</th>
        <th style="width:55%; background:#49483e; color:#f8f8f2;">설명</th>
    </tr>
    <tr>
        <td>init<br/>(생성하기)</td>
        <td></td>
        <td>git init</td>
        <td>새로운 git 저장소 생성</td>
    </tr>
    <tr>
        <td>pull<br/>(가져와 병합하기)</td>
        <td></td>
        <td>git pull</td>
        <td>
            원격 저장소에서 로컬 저장소로 업데이트<br/>
            원격 저장소에서 최신 변경 이력을 다운로드하여 내 로컬 저장소에 그 내용을 적용
        </td>
    </tr>
    <tr>
        <td>fetch<br/>(가져오기)</td>
        <td></td>
        <td>git fetch origin</td>
        <td>
            원격 저장소의 내용을 확인만 하고 로컬 데이터와 병합은 하고 싶지 않은 경우 사용하는 명령어<br/>
            원격 저장소의 최신 이력을 확인, 가져온 최신 커밋 이력은 이름 없는 브랜치로 로컬에 가져옴, 'FETCH_HEAD'의 이름으로 체크아웃 가능<br/>
            fetch 명령어 후 merge 를 수행하는 것은 pull 명령어와 동일한 기능
        </td>
    </tr>
    <tr>
        <td>add<br/>(추가하기)</td>
        <td></td>
        <td>git add &#60;인덱스에 등록할 파일명&#62;</td>
        <td>변경사항을 인덱스에 등록</td>
    </tr>
    <tr>
        <td rowspan="1">commit<br/>(기록하기)</td>
        <td>-m</td>
        <td>git commit -m "커밋 내용"</td>
        <td>
            이전 커밋 상태부터 현재 상태까지의 변경 이력이 기록된 커밋(혹은 리비전)이 생성<br/>
            '작업 트리'에 있는 변경 내용을 저장소에 바로 기록하는 것이 아니라 그 사이 공간인 '인덱스'에 파일 상태를 기록(stage - 스테이징 한다고 표현)<br/>
            commit 진행 시, 내용 입력 필수
        </td>
    </tr>
    <tr>
        <td>push<br/>(밀어넣기)</td>
        <td></td>
        <td>git push</td>
        <td>원격 저장소로 변경된 파일을 업로드하는 것</td>
    </tr>
    <tr>
        <td>clone<br/>(복제하기)</td>
        <td></td>
        <td>git clone &#60;URL&#62;</td>
        <td>
            원격 저장소를 복제(원격 저장소의 내용을 통째로 다운로드하는 것)<br/>
            변경 이력도 함께 로컬 저장소에 복제되어 오므로, 원래 원격 저장소와 똑같이 이력을 참조하고 커밋 진행 가능
        </td>
    </tr>
    <tr>
        <td>reset<br/>(되돌리기, 이력 x)</td>
        <td></td>
        <td>git reset &#60;옵션&#62; &#60;돌아가고싶은 커밋&#62;</td>
        <td>돌아가려는 커밋으로 리파지토리는 재설정, 해당 커밋 이후의 이력은 없애는 명령어</td>
    </tr>
    <tr>
        <td>revert<br/>(되돌리기, 이력 o)</td>
        <td></td>
        <td>git revert &#60;되돌릴 커밋&#62;</td>
        <td>상태를 되돌리는 명령어, reset 명령어와 달리 이전 이력은 그대로 유지</td>
    </tr>
    <tr>
        <td>merge<br/>(병합하기)<br/>(바로 합치기)</td>
        <td></td>
        <td></td>
        <td>
            여러 개의 브랜치를 하나로 모을 수 있음<br/>
            내가 끌어온 저장소가 최신 버전이 아닌 경우, 즉 내가 pull 을 실행한 후 다른 사람이 push 를 하여 원격 저장소를 업데이트 해버린 경우에는 위의 그림과 같이 내 push 요청이 거부될 수 있음<br/>
            다른 사람의 업데이트 이력을 내 저장소에도 갱신 해야함
        </td>
    </tr>
    <tr>
        <td>rebase<br/>(병합하기)<br/>(브랜치 이력 재정렬하기)</td>
        <td></td>
        <td></td>
        <td>히스토리 관리를 별로 신경쓰지 않고 혼자서만 커밋하거나 아니면 믿을수 있는 소수만 커밋한다면 merge 대신 rebase 사용 권장</td>
    </tr>
    <tr>
        <td>stash<br/>(임시 저장하기)</td>
        <td></td>
        <td></td>
        <td>
            파일의 변경 내용을 일시적으로 기록해두는 영역<br/>
            작업 트리와 인덱스 내에서 아직 커밋하지 않은 변경을 일시적으로 저장해 둘 수 있음<br/>
            stash 에 저장된 변경 내용은 나중에 다시 불러와 원래의 브랜치나 다른 브랜치에 커밋할 수 있음
        </td>
    </tr>
    <tr>
        <td>checkout<br/>(전환하기)</td>
        <td></td>
        <td>git checkout &#60;브랜치명&#62;</td>
        <td>원하는 다른 브랜치로 전환 시 사용하는 명령어</td>
    </tr>
</table>

## Merge vs Rebase
{: .no_toc }
 - **merge(바로 합치기)**
   - 변경 내용의 이력이 모두 그대로 남아 있기 때문에 이력이 복잡해짐
 - **rebase(브랜치 이력 재정렬하기)**
   - 이력은 단순해지지만, 원래의 커밋 이력이 변경됨. 정확한 이력을 남겨야 할 필요가 있을 경우에는 사용하면 안됨.

## Commit vs Push
{: .no_toc }

![]({% link assets/images/2020-04-09/02-basic-01.png %}){: style="border:1px solid rgb(0,0,0);"}

---

## Branch 종류 [Git-Flow 참고]

### Master Branch
 - **제품으로 출시될 수 있는 브랜치 (배포)**
 - 저장소 생성시 master branch 생성됨
 - 배포 가능한 상태만을 관리, 커밋할 때에는 태그를 사용하여 배포 번호를 기록

### Develop Branch
 - **다음 출시 버전을 개발하는 브랜치 (개발) (병합 대상)**
 - 이 브랜치를 기반으로 개발을 진행

### Feature Branch
 - **기능을 개발하는 브랜치**
 - 기능 개발, 개발 완료 시 Develop Branch로 병합
 - 기본적으로 공유할 필요가 없기 때문에, 원격으로는 관리하지 않음
 - Feature/{branch-name}

### Release Branch
 - **이번 출시 버전을 준비하는 브랜치 (출시)**
 - 릴리즈를 위한 최종적인 버그 수정 등의 개발을 수행
 - 버그를 수정하거나 새로운 기능을 포함한 상태로 모든 기능이 정상적으로 동작하는지 확인
 - 브랜치의 이름은 관례적으로 브랜치 이름 앞에 'release-' 를 붙임

### Hotfix Branch
 - **출시 버전에서 발생한 버그를 수정 하는 브랜치 (버그)**
 - 배포한 버전에 긴급하게 수정을 해야 할 필요가 있을 경우, 'master' 브랜치에서 분기하는 브랜치
 - 브랜치 이름 앞에 'hotfix-'를 붙입

## Git-Flow
{: .no_toc }
 - 저장소를 보다 고수준으로 관리하기 위한 브랜칭 관리 전략(branch management strategy)

![]({% link assets/images/2020-04-09/02-total-branch-01.png %}){: style="width:500px;"}


<br/>

---

## Fork vs Pull Request
### Fork
 - 다른 사람의 Github repository에서 내가 어떤 부분을 수정하거나 추가 기능을 넣고 싶을 때 해당 respository를 내 Github repository로 그대로 복제하는 기능

### Pull Request
 - fork 및 파일 수정 후, 다른 사람의 Github repository에 변경 사항을 적용하고 싶으면 해당 저장소에 요청하는 것
 - pull request가 original repository의 관리자로 부터 승인 되었으면 내가 만든 코드가 commit, merge되어 original 에 반영

<br/>

---

[01. Git & Github 기본설명]({{ site.baseurl }}{% link docs/2020-04-09/01-git-github.md %}#typography){: .btn .btn-outline }
[03. 로컬저장소 환경설정]({{ site.baseurl }}{% link docs/2020-04-09/03-local-repository.md %}#typography){: .btn .btn-outline }

---