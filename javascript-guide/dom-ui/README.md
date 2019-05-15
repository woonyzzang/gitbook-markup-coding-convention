# DOM 제어
> DOM 제어가 필요할 경우 해당 DOM에 조작을 위한 용도의 id나 class를 추가하되, `"ui_"`를 prefix로 명명한다.

``` javascript
// DOM조작은 ui_가 붙은 클래스명이나 아이디를 추가하여 제어한다.
<div class="content ui_content"></div>

<script>
$('.ui_content').on('click', function() {});
</script>
```

스크립트 내부에서는 반드시 필요한 경우를 제외하고는 css를 제어하지 않는다. css를 추가할 경우 화면 레이아웃이 틀어지는 경우가 생길 수 있기 때문에 클래스를 삽입, 제거하는 형태로 제어한다.

``` javascript
<style>
.moveContent{position:absolute}
</style>

<div class="content ui_content"></div>

<script>
var $content = $('.ui_content');

$content.addClass('moveContent');
$content.animate({left:100, top:100, opacity:0}, 700);
</script>
```