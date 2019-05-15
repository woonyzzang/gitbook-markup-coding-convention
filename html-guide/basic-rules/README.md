# HTML 코드 기본 규칙
> HTML 코드를 작성할 때 다음과 같은 기본 규칙을 준수한다.

## W3C Validation
HTML은 해당 DTD의 명세에 맞게 작성하며, W3C Validation을 통과해야 한다.
단, HTML5 DTD 선언 시 다음 오류 내용은 허용한다.

* `<iframe>` 의 frameborder 속성

## 영문 소문자 사용
DTD를 제외한 모든 요소와 속성은 소문자로 작성한다.

[ 소문자 작성 예 ]

**잘못된 예**
``` html
<SPAN class="desc">간단한 설명</SPAN>
```
**올바른 예**
``` html
<span class="desc">간단한 설명</span>
```

## 속성값 표기
속성값은 큰 따움표(" ")로 묶는다.

[ 속성값 표기 예 ]

**잘못된 예**
``` html
<img src='test.gif' width='100' height='100' alt='테스트'>
```
**올바른 예**
``` html
<img src="test.gif" width="100" height="100" alt="테스트">
```

## 엔티티 코드 사용
특수 기호는 엔티티 이름(entity name)을 사용해서 엔티티 코드(entity code)로 변환한다. 엔티티 번호(entity number)는 사용하지 않는다. 단, 작은 따옴표(') 는 엔티티 번호인 &#38;#39;  큰 따옴표(")는 엔티티 번호인 &#38;&#34; 슬래시(/)는 엔티티 번호인 &#47;로 선언한다.

* 엔티티 코드는 ISO-8859-1을 기준으로 하며, 특수기호 엔티티 코드 종류는 아래 참조 링크 문서에서 확인할 수 있다.
* [HTML 4.01 Character entity references](https://www.w3.org/TR/html4/sgml/entities.html)
* [HTML 5 Character entity references](https://www.w3.org/TR/html5/syntax.html#character-references)

[ 엔티티 코드 사용 예 ]

**잘못된 예**
``` html
<a href="…&nid=2">
```
**올바른 예**
``` html
<a href="…&amp;nid=2">
```

참고: <, >, ', ", & 등의 특수기호를 엔티티 코드로 변환하지 않으면 브라우저가 이를 시작 &fral;종료 태그나 속성으로 잘못 해석할 수 있다. 자동으로 생성되는 링크의 경로나 이미지의 alt값에도 엔티티 코드가 바르게 적용되게 한다.