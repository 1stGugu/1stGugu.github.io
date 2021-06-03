---
layout: post
title: 정규 표현식 pattern
subtitle: 정규 표현식의 패턴을 정리해보자
cover-img: /assets/img/path.jpg
thumbnail-img: ''
#gh-repo: daattali/beautiful-jekyll
#gh-badge: [star]
tags: [dev]
comments: true
---

**html 태그 제거 정규식**
```javascript
var str;
str.replace(/<(\/)?([a-zA-Z0-9]*)(\s[a-zA-Z]*=[^>]*)?(\s)*(\/)?>/g, "");
```

**탭 제거 정규식**
```javascript
var str;
str.replace(/\t/g, '');
```
