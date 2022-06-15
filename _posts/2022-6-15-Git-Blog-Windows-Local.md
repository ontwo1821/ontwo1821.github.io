---
layout: post
title: Git Blog Windows 로컬 환경 구축
---

Git 블로그 시작을 위해 로컬에서 개발 환경을 구성해봤다.

작성은 마크다운을 이용 [https://kramdown.gettalong.org/quickref.html](https://kramdown.gettalong.org/quickref.html)


## 1. jekyll 오픈소스를 fork한 repository를 clone 한다.


~~~ bash
$ git clone https://repostiry주소
~~~

## 2. ruby 다운로드 및 설치

[https://rubyinstaller.org/downloads](https://rubyinstaller.org/downloads)

## 3. jekyll 플러그인 설치 등

~~~ bash
$ gem install github-pages
~~~

## 4. 번들 추가

clone 받은 위치로 이동하여 Gemfile을 생성 및 번들에 jekyll 및 webrick 추가

~~~ bash
$ bundle init
~~~

~~~ bash
$ bundle add webrick
~~~

~~~ bash
$ bundle add jekyll
~~~

## 5. 개발

live reload를 적용하여 빠르게 작성!

~~~ bash
$ jekyll serve -l -o
~~~