---
layout: post
title: 연산자 우선순위
subtitle: C
cover-img: /assets/img/path.jpg
thumbnail-img: ''
tags: [DEV, C]
comments: true
---

|우선순위|연산자|설명|결합 법칙(방향)|
|---|:---:|:---:|---:|
|1|x++
x--
( )
[ ]
.
->
(자료형){값}|증가 연산자(뒤, 후위)
감소 연산자(뒤, 후위)
함수 호출
배열 첨자
구조체/공용체 멤버 접근
포인터로 구조체/공용체 멤버 접근
복합 리터럴|→|
