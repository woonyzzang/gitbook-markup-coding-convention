# th
> scope, abbr, id 순서로 속성을 선언한다.

* 표에 셀 제목이 명시되지 않은 경우에도 th 요소를 필수로 선언해서 의미에 맞는 제목을 명시한다. (화면에 표시되지 않도록 CSS로 숨김 처리)
* scope 속성은 반드시 선언해야 한다. (scope="col"의 뜻은 세로(column), scope="row"는 가로(row) 이다.)
* abbr과 id 속성은 선택적으로 사용한다.

``` html
<th scope="col" abbr="가격">음식의 가격(won)</th>
```