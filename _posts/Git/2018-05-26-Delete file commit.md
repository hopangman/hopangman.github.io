---
layout: post
title: "Git 삭제한 파일들 한번에 반영하기"
date:   2018-05-26 17:09:00
categories: [Git]
comments: true
---
git status 에 deleted 된 파일들 한번에 지우고 반영하기!  
<!--more-->
  
[참조 블로그](http://devxpert.egloos.com/1034155)  
  
prompt에 git status를 입력하면  
삭제된 파일들이 deleted 되었다며 잔뜩 나올때가 있다.  
  
이럴 때, 가장 기본적인 방법 중 하나는 다음과 같다.  
  
prompt> git rm <file> --> 삭제된 파일들 하나씩 일일이...  
prompt> git commit -m "Message"  
prompt> git push  
  
하지만, 지운 파일이 많을 경우...... 불가능에 가까워진다.. OTL  
  
하지만, 걱정 말자. git 만든 사람들은 똑똑한 사람들이다 ㅎㅎ  
**한 번에 모든 상태를 반영할 수 있는 방법이 있다.**  
  
prompt> git add -u    --> -u 옵션의 의미는 update tracked files  
prompt> git commit -m "Message"  
prompt> git push  
  
이렇게 하면, 한 번에 삭제된 모든 파일을 스테이징에 올리고 저장소에 반영할 수 있다!  