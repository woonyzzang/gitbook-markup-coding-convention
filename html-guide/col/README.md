# col
> 표 각 열의 너비를 지정하기 위해 선언한다. width, span 속성을 다음과 같은 순서로 선언한다.

* 표 각 열의 너비를 지정하기 위해 선언한다. width, span 속성이 있으며 이 속성은 필요에 따라 선택적으로 사용한다.
* 테이블에 border가 없는 경우에는 `<col width="">` 사용을 한다. border가 있는 경우에 크로스브라우징시 1px 밀리는 이슈가 발생할 수 있는데 이럴경우 `<col class="">` 를 사용하여 CSS에서 width를 핸들링 한다.
* 단, HTML5 DTD 선언 시 col 요소의 width 속성은 전부 class 속성을 줘서 CSS로 핸들링 하거나 `<col style=width:""">` 인라인 style로 핸들링 한다.

**– HTML 경우**
``` html
<col span="2" width="100">
<col width="100">
<col width="*">
<col width="50%">
<col style="width:50%">
```
**– HTML5 경우**
``` html
<col span="2" style="width:100px">
<col style="width:100px">
<col>
<col style="width:50%">
```