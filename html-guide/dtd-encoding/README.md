# DTD 및 인코딩
> **DOCTYPE**<br>문서타입에 (X)HTML의 버전과 문서형을 지정하는데, 신규 HTML 문서를 작성할 때는 기본 DTD로 HTML 4.01, 하위 브라우져 호환성을 위해 Transitional 모드를 사용 한다.(Transition 모드를 사용하더라도, 웹표준 준수율의 향상을 위해 가급적 Strict 모드의 문법을 사용하는 것을 권장함.) HTML4.01 Transitional DTD를 사용하는 이유는 다음과 같다.
> * XHTML만큼 표현 규칙에 맞는(well-formed) 언어다.
> * XHTML을 사용하면 HTML 기준으로 작성된 PC 환경의 자바스크립트 라이브러리와 호환되지 않는다.
> * XHTML에서 VML이 바르세 표현되지 않는다.

## DTD 선언
HTML 문서는 반드시 DTD를 선언한다.

## 기본 DTD

**– HTML**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```
**– XHTML**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```
**– HTML5 (권장)**
``` html
<!DOCTYPE html>
```

## DTD 종류
**- HTML Strict**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```
**– HTML Transitional**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```
**– HTML Frameset**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd">
```
**– XHTML Strict**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
```
**– XHTML Transitional**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
```
**– XHTML Frameset**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Frameset//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-frameset.dtd">
```
**– HTML5**
``` html
<!DOCTYPE html">
```

[ DTD 형식 ]

| **DTD** | **설명** |
| --- | --- |
| <!DOCTYPE | 현재문서는 |
| html | 일반적으로 html이나 xhtml으로, 최상위 엘리먼트는 html이므로 html로 작성 |
| PUBLIC | PUBLIC 또는 SYSTEM 을 설정, PUBLIC(국제적 공용문서) ⁄ SYSTEM(내부적, 제한적 문서) |
| "-//W3C//DTD XHTML 1.0 Transitional//EN" | 비공인 인증인 W3C기관에 의해 XHTML1.0을 transitional 방식의 영어 공용어를 출력하며 |
| "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd"> | 참조할 DTD문서는 http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd 이다. |
|| **Strict**<br>선언된 (x)HTML 버전의 문법과 구조를 정확하게 사용한다. 지원하지 않는 엘리먼트를 사용해서는 안된다.<br>**Transitional**<br>과도기적으로 사용하기 위한 선언으로, strict보다 유연하다. 선언된 버전 이외의 문법과 구조를 허용한다.<br>**Frameset**<br>Transitional 속성과 더불어, frameset(iframe, frame)을 지원한다.<br>※ frameset은 문서의 구조에 관한 엘리먼트이기 떄문에, transitional에서 frameset을 사용해도 화면표시가 일어난다. 따라서, 사실상 frameset은 transitional과 동일하게 취급된다. |
  
 ## Strict DTD 사라진 엘리먼트
 center, font, iframe, strike, u와 같은 엘리먼트의 사용이 엄격형에서 사용하지 말아야 한다.
 
 [ Strict DTD 금기 사항 ]
 
 | **엘리먼트** | **금기사항** |
 | --- | --- |
 | a | 다른 a 엘리먼트들을 포함 할 수 없다. |
 | pre | img, object, big, small, sub 또는 sup 엘리먼트들을 포함 할 수 없다. |
 | button | input, select, textarea, label, button, form, fieldset, iframe 또는 isindex 엘리먼트들을 포함 할 수 없다. |
 | label | 다른 label 엘리먼트들을 포함 할 수 없다. |
 | form | 다른 form엘리먼트들을 포함 할 수 없고, input 엘리먼트를 직접 사용할 수 없고, 반드시 div,p 엘리먼트와 같은 블록 레벨 요소로 감싸주어야 한다. |
 | body | text⁄img를 직접 사용할 수 없고, 반드시 div,p 엘리먼트와 같은 블록 레벨 요소로 감싸주어야 한다. |
 | blockquote | text는 div, p 엘리먼트와 같은 블록 레벨 요소로 감싸주어야 한다. |
 
 ## Strict DTD 사라진 속성
 
``` text
align : tabel 관련 태그에서만 허용됨(col, colgroup, tbody, td, tfoot, th, thead, tr).
language
background
bgcolor
border : table 태그에서만 허용됨.
height : img, object 태그에서만 허용됨.
hspace
name : HTML 4.01 Strict에서는 허용되고, XHTML 1.0 Strict에서는 form, image 태그를 제외하고 허용됨.
noshade
nowrap
target
text, link, vlink, alink
vspace
width : img, object, table, col, colgroup 태그에서만 허용됨.
```

## Strict DTD 필수 속성
``` dtd
<map name="CDATA">
<area alt="%Text;">
<img src="%URI;" alt="%Text;">
<param name="CDATA">
<form action="%URI;">
<optgroup label="%Text;">
<textarea rows="NUMBER" cols="NUMBER">
<base href="%URI;">
<meta contect="CDATA">
<style type="%ContentType;">
<script type="%ContentType;">
<applet width="%Length;" height="%Length;">
```

주의: 다음과 같은 경우 DTD 설정별 표준 문법으로 작성하더라도 브라우저에서 쿼크 모드로 인식해서 바르게 해석되지 않으므로 주의한다.

**– DTD가 선언되지 않은 경우(html 태그로 문서 시작)**
``` html
<html>
```
**– 선언한 DTD 앞에 다른 문자가 오는 경우**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd">
```

## DTD 적용시 예외
모든 HTML문서는 반드시 DTD를 선언하여야 하지만 아래의 경우 예외 사항으로 Quirks Mode 를 사용한다.

**– DTD가 없는 서비스에 들어가는 문서인 경우**
``` html
<!DOCTYPE html PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN">
```

Quirks Mode 사용시 문제점: CSS Box model상에서 브라우저간 맞지 않는 문제가 있다.

- - -

## 인코딩 선언
HTML 문서는 반드시 인코딩 정보를 선언한다. 인코딩 설정은 DB의 인코딩 방식과도 관련이 있으므로 반드시 담당 개발자와 협의해서 정해야 한다.

## 기본 인코딩
신규 HTML 문서를 작성할 때 기본 인코딩으로 UTF-8을 사용한다. UTF-8은 다국어 지원이 가능하며, EUC-KR보다 표현 가능한 한글(고어, 음절 등)이 더 많다.

**– (X)HTML 인코딩 선언**
``` html
<meta http-equiv="Content-Type" content="text/html;charset=utf-8">
```
**– HTML5 인코딩 선언**
``` html
<meta charset="utf-8">
```

참고: UTF-8은 다음과 같은 특징이 있다.
* 한글은 UTF-8에서 3바이트, EUC-KR에서 2바이트를 차지하므로 인코딩을 UTF-8로 지정하면 DB 저장 용량이나 트래픽이 커진다.
* 인터넷 익스플로러7 이상의 버전에서는 링크의 밑줄이 글자와 붙어 보이는 현상이 있다.

## 기타 인코딩
UTF-8 인코딩을 사용할 수 없으면 EUC-KR을 사용한다.

``` html
<meta http-equiv="Content-Type" content="text/html;charset=euc-kr">
```

HTML, CSS 파일을 저장할 때 반드시 설정한 인코딩을 선택해서 저장한다.