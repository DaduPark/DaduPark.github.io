---
title:  "깃블로그 다른 컴퓨터로 실행"
excerpt: "회사나 다른 컴퓨터에서 바로 실행할수있도록 기록을 남겼다."

categories:
  - Blog
tags:
  - Blog
last_modified_at: 2021-01-21
---

1. Ruby 설치하기
https://rubyinstaller.org/downloads/ 홈페이지에서 ==>Ruby+Devkit 2.7.2-1 (x64) 설치하기

2. Jekyll 과 bundler 설치하기

$ gem install jekyll bundler

3.git clone

$ git clone https://github.com/DaduPark/DaduPark.github.io.git

4. 글 등록
>지킬이 포스트 글로 인식하는 파일들은 _posts 폴더 밑의 YEAR-MONTH-DAY-title.md 형식의 파일들이다.
posts 폴더에 마크다운글등록

cd DaduPark.github.io

$ git add .
$ git commit -m "첫번째 블로그 글 등록"
$ git push -u origin master

5.로컬 컴퓨터에서 블로그 수정사항을 확인
$ bundle exec jekyll serve

>Bundler could not find compatible versions for gem "jekyll-feed": 에러 발생시 [https://m.blog.naver.com/PostView.nhn?blogId=flowerdances&logNo=221110593847&proxyReferer=https:%2F%2Fwww.google.com%2F] 참고
>참고 https://devinlife.com/howto%20github%20pages/first-post/