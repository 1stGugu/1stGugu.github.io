---
layout: post
title: MariaDB 소문자, 대문자 관련 이슈
subtitle: DB명, 테이블, 컬럼명 default 변경
cover-img: /assets/img/path.jpg
thumbnail-img: ''
#gh-repo: daattali/beautiful-jekyll
#gh-badge: [star]
tags: [DEV, DB, MariaDB, Mysql]
comments: true
---


테이블명 및 컬럼명이 소문자로 저장되는 현상이 있어 확인해보니 MariaDB, Mysql의 기본 설정값으로 인한 문제였습니다.


```
lower_case_table_names = 0  // 테이블 생성 및 조회 시 대·소문자 구분한다.  
lower_case_table_names = 1  // 입력 값이 대·소문자든 소문자로 인식 소문자 인식 파일 생성  
lower_case_table_names = 2  // 윈도우에서 대·소문자를 구분해서 테이블생성  

기본값
리눅스, 유닉스 : 0
윈도우 : 1
매킨토시 : 2
```

![MariaDB](/assets/img/post/maria_myini.png){: .mx-auto.d-block :}  
설치경로의 \MariaDB 10.5\data\my.ini 파일을 열어, [mysqld] 아래에 lower_case_table_names = 2 를 입력한 후 저장합니다.

![MariaDB](/assets/img/post/maria_myini_edit.png){: .mx-auto.d-block :}

서비스의 MariaDB를 재시작하면 됩니다.

![MariaDB](/assets/img/post/maria_service.png){: .mx-auto.d-block :}
