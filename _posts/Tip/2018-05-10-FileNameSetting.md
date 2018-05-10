---
layout: post
title: "한글 파일명 오류해결하기!"
date:   2018-05-10 17:37:00
categories: [Tip]
comments: true
---
Mac 터미널로 git에 push하려고 하는데 한글파일명이 /123/123/123/ 이런식의 숫자로 표시되는 경우 해결방법!  
<!--more-->
git status 명령으로 변경 파일을 보면 한글이 \123\456... 와 같이 보이는 문제가 있다.  
보이기만 이렇게 보이는 것이면 그냥 참겠지만 commit 하는 등의 과정에서 파일명을 지정하는게 어려워진다.  
이 문제를 해결하는 방법은 아래와 같다.  
  
[참조 블로그](https://blog.asamaru.net/2017/06/26/mac-os-git-korean-file-name-corequotepath/)
  
```
git config --global core.quotepath false
git config --local core.quotepath false
```
파일명을 영어로 작성하는게 좋겠다..
그런데 영어실력이.... ㅎㅎ