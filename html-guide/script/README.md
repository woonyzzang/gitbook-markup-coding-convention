# script
> type, src 순서로 속성을 선언한다.

**– HTML 경우**
``` html
<script type="text/javascript" src=""></script>
```
**– HTML5 경우**
``` html
<script src=""></script>
```

script는 body 요소 마지막내에 선언하는 것을 원칙으로 한다. 단, 성능 이슈가 있을 시 개발 부서와 협의해서 선언 위치를 변경할 수 있다.

참고: language 속성은 HTML4 이전 버전의 하위 호환성을 위해 사용하는 비표준 속성이므로 사용하지 않는다.

## 내부 자바스크립트
XHTML일 경우 내부 자바스크립트 코드는 CDATA 주석을 선언하고 사용한다.

**– HTML 경우**
``` html
<script type="text/javascript">
    alert('확인');
</script>
```
**– XHTML 경우**
``` html
<script type="text/javascript">
<!--[CDATA[
    alert('확인');
]]-->
</script>
```
**– HTML5 경우**
``` html
<script>
    alert('확인');
</script>
```