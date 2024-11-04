---
layout: post
title: "Github Blog 사용법"
date: 2024-11-04 20:54:00
excerpt: "너도 복잡한 설정따위 집어치우고 Github Blog 사용할 수 있다"
---


## 1. 마음에 드는 jekyll 스타일 fork하기
github 계정이 있다면 [jekyll 스타일 모음](https://jekyllthemes.io/free)에서 원하는 스타일을 고르자.
없다면 후딱 회원가입해 오자

골랐다면 **Get Documentation on Github**을 클릭해 github 레포지토리로 들어간 후 Fork를 클릭하자.

이후 Fork해 올 레포지토리 이름을 본인 깃허브 계정 아이디로 설정하자.

## 2. 설정파일 수정하기
원하는 스타일을 Fork해왔다면 _config.yml 파일로 들어가자.

수정(펜 모양)버튼을 클릭해 아래의 항목들을 수정하자.
name: [내 블로그 타이틀 이름]
baseurl: /[깃허브 아이디]
url: [깃허브 아이디].github.io

다 수정했다면 commit changes를 클릭하고 수정사항이 다 반영될 때 까지 기다리자(몇 분 정도 소요)

## 3. 글 작성하기
수정이 잘 적용된 것을 확인하고 나면 _post 폴더로 들어간 후 상단의 add file 버튼을 클릭하자

이후 먼저 [연]-[월]-[일]-포스트 제목.md 형식으로 파일 이름을 지어주자.

포스트 파일에는 헤더, 본문을 각각 나누어 작성해야 한다.

먼저 헤더는 아래와 같이 ---로 구분지어서 작성한다.

```yml
---
layout: post                    # 레이아웃 설정 
title: "제목"                    # 포스트 제목
date: YYYY-MM-dd HH:mm:ss        # 포스트 작성 시간
categories: [카테고리1, 카테고리2]  # 카테고리 (선택)
tags: [태그1, 태그2]               # 태그 (선택)
excerpt: "요약본"                # 포스트 요약 글(선택)
---
```

본문은 Markdown 형식을 이용해 작성하면 된다.

예시
```
# 환영합니다! - 첫 번째 블로그 포스트

이것은 GitHub Pages에 올리는 첫 번째 포스트입니다. 여기서 간단한 Markdown 문법을 소개해 보겠습니다.

## Markdown 사용 예시

- **굵은 글씨**: `**굵은 글씨**` 또는 `__굵은 글씨__`
- *기울임 글씨*: `*기울임*` 또는 `_기울임_`
- [링크](https://example.com): `[링크](https://example.com)`

### 코드 블록 추가하기

코드 블록을 삽입할 수도 있습니다. 예를 들어, Python 코드 예시는 다음과 같습니다:

```python
def hello_world():
    print("Hello, World!")

```
