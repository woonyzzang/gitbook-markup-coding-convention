# Layer Popup Layout Guide

## HTML 4.01 ⁄ XHTML 1.0 기본 레이어팝업 레이아웃
신규 HTML문서를 작성할 때는 다음과 같은 기본 HTML문서 구조를 따른다.

``` html
<div class="ly_pop_wrap">
    <!-- ly_pop_header -->
    <div class="ly_pop_header">레이어팝업 헤더 영역</div>
    <!-- //ly_pop_header -->
    <!-- ly_pop_container -->
    <div class="ly_pop_container">
        <!-- ly_pop_content -->
        <div class="ly_pop_content">레이어팝업 콘텐츠 영역</div>
        <!-- //ly_pop_content -->
    </div>
    <!-- //ly_pop_container -->
    <!-- ly_pop_footer -->
    <div class="ly_pop_footer">레이어팝업 푸터 영역</div>
    <!-- //ly_pop_footer -->
</div>
```

## HTML5 기본 레이어팝업 레이아웃
HTML5 DTD를 선언할시에는 다음과 같은 구조를 따른다.

``` html
<article class="ly_pop_wrap">
    <!-- header -->
    <header class="ly_pop_header">레이어팝업 헤더 영역</header>
    <!-- //header -->
    <!-- ly_pop_container -->
    <div class="ly_pop_container">
        <!-- ly_pop_content -->
        <div class="ly_pop_content">레이어팝업 콘텐츠 영역</div>
        <!-- //ly_pop_content -->
    </div>
    <!-- //ly_pop_container -->
    <!-- ly_pop_footer -->
    <footer class="ly_pop_footer">레이어팝업 푸터 영역</footer>
    <!-- //ly_pop_footer -->
</article>
```