# input
> label 요소, title 속성, alt 속성을 통해 스크린리더 사용자는 주변 맥락에 대한 이해 없이 각 요소에 독립적으로 접근해도 폼을 이해할수 있다.

``` html
<label for="uid">아이디</label><input type="text" name="uid" id="uid">

<label for="upw">비밀번호</label><input type="password" title="..." name="upw" id="upw">

<input type="image" src="" alt="대체텍스트">
```

다음과 같이 type 값에 따라 속성을 선언한다.

type이 text인 경우: type, title, accesskey, value, name, id 순서로 속성을 선언한다.

``` html
<input type="text" title="" accesskey="" value="" id="">
```

* 동일한 스타일의 텍스트 필드나 너비값이 다르면 style 속성을 이용해 width 값을 제어한다.
* 텍스트 필드에 가이드를 위한 내용이 들어가면 value 속성을 선택적으로 사용할 수 있다.
* label 요소 또는 title 속성을 반드시 선언한다.

type이 raido, checkbox 경우: type, checked , name, id순서로 속성을 선언한다.

``` html
<input type="raido" checked name="vt_align" id="alignLft"><label for="alignLft">왼쪽정렬</label>
<input type="raido" name="vt_align" id="alignCnt"><label for="alignCnt">가운데정렬</label>
<input type="raido" name="vt_align" id="alignRgt"><label for="alignRgt">오른쪽정렬</label>

<input type="checkbox" checked name="sports" id="soccer"><label for="soccer">축구</label>
<input type="checkbox" name="sports" id="basketBall"><label for="basketBall">농구</label>
<input type="checkbox" name="sports" id="tennis"><label for="tennis">테니스</label>
```

* 필요하면 선택적으로 name 속성을 이용해 항목을 그룹으로 나눈다.
* 기본적으로 선택된 값임을 표시하려면 checked라고 표기한다. (XHTML일 경우 checked="checked"라고 표기)
* label 요소와 반드시 함께 사용하며 title 속성은 선언하지 않는다.

type이 image 경우: type, src, alt 순서로 속성을 선언한다. alt 속성은 반드시 선언한다.

``` html
<input type="image" src="" alt="">
```

type이 submit, button, reset인 경우: type 속성을 선언한다. label 요소 또는 title 속성을 선언하지 않는다.

``` html
<input type="button">
```

참고: 특별한 이슈가 아닌 경우를 제외하고는 버튼 요소들은 input 요소를 사용하기 보단 button 요소를 사용한다.