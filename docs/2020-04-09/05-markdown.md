---
layout: default
title: '05. MarkDown 문법'
parent: '[2020.04.09] git & github'
nav_order: 5
#nav_exclude: true
---

# MarkDown 문법
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## 제목
```bash
# 텍스트 // h1
## 텍스트 // h2
### 텍스트 // h3
#### 텍스트 // h4
##### 텍스트 // h5
###### 텍스트 // h6
```
# 텍스트
{: .no_toc }
## 텍스트
{: .no_toc }
### 텍스트
{: .no_toc }
#### 텍스트
{: .no_toc }
##### 텍스트
{: .no_toc }
###### 텍스트
{: .no_toc }

---

## 밑줄
```bash
<U>밑줄 표시할 텍스트</U>
```
<U>밑줄 표시할 텍스트</U>

---

## 목차
```bash
    # 숫자로 작성하면 해당 숫자로 표시
    0. TOC
    {:toc}

    # *로 작성하면 목록형으로 표시
    * TOC
    {:toc}

    # 목차 제외
    # 제외하고 싶은 제목 밑에 {: .no_toc }을 추가하면 그 제목은 목차에서 제외됩
    {: .no_toc }
```

---

## 링크
```bash
    # 해당 창에서 페이지 이동
    ['노출할 텍스트']('이동할 URL')
    
    # 새 창에서 페이지 이동
    ['노출할 텍스트']('이동할 URL'){: target="_blank" }
```

[네이버(해당페이지 이동)](https://www.naver.com/)

[네이버(새창 이동)](https://www.naver.com/){: target="_blank" }

---

## 정렬
```bash
    # 가운데 정렬
    안녕하세요
    {: .text-center }

    # 왼쪽 정렬 (해당 jekyll theme css에서는 정의되어 있지 않음..?)
    안녕하세요
    {: .text-left }

    # 오른쪽 정렬 (해당 jekyll theme css에서는 정의되어 있지 않음..?)
    안녕하세요
    {: .text-right }

```

안녕하세요
{: .text-center }

안녕하세요
{: .text-left }

안녕하세요
{: .text-right }

---

## 테이블
```bash
    First Header  | Second Header
    ------------- | -------------
    Content Cell  | Content Cell
    Content Cell  | Content Cell
```

First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

---

## 이미지
```bash
    # ![이미지명](이미지 경로 및 파일명){: 스타일}
    ![markdown-03]({% link assets/images/2020-04-09/04-markdown-03.png %}){: style="border:1px solid rgb(0,0,0);"}
```

![markdown-03]({% link assets/images/2020-04-09/04-markdown-03.png %}){: style="border:1px solid rgb(0,0,0);"}

---

## 블록 인용구
```bash
    > 문단 구분
    >> 문단 구분
    >>> 문단 구분
```
> 문단 구분

>> 문단 구분

>>> 문단 구분

---

## 강조
```bash
    *기울임*
    _기울임_
    **굵게**
    __굵게__
    ~~취소선~~
```

*기울임*

_기울임_

**굵게**

__굵게__

~~취소선~~

---

[Markdown kitchen sink]({% link docs/index-test.md %})

---

[04. 원격저장소 업로드]({{ site.baseurl }}{% link docs/2020-04-09/04-remote-upload.md %}#typography){: .btn .btn-outline }
[06. 참고사항]({{ site.baseurl }}{% link docs/2020-04-09/06-result.md %}#typography){: .btn .btn-outline }

---