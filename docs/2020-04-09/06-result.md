---
layout: default
title: '06. 참고사항'
parent: '[2020.04.09] git & github'
nav_order: 6
#nav_exclude: true
---

# 업로드 관련 참고사항
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## docs 파일 경로
```bash
# md 파일 경로 (docs)
$ /docs/

# 이미지 경로
$ /assets/images/
```

---

## md 파일 작성 요령
```bash
# docs xxxx.md 파일 상단
---
layout: default
title: '타이틀명'                        // 좌측 네비게이션에 표시할 타이틀명
nav_order: 2                            // 좌측 네비게이션 내 표시할 순서 지정
has_children: true                      // children docs 여부 
permalink: /docs/2020-04-09             // 해당 경로에 있는 .md 파일링크 목록 표시
nav_exclude: true                       // 설정 시 미노출
parent: '부모 타이틀명'                  // 좌측 네비게이션에서 부모의 타이틀명
grand_parent: Sample Page               // 3step 이상의 children 설정 시 필수 옵션, 현재 기준으로 parent 값으로 설정
---
```

## 로컬환경 셋팅 시 참고사항
```bash
# /just-the-docs.gemspec
# jekyll & jekyll-seo-tag 설치 시 default로 설치된 버전이 다른 경우 로컬환경 서버 실행 시 오류가 발생할 수 있음 참고

# Ruby gem - 리눅스의 yum apt 과 같은 것으로 필요 프로그램을 관리할 수 있는 프로그램
# gem으로 설치 시 jekyll / bundler 의 defult 버전이 다른 경우 로컬환경 서버 실행 시 오류가 발생할 수 있음 참고
```

---

[05. MarkDown 문법]({{ site.baseurl }}{% link docs/2020-04-09/05-markdown.md %}#typography){: .btn .btn-outline }

---