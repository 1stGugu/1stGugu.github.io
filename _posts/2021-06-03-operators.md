---
layout: post
title: 연산자 우선순위
subtitle: C
cover-img: /assets/img/path.jpg
thumbnail-img: ''
tags: [DEV, C]
comments: true
---

| 우선순위 | 연산자 | 설명 | 결합 법칙(방향) |
|:---:|:---:|:---:|:---:|
| 1 | x++ | 증가 연산자(뒤, 후위) | → |
| ^^ | x-- | 감소 연산자(뒤, 후위) | ^^ |
| ^^ | ( ) | 함수 호출 | ^^ |
| ^^ | [ ] | 배열 첨자 | ^^ |
| ^^ | . | 구조체/공용체 멤버 접근 | ^^ |
| ^^ | -> | 포인터로 구조체/공용체 멤버 접근 | ^^ |
| ^^ | (자료형){값} | 복합 리터럴 | ^^ |

<table>
    <thead>
      <tr>
        <th>우선순위</th>
        <th>연산자</th>
        <th id="yui_3_17_2_1_1622686702768_58">설명</th>
        <th>결합 법칙(방향)</th>
      </tr>
    </thead>
    <tbody id="yui_3_17_2_1_1622686702768_30">
      <tr id="yui_3_17_2_1_1622686702768_61">
        <td>1<br><br><br><br><br></td>
        <td id="yui_3_17_2_1_1622686702768_60"><span class="cdio-codei">x++<br>x--<br>( )<br>[ ]<br>.<br>-&gt;<br>(자료형){값}</span></td>
        <td id="yui_3_17_2_1_1622686702768_62"><span class="cdio-codei" id="yui_3_17_2_1_1622686702768_84">증가 연산자(뒤, 후위)<br>감소 연산자(뒤, 후위)<br>함수 호출<br>배열 첨자<br>구조체/공용체 멤버 접근<br>포인터로 구조체/공용체 멤버 접근<br>복합 리터럴</span></td>
        <td id="yui_3_17_2_1_1622686702768_63">→<br><br><br><br><br></td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_40">
        <td id="yui_3_17_2_1_1622686702768_83">2<br><br><br><br><br><br><br><br><br><br></td>
        <td id="yui_3_17_2_1_1622686702768_53"><span class="cdio-codei">++x<br>--x<br>+x<br>-x<br>!<br>~<br>(자료형)<br>*x<br>&amp;x<br>sizeof</span></td>
        <td id="yui_3_17_2_1_1622686702768_39"><span class="cdio-codei">증가 연산자(앞, 전위)<br>감소 연산자(앞, 전위)<br>단항 덧셈(양의 부호)<br>단항 뺄셈(음의 부호)<br>
        논리 NOT<br>비트 NOT<br>자료형 캐스팅(자료형 변환)<br>포인터 x 역참조<br>x의 주소<br>자료형의 크기</span><br></td>
        <td id="yui_3_17_2_1_1622686702768_68">←<br><br><br><br><br><br><br><br><br><br><br></td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_66">
        <td>3<br><br><br></td>
        <td id="yui_3_17_2_1_1622686702768_67"><span class="cdio-codei">*<br>/<br>%</span></td>
        <td id="yui_3_17_2_1_1622686702768_65"><span class="cdio-codei" id="yui_3_17_2_1_1622686702768_64">곱셈<br>나눗셈<br>나머지</span></td>
        <td id="yui_3_17_2_1_1622686702768_71">→<br><br><br></td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_70">
        <td>4<br><br></td>
        <td id="yui_3_17_2_1_1622686702768_69"><span class="cdio-codei">+<br>-</span></td>
        <td id="yui_3_17_2_1_1622686702768_72"><span class="cdio-codei">덧셈<br>뺄셈</span></td>
        <td id="yui_3_17_2_1_1622686702768_73">→<br><br></td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_44">
        <td>5<br><br></td>
        <td id="yui_3_17_2_1_1622686702768_74"><span class="cdio-codei">&lt;&lt;<br>&gt;&gt;</span></td>
        <td id="yui_3_17_2_1_1622686702768_45"><span class="cdio-codei">비트를 왼쪽으로 시프트<br>비트를 오른쪽으로 시프트</span></td>
        <td id="yui_3_17_2_1_1622686702768_75">→<br><br></td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_47">
        <td id="yui_3_17_2_1_1622686702768_59">6<br><br><br><br></td>
        <td id="yui_3_17_2_1_1622686702768_76"><span class="cdio-codei">&lt;<br>&lt;=<br>&gt;<br>&gt;=</span></td>
        <td id="yui_3_17_2_1_1622686702768_46"><span class="cdio-codei">작음<br>작거나 같음<br>큼<br>크거나 같음</span></td>
        <td id="yui_3_17_2_1_1622686702768_77">→<br><br><br><br></td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_49">
        <td>7<br><br></td>
        <td id="yui_3_17_2_1_1622686702768_78"><span class="cdio-codei">==<br>!=</span></td>
        <td id="yui_3_17_2_1_1622686702768_50"><span class="cdio-codei">같음<br>다름</span></td>
        <td id="yui_3_17_2_1_1622686702768_48">→<br><br></td>
      </tr>
      <tr>
        <td>8</td>
        <td><span class="cdio-codei">&amp;</span></td>
        <td><span class="cdio-codei">비트 AND</span></td>
        <td>→</td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_52">
        <td>9</td>
        <td><span class="cdio-codei">^</span></td>
        <td id="yui_3_17_2_1_1622686702768_51"><span class="cdio-codei">비트 XOR</span></td>
        <td>→</td>
      </tr>
      <tr>
        <td>10</td>
        <td><span class="cdio-codei">|</span></td>
        <td><span class="cdio-codei">비트 OR</span></td>
        <td>→</td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_57">
        <td>11</td>
        <td><span class="cdio-codei">&amp;&amp;</span></td>
        <td id="yui_3_17_2_1_1622686702768_56"><span class="cdio-codei">논리 AND</span></td>
        <td>→</td>
      </tr>
      <tr>
        <td>12</td>
        <td><span class="cdio-codei">||</span></td>
        <td><span class="cdio-codei">논리 OR</span></td>
        <td>→</td>
      </tr>
      <tr>
        <td>13</td>
        <td><span class="cdio-codei">? :</span></td>
        <td><span class="cdio-codei">삼항 연산자</span></td>
        <td>←</td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_80">
        <td>14<br><br><br><br><br><br><br><br><br><br><br><br></td>
        <td><span class="cdio-codei"><span class="cdio-codei">=<br>+=<br>-=<br>*=<br>/=<br>%=<br>&lt;&lt;=<br>&gt;&gt;=<br>&amp;=<br>^=<br>|=</span><br></span></td>
        <td id="yui_3_17_2_1_1622686702768_79"><span class="cdio-codei">할당<br>덧셈 후 할당<br>뺄셈 후 할당<br>곱셈 후 할당<br>나눗셈 후 할당<br>나머지 연산 후 할당<br>비트를 왼쪽으로 시프트한 후 할당<br>비트를 오른쪽으로 시프트한 후 할당<br>비트 AND 연산 후 할당<br>비트 XOR 연산 후 할당<br>비트 OR 연산 후 할당</span><br></td>
        <td>←<br><br><br><br><br><br><br><br><br><br><br><br></td>
      </tr>
      <tr id="yui_3_17_2_1_1622686702768_82">
        <td>15</td>
        <td><span class="cdio-codei">,</span></td>
        <td><span class="cdio-codei">쉼표(콤마) 연산자</span></td>
        <td id="yui_3_17_2_1_1622686702768_81">→</td>
      </tr>
    </tbody>
  </table>
